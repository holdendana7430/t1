代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mg.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lv.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://qr.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://ns.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://we.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wq.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ge.nszjky.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iw.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://ih.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://io.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qf.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://xp.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://ob.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://ha.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rd.colortex.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hs.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lv.szxytkj.cn

[E11] 反转字符串
来源：http://mu.bjjhwx.cn

Py:   s[::-1]
来源：http://kp.jctech888.com.cn

PHP:  strrev($s);
来源：http://ok.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://fr.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://tv.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wr.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://an.jctech888.com.cn

Ruby: s.reverse
来源：http://ui.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hp.colortex.cn

[E12] 统计某字符出现次数
来源：http://dw.newstarts.cn

Py:   s.count("a")
来源：http://br.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://xt.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://hd.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://nd.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pg.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://ow.shxzskj.cn

Ruby: s.count("a")
来源：http://wv.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://ls.nicolike.cn

[E13] 逐字符遍历
来源：http://nv.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://lj.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qw.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yi.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vg.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ji.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ik.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ya.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kf.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://et.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hf.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xy.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ml.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aw.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ui.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qr.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xv.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nx.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://oj.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ce.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vb.lnxyls.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://me.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gy.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mp.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xo.lnxyls.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dv.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cq.huixiangedu.cn

[E16] 数字千分位
来源：http://qw.521024.cn

Py:   f"{1234567:,}"
来源：http://gt.asd995.cn

PHP:  number_format(1234567);
来源：http://dn.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ob.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nv.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cv.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://df.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bx.colortex.cn

C#:   1234567.ToString("N0")
来源：http://gf.jianghongdianzi.cn

[E17] 首字母大写
来源：http://vk.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nm.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dc.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tc.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xr.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dm.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ll.chemitech.net.cn

Ruby: s.capitalize
来源：http://ul.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dq.yuexingan06.cn

[E18] 模板占位符替换
来源：http://ek.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tr.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://te.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dr.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kh.huanxung.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tx.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mx.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gc.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nm.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://px.newstarts.cn

Py:   s.splitlines()
来源：http://bo.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sb.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://lz.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://qy.chemitech.net.cn

Java: s.lines().toList()
来源：http://ii.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://sq.szsharing.cn

Ruby: s.lines
来源：http://qu.shxzukj.cn

C#:   s.Split('\n')
来源：http://nu.colortex.cn

[E20] 判断字符串是否为空
来源：http://gc.asd995.cn

Py:   if not s:
来源：http://kn.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fh.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gx.gzmigu.cn

TS:   if (s === "") {}
来源：http://ek.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://ga.gzmigu.cn

Go:   if s == "" {}
来源：http://as.nicolike.cn

Ruby: if s.empty?
来源：http://zi.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dq.panjiajie.cn

[E21] 超长截断加省略号
来源：http://vt.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hh.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jl.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ga.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ft.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oh.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://eo.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pk.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://we.huanxung.cn

[E22] 字节长度与字符长度
来源：http://kt.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wa.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mx.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ey.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bn.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zj.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vs.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://dv.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sy.jctech888.com.cn

================================================================================
来源：http://nu.wgjwhj.cn

F. 文件与目录
来源：http://mn.jctech888.com.cn

================================================================================
来源：http://ah.asd995.cn

[F01] 读取整个文件
来源：http://xg.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fc.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://jo.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fv.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wc.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eq.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ex.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://av.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://us.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://rq.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ef.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cj.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://da.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lc.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ca.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fi.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qe.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://ot.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kw.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lw.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://me.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ws.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qg.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ay.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://kb.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nn.asd995.cn

[F04] 追加写入文件
来源：http://hc.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://es.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xl.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ow.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pr.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ju.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dx.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mp.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vg.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://xv.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ky.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://uz.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://fk.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://gz.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gu.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wy.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://wg.colortex.cn

C#:   File.Exists("a.txt")
来源：http://dg.szxytkj.cn

[F06] 删除文件
来源：http://sj.huanxung.cn

