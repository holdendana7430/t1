代发 wailian999

PHP:  implode(",", $items);
来源：http://rs.newstarts.cn

JS:   items.join(",")
来源：http://fy.jctech888.com.cn

TS:   items.join(",")
来源：http://kk.muxihuayi.cn

Java: String.join(",", items)
来源：http://wv.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://kb.chemitech.net.cn

Ruby: items.join(",")
来源：http://sc.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://xf.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://xs.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qs.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ru.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://cp.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://sc.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://qa.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ze.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xq.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hn.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://zx.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tq.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gw.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://ax.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://cv.nszjky.cn

Java: String.format("%03d", 7)
来源：http://gq.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ub.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pg.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ze.colortex.cn

[E11] 反转字符串
来源：http://dn.9csxet.cn

Py:   s[::-1]
来源：http://xv.newstarts.cn

PHP:  strrev($s);
来源：http://mn.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://sk.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://wj.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jy.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ut.nszjky.cn

Ruby: s.reverse
来源：http://wz.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ok.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://bn.huixinmuqiang.cn

Py:   s.count("a")
来源：http://iz.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://jp.szsharing.cn

JS:   s.split("a").length - 1
来源：http://ij.9csxet.cn

TS:   s.split("a").length - 1
来源：http://nx.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gn.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://ak.shxzskj.cn

Ruby: s.count("a")
来源：http://tn.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://ds.nicolike.cn

[E13] 逐字符遍历
来源：http://ik.chemitech.net.cn

Py:   for ch in s: print(ch)
来源：http://gu.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yx.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ba.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rk.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yb.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xk.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yv.bookmarksfly.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tt.szsharing.cn

[E14] URL 编码与 Base64
来源：http://fk.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ev.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dh.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wg.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qh.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bu.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qk.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nx.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xt.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://dv.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wg.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ur.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ss.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://je.shxzukj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gn.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ur.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lk.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gr.huixinmuqiang.cn

[E16] 数字千分位
来源：http://pn.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://ck.panjiajie.cn

PHP:  number_format(1234567);
来源：http://kz.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gm.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xg.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rl.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://de.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hk.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://xy.colortex.cn

[E17] 首字母大写
来源：http://xy.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vq.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ah.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yv.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eq.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lc.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jh.chemitech.net.cn

Ruby: s.capitalize
来源：http://ui.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ui.9csxet.cn

[E18] 模板占位符替换
来源：http://hi.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yk.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hg.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zn.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ha.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ow.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xq.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ty.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kr.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://fd.521024.cn

Py:   s.splitlines()
来源：http://zp.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oy.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://tn.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://fx.lnxyls.cn

Java: s.lines().toList()
来源：http://nu.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://dp.nszjky.cn

Ruby: s.lines
来源：http://wm.colortex.cn

C#:   s.Split('\n')
来源：http://wg.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://cz.shtwfgs.cn

Py:   if not s:
来源：http://rr.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://st.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sy.hahajie.cn

TS:   if (s === "") {}
来源：http://mb.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://ha.shxzskj.cn

Go:   if s == "" {}
来源：http://zz.9csxet.cn

Ruby: if s.empty?
来源：http://wk.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pl.szxytkj.cn

[E21] 超长截断加省略号
来源：http://vo.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ti.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gs.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tf.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vl.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://la.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://xy.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://li.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iy.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://st.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ve.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qy.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cu.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ux.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fy.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ez.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://hc.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kg.jctech888.com.cn

================================================================================
来源：http://yk.yuntaijiaju.cn

F. 文件与目录
来源：http://gy.shxzukj.cn

================================================================================
来源：http://uk.hnjuh.cn

[F01] 读取整个文件
来源：http://hn.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gq.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://vx.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bt.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wd.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wt.lnxyls.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nj.nicolike.cn

Ruby: File.read("a.txt")
来源：http://eu.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://wl.nszjky.cn

