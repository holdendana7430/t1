代发 wailian999

Ruby: s.split(",");  s.split
来源：http://tn.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zq.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://xj.haigaiapp.cn

Py:   ",".join(items)
来源：http://ps.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://oy.wgjwhj.cn

JS:   items.join(",")
来源：http://pa.jianghongdianzi.cn

TS:   items.join(",")
来源：http://zr.521024.cn

Java: String.join(",", items)
来源：http://rh.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://hd.shxzskj.cn

Ruby: items.join(",")
来源：http://ti.lnxyls.cn

C#:   string.Join(",", items)
来源：http://sl.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://fv.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ak.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mr.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://ud.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://rl.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://fo.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uy.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xb.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tt.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://rz.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ap.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fm.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://vi.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://im.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://gw.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cf.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eq.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ke.newstarts.cn

[E11] 反转字符串
来源：http://ar.newstarts.cn

Py:   s[::-1]
来源：http://ue.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://os.521024.cn

JS:   [...s].reverse().join("")
来源：http://hz.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://uy.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://np.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ay.asd995.cn

Ruby: s.reverse
来源：http://uh.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://la.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://qd.shtwfgs.cn

Py:   s.count("a")
来源：http://oz.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://zf.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://np.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://eu.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iv.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://ed.bjjhwx.cn

Ruby: s.count("a")
来源：http://py.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://mg.chemitech.net.cn

[E13] 逐字符遍历
来源：http://bd.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://bn.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://no.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bv.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wc.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yo.szxytkj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vk.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sw.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gh.szsharing.cn

[E14] URL 编码与 Base64
来源：http://ka.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ni.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vr.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hy.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ps.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jx.yuntaijiaju.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xw.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hk.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pj.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://ut.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jg.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://se.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sy.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://us.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kh.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jf.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rx.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cj.nszjky.cn

[E16] 数字千分位
来源：http://cb.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://ym.shxzukj.cn

PHP:  number_format(1234567);
来源：http://cb.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pl.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vd.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yu.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ao.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hf.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://xa.huanxung.cn

[E17] 首字母大写
来源：http://uz.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gc.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://cl.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oh.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://po.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gk.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zb.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://gl.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xs.szsharing.cn

[E18] 模板占位符替换
来源：http://cg.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fw.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pk.chemitech.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yi.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hf.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wb.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://oi.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://of.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ig.asd995.cn

[E19] 多行文本按行拆分
来源：http://uf.hnjuh.cn

Py:   s.splitlines()
来源：http://ax.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yj.hahajie.cn

JS:   s.split(/\r?\n/)
来源：http://ia.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://ne.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://ov.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://pu.huixinmuqiang.cn

Ruby: s.lines
来源：http://tq.lnxyls.cn

C#:   s.Split('\n')
来源：http://vh.nszjky.cn

[E20] 判断字符串是否为空
来源：http://uz.nszjky.cn

Py:   if not s:
来源：http://nq.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mp.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ep.chemitech.net.cn

TS:   if (s === "") {}
来源：http://jd.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://ag.nicolike.cn

Go:   if s == "" {}
来源：http://ls.panjiajie.cn

Ruby: if s.empty?
来源：http://ga.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cz.hnjuh.cn

[E21] 超长截断加省略号
来源：http://ka.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ir.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rf.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ui.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qj.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ks.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ij.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vr.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ui.nicolike.cn

[E22] 字节长度与字符长度
来源：http://vv.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tl.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://av.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xk.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aa.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vd.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nz.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://jt.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xh.shxzskj.cn

================================================================================
来源：http://nr.huixinmuqiang.cn

F. 文件与目录
来源：http://kk.szsharing.cn

================================================================================
来源：http://tl.nicolike.cn

[F01] 读取整个文件
来源：http://mh.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lr.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://yh.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ow.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yd.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zh.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jm.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://pk.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://af.colortex.cn

[F02] 逐行读取文件
来源：http://vc.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ix.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ou.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wm.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xd.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://od.shtwfgs.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mw.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rt.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ng.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://sr.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mw.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fg.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ik.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tk.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ch.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fm.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://gs.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ry.shxzskj.cn