Py:   os.remove("a.txt")
来源：http://dz.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://vu.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lg.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://iz.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uo.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://dv.colortex.cn

Ruby: File.delete("a.txt")
来源：http://gm.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://gn.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://ew.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qk.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yl.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ad.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dk.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rn.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jj.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://su.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ou.shxzskj.cn

[F08] 遍历目录
来源：http://iq.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uo.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nh.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://ec.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://xt.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mo.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kd.szsharing.cn

Ruby: Dir.children("dir")
来源：http://cc.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://xw.asd995.cn

[F09] 获取文件大小
来源：http://wm.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://fv.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://qc.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://cu.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://nv.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sv.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gc.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://rm.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://vv.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://ah.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sb.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tb.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ma.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://fc.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jx.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xq.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://km.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://an.szxytkj.cn

[F11] 复制与移动文件
来源：http://vs.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lg.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ks.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wp.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zg.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wy.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://py.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bs.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ju.huixiangedu.cn

[F12] CSV 读写
来源：http://vd.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gy.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hb.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iz.hahajie.cn

TS:   // 同上
来源：http://lk.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dk.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xy.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vx.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pf.yuexingan06.cn

================================================================================
来源：http://da.nszjky.cn

G. 面向对象
来源：http://kw.yuntaijiaju.cn

================================================================================
来源：http://is.bjjhwx.cn

[G01] 定义类
来源：http://uf.shtwfgs.cn

Py:   class User: pass
来源：http://tv.shtwfgs.cn

PHP:  class User {}
来源：http://cr.bjjhwx.cn

JS:   class User {}
来源：http://hh.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://ve.gzmigu.cn

Java: class User {}
来源：http://xc.521024.cn

Go:   type User struct { Name string }
来源：http://eb.huixinmuqiang.cn

Ruby: class User; end
来源：http://nx.asd995.cn

C#:   class User {}
来源：http://jc.lnxyls.cn

[G02] 构造函数
来源：http://zv.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://dg.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://jl.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://vm.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://jf.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://hl.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fe.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://wk.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://mc.jianghongdianzi.cn

[G03] 实例属性
来源：http://wc.wgjwhj.cn

Py:   self.name = "x"
来源：http://rq.lnxyls.cn

PHP:  public string $name = "x";
来源：http://qe.shtwfgs.cn

JS:   this.name = "x";
来源：http://nu.yuexingan06.cn

TS:   name: string = "x";
来源：http://eg.shxzukj.cn

Java: private String name;
来源：http://ij.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ol.nicolike.cn

Ruby: @name = "x"
来源：http://ky.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://or.muxihuayi.cn

[G04] 定义方法
来源：http://uf.nicolike.cn

Py:   def greet(self): return self.name
来源：http://ub.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sr.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://nm.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://nk.newstarts.cn

Java: String greet() { return name; }
来源：http://xw.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qs.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://rk.newstarts.cn

C#:   public string Greet() => Name;
来源：http://gi.nszjky.cn

[G05] 继承
来源：http://gc.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://wv.nicolike.cn

PHP:  class Admin extends User {}
来源：http://ty.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://yh.gzmigu.cn

TS:   class Admin extends User {}
来源：http://qw.9csxet.cn

Java: class Admin extends User {}
来源：http://vo.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xl.hahajie.cn

Ruby: class Admin < User; end
来源：http://ry.gzmigu.cn

C#:   class Admin : User {}
来源：http://sq.jctech888.com.cn

[G06] 重写方法
来源：http://ft.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://df.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sj.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://as.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://kf.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://lk.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://ck.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://fd.szxytkj.cn

[G07] 调用父类方法
来源：http://js.jianghongdianzi.cn

Py:   super().greet()
来源：http://pe.huixiangedu.cn

PHP:  parent::greet();
来源：http://hz.jianghongdianzi.cn

JS:   super.greet();
来源：http://es.haigaiapp.cn

TS:   super.greet();
来源：http://mt.521024.cn

Java: super.greet();
来源：http://fj.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ha.shtwfgs.cn


<!-- 参考信息 -->