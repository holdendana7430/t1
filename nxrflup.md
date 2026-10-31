代发 wailian999

Ruby: s.split(",");  s.split
来源：http://tk.shxzskj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vu.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://yt.wgjwhj.cn

Py:   ",".join(items)
来源：http://vs.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://hr.nszjky.cn

JS:   items.join(",")
来源：http://qk.hnjuh.cn

TS:   items.join(",")
来源：http://sr.wgjwhj.cn

Java: String.join(",", items)
来源：http://oe.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://qm.chemitech.net.cn

Ruby: items.join(",")
来源：http://pz.shxzukj.cn

C#:   string.Join(",", items)
来源：http://lq.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://em.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ds.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zz.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://fw.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://jv.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://xq.gzmigu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://no.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uz.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tg.nszjky.cn

[E10] 左侧补零 / 定长填充
来源：http://wo.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zr.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fn.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://jk.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://gv.gzmigu.cn

Java: String.format("%03d", 7)
来源：http://wt.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zx.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ea.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cg.haigaiapp.cn

[E11] 反转字符串
来源：http://yx.hnjuh.cn

Py:   s[::-1]
来源：http://xl.haigaiapp.cn

PHP:  strrev($s);
来源：http://je.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://uh.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://px.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ev.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gy.9csxet.cn

Ruby: s.reverse
来源：http://as.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wt.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://rq.shtwfgs.cn

Py:   s.count("a")
来源：http://nz.521024.cn

PHP:  substr_count($s, "a");
来源：http://su.nszjky.cn

JS:   s.split("a").length - 1
来源：http://cz.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://ep.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://si.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://vg.chemitech.net.cn

Ruby: s.count("a")
来源：http://mg.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://zb.chemitech.net.cn

[E13] 逐字符遍历
来源：http://nt.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://dt.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sz.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://if.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cw.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mg.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cu.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dv.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ng.521024.cn

[E14] URL 编码与 Base64
来源：http://wc.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hh.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://we.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aq.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hk.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ai.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pn.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tc.yuexingan06.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gx.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://hu.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rc.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sf.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cz.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://li.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ap.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rn.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gm.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dl.shxzukj.cn

[E16] 数字千分位
来源：http://ol.szsharing.cn

Py:   f"{1234567:,}"
来源：http://to.szsharing.cn

PHP:  number_format(1234567);
来源：http://bz.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hs.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kq.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pk.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kx.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://il.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://ds.haigaiapp.cn

[E17] 首字母大写
来源：http://qq.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zg.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sr.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uo.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yo.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vp.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zl.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://ag.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://us.newstarts.cn

[E18] 模板占位符替换
来源：http://fl.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dv.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fz.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cx.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bp.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pe.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bp.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ml.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://nh.asd995.cn

Py:   s.splitlines()
来源：http://wy.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wx.yuexingan06.cn

JS:   s.split(/\r?\n/)
来源：http://uw.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://vl.521024.cn

Java: s.lines().toList()
来源：http://nj.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://pt.nicolike.cn

Ruby: s.lines
来源：http://hd.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://zb.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://to.jctech888.com.cn

Py:   if not s:
来源：http://vd.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fx.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wz.szxytkj.cn

TS:   if (s === "") {}
来源：http://iy.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://ug.newstarts.cn

Go:   if s == "" {}
来源：http://sj.shtwfgs.cn

Ruby: if s.empty?
来源：http://db.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aj.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://eo.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ff.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fj.huixiangedu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mn.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qu.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kj.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://rf.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lh.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rt.asd995.cn

[E22] 字节长度与字符长度
来源：http://sh.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cz.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fw.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iw.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xe.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://co.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ia.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://wi.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hc.muxihuayi.cn

================================================================================
来源：http://js.wgjwhj.cn

F. 文件与目录
来源：http://rg.nszjky.cn

================================================================================
来源：http://lp.muxihuayi.cn

[F01] 读取整个文件
来源：http://cm.chemitech.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dm.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://ys.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hx.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kn.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fz.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nt.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://di.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://it.szsharing.cn