[F04] 追加写入文件
来源：http://oh.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jg.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pc.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zt.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tv.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vd.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://af.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aq.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ea.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://yz.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fy.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://ro.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://lw.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://uq.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jx.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://or.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://bb.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://ru.huixiangedu.cn

[F06] 删除文件
来源：http://ak.hahajie.cn

Py:   os.remove("a.txt")
来源：http://wi.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://oj.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://av.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mp.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ax.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://tz.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://ed.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://st.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://hu.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jl.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tu.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://by.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ge.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cl.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wh.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kp.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qj.muxihuayi.cn

[F08] 遍历目录
来源：http://wg.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cp.panjiajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ua.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://pd.521024.cn

TS:   fs.readdirSync("dir")
来源：http://md.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hl.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ww.asd995.cn

Ruby: Dir.children("dir")
来源：http://sv.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://ro.newstarts.cn

[F09] 获取文件大小
来源：http://fd.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://mh.nicolike.cn

PHP:  filesize("a.txt");
来源：http://ni.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://zy.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://kx.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qr.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yy.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://hk.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://rk.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://mf.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ww.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bd.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kf.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://xr.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yz.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kp.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jo.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yb.wgjwhj.cn

[F11] 复制与移动文件
来源：http://oh.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vb.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rv.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cg.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hc.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mn.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://co.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://um.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lw.asd995.cn

[F12] CSV 读写
来源：http://zr.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zn.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sc.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sr.bjjhwx.cn

TS:   // 同上
来源：http://dw.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ve.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yf.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vq.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xa.jctech888.com.cn

================================================================================
来源：http://xu.jctech888.com.cn

G. 面向对象
来源：http://es.hahajie.cn

================================================================================
来源：http://tq.huanxung.cn

[G01] 定义类
来源：http://zy.chemitech.net.cn

Py:   class User: pass
来源：http://hw.newstarts.cn

PHP:  class User {}
来源：http://fh.521024.cn

JS:   class User {}
来源：http://ds.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://pg.bjjhwx.cn

Java: class User {}
来源：http://qv.nicolike.cn

Go:   type User struct { Name string }
来源：http://fk.szsharing.cn

Ruby: class User; end
来源：http://dk.shtwfgs.cn

C#:   class User {}
来源：http://nh.newstarts.cn

[G02] 构造函数
来源：http://ha.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://kf.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://gl.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://pc.muxihuayi.cn

TS:   constructor(public name: string) {}
来源：http://uz.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://dt.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gh.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://rf.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://nq.newstarts.cn

[G03] 实例属性
来源：http://ck.huanxung.cn

Py:   self.name = "x"
来源：http://sd.newstarts.cn

PHP:  public string $name = "x";
来源：http://hq.colortex.cn

JS:   this.name = "x";
来源：http://xq.hnjuh.cn

TS:   name: string = "x";
来源：http://jy.szsharing.cn

Java: private String name;
来源：http://jr.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eg.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://ad.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://lf.nszjky.cn

[G04] 定义方法
来源：http://ao.hahajie.cn

Py:   def greet(self): return self.name
来源：http://nk.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nk.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://xm.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://va.haigaiapp.cn

Java: String greet() { return name; }
来源：http://tn.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zh.hnjuh.cn

Ruby: def greet; @name; end
来源：http://js.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://pd.521024.cn

[G05] 继承
来源：http://bk.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://lu.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://wy.shxzukj.cn

JS:   class Admin extends User {}
来源：http://bc.gzmigu.cn

TS:   class Admin extends User {}
来源：http://vc.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://fl.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fp.panjiajie.cn

Ruby: class Admin < User; end
来源：http://gk.chemitech.net.cn

C#:   class Admin : User {}
来源：http://dl.newstarts.cn

[G06] 重写方法
来源：http://ny.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://xq.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ae.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://sl.jctech888.com.cn


<!-- 参考信息 -->