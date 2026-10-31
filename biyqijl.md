代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qh.wgjwhj.cn

[E11] 反转字符串
来源：http://da.haigaiapp.cn

Py:   s[::-1]
来源：http://ol.hnjuh.cn

PHP:  strrev($s);
来源：http://ke.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://vk.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://uw.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lf.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wf.yuntaijiaju.cn

Ruby: s.reverse
来源：http://vi.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fg.9csxet.cn

[E12] 统计某字符出现次数
来源：http://hk.shtwfgs.cn

Py:   s.count("a")
来源：http://vs.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://eb.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://fq.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://hk.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rp.9csxet.cn

Go:   strings.Count(s, "a")
来源：http://tn.panjiajie.cn

Ruby: s.count("a")
来源：http://um.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://gs.bookmarksfly.cn

[E13] 逐字符遍历
来源：http://hw.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://hi.nicolike.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hh.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ss.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pj.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ut.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ua.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cm.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dw.nicolike.cn

[E14] URL 编码与 Base64
来源：http://dl.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cu.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://au.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://at.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ai.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sa.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gy.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cz.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dm.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://kp.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kt.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ex.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ol.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xj.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ft.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pv.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qy.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oj.shxzskj.cn

[E16] 数字千分位
来源：http://ap.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://gs.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://nm.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eq.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qm.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yc.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xx.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ae.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://gy.hahajie.cn

[E17] 首字母大写
来源：http://rd.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://en.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sg.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cg.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cd.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ys.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yl.szxytkj.cn

Ruby: s.capitalize
来源：http://af.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ex.huixinmuqiang.cn

[E18] 模板占位符替换
来源：http://ws.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vt.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gx.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sk.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cz.gzmigu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nc.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ws.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fr.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rv.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://yb.szxytkj.cn

Py:   s.splitlines()
来源：http://yf.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fz.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://ix.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://wm.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://th.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://qv.szxytkj.cn

Ruby: s.lines
来源：http://ml.szxytkj.cn

C#:   s.Split('\n')
来源：http://ni.521024.cn

[E20] 判断字符串是否为空
来源：http://cr.newstarts.cn

Py:   if not s:
来源：http://aq.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cg.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ai.szsharing.cn

TS:   if (s === "") {}
来源：http://fo.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://yc.hahajie.cn

Go:   if s == "" {}
来源：http://df.shtwfgs.cn

Ruby: if s.empty?
来源：http://rv.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://an.hahajie.cn

[E21] 超长截断加省略号
来源：http://op.gzmigu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ra.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xp.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cq.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sm.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gx.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://wp.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uu.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ho.9csxet.cn

[E22] 字节长度与字符长度
来源：http://fv.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ea.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lr.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ce.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vj.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yr.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ex.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://fr.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nn.panjiajie.cn

================================================================================
来源：http://ze.szsharing.cn

F. 文件与目录
来源：http://ld.muxihuayi.cn

================================================================================
来源：http://hs.wgjwhj.cn

[F01] 读取整个文件
来源：http://tm.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oe.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://gg.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ra.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kt.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xy.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sd.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://mv.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://hk.muxihuayi.cn

[F02] 逐行读取文件
来源：http://ul.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dm.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ua.shxzskj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dg.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xg.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xb.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://om.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jz.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cq.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://sc.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ed.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mw.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dh.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fs.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://az.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ed.jianghongdianzi.cn

Ruby: File.write("a.txt", "hi")
来源：http://yx.lnxyls.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hj.shxzukj.cn

[F04] 追加写入文件
来源：http://sc.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kt.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://we.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qh.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ab.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://go.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pn.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ss.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rb.521024.cn

[F05] 判断文件或目录是否存在
来源：http://oy.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vw.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://mr.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://do.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://un.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yr.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gx.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://cq.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://mi.jianghongdianzi.cn

[F06] 删除文件
来源：http://rk.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://lt.nszjky.cn

PHP:  unlink("a.txt");
来源：http://bl.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://og.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://iq.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wf.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://ru.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://yg.asd995.cn

C#:   File.Delete("a.txt");
来源：http://mo.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://de.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xm.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gn.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cz.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ja.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://me.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://az.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uk.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oj.lnxyls.cn