[F02] 逐行读取文件
来源：http://sg.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://py.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nk.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ev.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kx.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xo.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sk.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ps.jctech888.com.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lm.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://cx.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kh.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://td.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fo.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://om.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rf.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sc.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://rq.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vs.szsharing.cn

[F04] 追加写入文件
来源：http://mp.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ul.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yl.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ya.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fm.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bc.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jv.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://me.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yw.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://in.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hf.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://ab.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://pn.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://ry.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hy.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://go.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://yg.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://an.bjjhwx.cn

[F06] 删除文件
来源：http://oj.521024.cn

Py:   os.remove("a.txt")
来源：http://ei.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://fp.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zw.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ow.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pz.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://do.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://ob.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://od.newstarts.cn

[F07] 创建目录（含多级）
来源：http://kv.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://em.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ub.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xr.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ox.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://am.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pn.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bl.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://im.gzmigu.cn

[F08] 遍历目录
来源：http://nn.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sd.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qr.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://ru.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://ve.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://db.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yu.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://sl.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://fe.nicolike.cn

[F09] 获取文件大小
来源：http://ot.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://yg.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://db.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://nw.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://bh.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iu.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jk.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://sw.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://ap.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://fm.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gz.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fd.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ep.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://og.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hd.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hm.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nd.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ub.szsharing.cn

[F11] 复制与移动文件
来源：http://fq.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iv.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qh.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tn.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xn.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jg.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vf.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lx.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vb.wgjwhj.cn

[F12] CSV 读写
来源：http://tg.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gm.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bc.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iz.shxzukj.cn

TS:   // 同上
来源：http://iy.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://np.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qk.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kv.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nn.szsharing.cn

================================================================================
来源：http://dh.lnxyls.cn

G. 面向对象
来源：http://ip.9csxet.cn

================================================================================
来源：http://fq.jctech888.com.cn

[G01] 定义类
来源：http://aa.bookmarksfly.cn

Py:   class User: pass
来源：http://zd.chemitech.net.cn

PHP:  class User {}
来源：http://wy.hahajie.cn

JS:   class User {}
来源：http://zp.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://oj.yuexingan06.cn

Java: class User {}
来源：http://jc.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://ep.newstarts.cn

Ruby: class User; end
来源：http://co.yuntaijiaju.cn

C#:   class User {}
来源：http://sh.9csxet.cn

[G02] 构造函数
来源：http://rl.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://vu.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://ef.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://td.521024.cn

TS:   constructor(public name: string) {}
来源：http://mg.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://ff.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ta.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://qe.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://bn.szxytkj.cn

[G03] 实例属性
来源：http://gl.521024.cn

Py:   self.name = "x"
来源：http://ey.colortex.cn

PHP:  public string $name = "x";
来源：http://tb.panjiajie.cn

JS:   this.name = "x";
来源：http://lu.shxzukj.cn

TS:   name: string = "x";
来源：http://dx.nszjky.cn

Java: private String name;
来源：http://gh.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dp.szsharing.cn

Ruby: @name = "x"
来源：http://fe.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://cb.nicolike.cn

[G04] 定义方法
来源：http://rz.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://ji.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ku.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://la.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://tq.huixiangedu.cn

Java: String greet() { return name; }
来源：http://zl.shxzskj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://or.shxzskj.cn

Ruby: def greet; @name; end
来源：http://az.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://lo.9csxet.cn

[G05] 继承
来源：http://oy.lnxyls.cn

Py:   class Admin(User): pass
来源：http://vd.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://kd.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://lx.asd995.cn

TS:   class Admin extends User {}
来源：http://iv.521024.cn

Java: class Admin extends User {}
来源：http://pz.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wt.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://sm.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://tj.muxihuayi.cn

[G06] 重写方法
来源：http://vi.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://kt.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yx.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://ri.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://iz.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://gi.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://og.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://bt.shxzukj.cn


<!-- 参考信息 -->