[F02] 逐行读取文件
来源：http://cz.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zh.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://de.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fv.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yx.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sz.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fq.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cp.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jd.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://rf.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ma.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cj.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nd.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jf.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ah.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pn.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://rx.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bx.521024.cn

[F04] 追加写入文件
来源：http://rr.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sl.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hf.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kj.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qb.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sw.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://le.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rk.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://im.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://kb.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cq.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://xs.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://dn.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://dj.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ib.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ew.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://qp.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://si.colortex.cn

[F06] 删除文件
来源：http://af.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://uz.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://kk.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pn.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jn.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mm.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://gz.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://mk.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://al.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://fv.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ex.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zl.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://at.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gk.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ru.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ri.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ur.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rl.wgjwhj.cn

[F08] 遍历目录
来源：http://tr.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uh.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cr.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://ww.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://qz.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://el.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://md.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://rz.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://gn.shtwfgs.cn

[F09] 获取文件大小
来源：http://bw.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://ag.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://ci.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://kw.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://et.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qr.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hc.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://mu.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://dw.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ym.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tx.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vx.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ez.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://xd.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qy.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eu.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xg.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yv.lnxyls.cn

[F11] 复制与移动文件
来源：http://zn.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ig.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fa.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bd.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ev.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ve.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dq.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fc.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ey.yuntaijiaju.cn

[F12] CSV 读写
来源：http://ci.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pw.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://am.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://id.wgjwhj.cn

TS:   // 同上
来源：http://lp.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tk.hahajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ud.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ij.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zt.haigaiapp.cn

================================================================================
来源：http://ef.yuntaijiaju.cn

G. 面向对象
来源：http://bo.huixiangedu.cn

================================================================================
来源：http://by.huanxung.cn

[G01] 定义类
来源：http://gk.chemitech.net.cn

Py:   class User: pass
来源：http://ur.nszjky.cn

PHP:  class User {}
来源：http://jv.wgjwhj.cn

JS:   class User {}
来源：http://fu.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://ur.yuntaijiaju.cn

Java: class User {}
来源：http://ie.nicolike.cn

Go:   type User struct { Name string }
来源：http://wb.nszjky.cn

Ruby: class User; end
来源：http://ov.yuexingan06.cn

C#:   class User {}
来源：http://de.szsharing.cn

[G02] 构造函数
来源：http://zc.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://jg.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://gt.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://oe.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://ag.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://ei.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nu.huixinmuqiang.cn

Ruby: def initialize(name); @name = name; end
来源：http://nv.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://as.huixinmuqiang.cn

[G03] 实例属性
来源：http://ts.yuexingan06.cn

Py:   self.name = "x"
来源：http://ba.nszjky.cn

PHP:  public string $name = "x";
来源：http://dh.huixiangedu.cn

JS:   this.name = "x";
来源：http://sb.shtwfgs.cn

TS:   name: string = "x";
来源：http://gk.bjjhwx.cn

Java: private String name;
来源：http://jp.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xb.9csxet.cn

Ruby: @name = "x"
来源：http://mq.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://nh.jianghongdianzi.cn

[G04] 定义方法
来源：http://zx.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://nr.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ss.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://pj.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://ol.haigaiapp.cn

Java: String greet() { return name; }
来源：http://he.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://eg.colortex.cn

Ruby: def greet; @name; end
来源：http://sj.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://nn.muxihuayi.cn

[G05] 继承
来源：http://iz.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://ix.hahajie.cn

PHP:  class Admin extends User {}
来源：http://ak.panjiajie.cn

JS:   class Admin extends User {}
来源：http://qx.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://cu.hahajie.cn

Java: class Admin extends User {}
来源：http://ba.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dz.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://be.shxzskj.cn

C#:   class Admin : User {}
来源：http://ka.nszjky.cn

[G06] 重写方法
来源：http://jj.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://ug.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rp.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://ky.huanxung.cn


<!-- 参考信息 -->