[F08] 遍历目录
来源：http://fi.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cd.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ic.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://cd.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://ll.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bz.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zl.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://cd.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://kf.9csxet.cn

[F09] 获取文件大小
来源：http://ai.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://rf.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://jv.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://wn.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://ay.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cz.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mc.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://gx.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://qj.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://xz.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fc.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wa.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qr.huanxung.cn

TS:   path.extname("a.txt")
来源：http://gx.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hd.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://db.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vp.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tp.shtwfgs.cn

[F11] 复制与移动文件
来源：http://be.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xs.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gp.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vy.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sg.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lk.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tm.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kg.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dh.asd995.cn

[F12] CSV 读写
来源：http://sc.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ns.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vk.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xg.muxihuayi.cn

TS:   // 同上
来源：http://nu.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fs.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wk.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vz.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nb.bjjhwx.cn

================================================================================
来源：http://uw.huixinmuqiang.cn

G. 面向对象
来源：http://jj.bookmarksfly.cn

================================================================================
来源：http://vz.shtwfgs.cn

[G01] 定义类
来源：http://rh.bookmarksfly.cn

Py:   class User: pass
来源：http://zj.yuntaijiaju.cn

PHP:  class User {}
来源：http://ho.jctech888.com.cn

JS:   class User {}
来源：http://wr.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://se.asd995.cn

Java: class User {}
来源：http://se.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://wm.yuntaijiaju.cn

Ruby: class User; end
来源：http://ql.gzmigu.cn

C#:   class User {}
来源：http://lk.nicolike.cn

[G02] 构造函数
来源：http://lf.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://pf.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://nu.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://nv.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://la.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://ey.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wp.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://oa.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://vk.shxzukj.cn

[G03] 实例属性
来源：http://sh.shxzskj.cn

Py:   self.name = "x"
来源：http://iz.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://eq.jctech888.com.cn

JS:   this.name = "x";
来源：http://vc.nicolike.cn

TS:   name: string = "x";
来源：http://bz.nicolike.cn

Java: private String name;
来源：http://jl.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://js.lnxyls.cn

Ruby: @name = "x"
来源：http://pl.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://je.shxzukj.cn

[G04] 定义方法
来源：http://fi.9csxet.cn

Py:   def greet(self): return self.name
来源：http://hc.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bj.nszjky.cn

JS:   greet() { return this.name; }
来源：http://an.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://jr.colortex.cn

Java: String greet() { return name; }
来源：http://xs.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://up.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://dr.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://ys.shxzukj.cn

[G05] 继承
来源：http://jp.asd995.cn

Py:   class Admin(User): pass
来源：http://jr.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://as.muxihuayi.cn

JS:   class Admin extends User {}
来源：http://py.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://jp.chemitech.net.cn

Java: class Admin extends User {}
来源：http://fd.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qm.newstarts.cn

Ruby: class Admin < User; end
来源：http://mg.panjiajie.cn

C#:   class Admin : User {}
来源：http://uw.huixiangedu.cn

[G06] 重写方法
来源：http://uy.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://bi.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ax.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://mx.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://jo.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://es.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ua.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://st.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://wn.wgjwhj.cn

[G07] 调用父类方法
来源：http://lu.jianghongdianzi.cn

Py:   super().greet()
来源：http://se.jctech888.com.cn

PHP:  parent::greet();
来源：http://gq.asd995.cn

JS:   super.greet();
来源：http://lx.hahajie.cn

TS:   super.greet();
来源：http://qv.chemitech.net.cn

Java: super.greet();
来源：http://pa.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xr.521024.cn

Ruby: super
来源：http://lv.yuntaijiaju.cn

C#:   base.Greet();
来源：http://bv.nicolike.cn

[G08] 静态方法与属性
来源：http://op.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nx.yuexingan06.cn

PHP:  public static function f() {}
来源：http://hv.huanxung.cn

JS:   static f() {}
来源：http://uk.wgjwhj.cn

TS:   static f(): void {}
来源：http://sv.huanxung.cn

Java: static void f() {}
来源：http://zo.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bu.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://bv.shxzskj.cn

C#:   public static void F() {}
来源：http://hj.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://ck.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://zp.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uu.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ca.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://yw.jianghongdianzi.cn


<!-- 参考信息 -->