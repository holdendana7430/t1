代发 wailian999

JS:   [...s].reverse().join("")
来源：http://fn.colortex.cn

TS:   [...s].reverse().join("")
来源：http://qs.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lr.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gu.lnxyls.cn

Ruby: s.reverse
来源：http://hz.yuexingan06.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zo.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://dw.jctech888.com.cn

Py:   s.count("a")
来源：http://ks.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://cy.nicolike.cn

JS:   s.split("a").length - 1
来源：http://oi.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://xq.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://th.asd995.cn

Go:   strings.Count(s, "a")
来源：http://zx.muxihuayi.cn

Ruby: s.count("a")
来源：http://kh.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://wg.colortex.cn

[E13] 逐字符遍历
来源：http://ft.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://sz.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jd.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://pl.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yy.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nz.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sb.nicolike.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://au.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ob.chemitech.net.cn

[E14] URL 编码与 Base64
来源：http://ek.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cw.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bv.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tp.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fj.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qx.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cp.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jr.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://mx.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ae.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sd.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lk.huixinmuqiang.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hm.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uj.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ps.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nr.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ge.huixinmuqiang.cn

[E16] 数字千分位
来源：http://kq.521024.cn

Py:   f"{1234567:,}"
来源：http://qe.9csxet.cn

PHP:  number_format(1234567);
来源：http://kt.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wi.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://in.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ih.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ti.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ar.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://dl.shtwfgs.cn

[E17] 首字母大写
来源：http://uy.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gv.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dx.521024.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lw.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://su.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dk.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iu.nszjky.cn

Ruby: s.capitalize
来源：http://uy.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xs.hahajie.cn

[E18] 模板占位符替换
来源：http://pt.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uo.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ok.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cz.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zr.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ld.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mw.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ol.bookmarksfly.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fo.newstarts.cn

[E19] 多行文本按行拆分
来源：http://ko.gzmigu.cn

Py:   s.splitlines()
来源：http://wr.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lx.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://vz.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://oa.yuexingan06.cn

Java: s.lines().toList()
来源：http://pl.521024.cn

Go:   strings.Split(s, "\n")
来源：http://uo.wgjwhj.cn

Ruby: s.lines
来源：http://bl.yuexingan06.cn

C#:   s.Split('\n')
来源：http://cy.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://ms.panjiajie.cn

Py:   if not s:
来源：http://xi.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oj.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dz.shtwfgs.cn

TS:   if (s === "") {}
来源：http://tz.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://lp.nszjky.cn

Go:   if s == "" {}
来源：http://gv.shtwfgs.cn

Ruby: if s.empty?
来源：http://rr.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gy.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://ro.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qh.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fn.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mk.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aj.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qr.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://ff.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uq.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vq.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://mr.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vp.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ey.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zj.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sn.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pi.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://um.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://cg.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bq.szsharing.cn

================================================================================
来源：http://co.muxihuayi.cn

F. 文件与目录
来源：http://fj.jianghongdianzi.cn

================================================================================
来源：http://hq.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://qf.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wd.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://xm.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tp.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mz.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yd.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ts.521024.cn

Ruby: File.read("a.txt")
来源：http://rr.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://zx.wgjwhj.cn

[F02] 逐行读取文件
来源：http://dp.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mc.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gw.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rz.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://il.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ff.newstarts.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oc.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gw.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yg.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://sk.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nv.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nk.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qx.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://os.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zn.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yn.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://ix.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cw.nicolike.cn

[F04] 追加写入文件
来源：http://wt.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ki.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wv.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gv.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wd.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xk.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sl.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fr.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sy.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://lf.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rr.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://sq.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://yr.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://is.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jk.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gl.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://am.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://io.nicolike.cn

[F06] 删除文件
来源：http://tn.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://ot.nszjky.cn

PHP:  unlink("a.txt");
来源：http://li.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cp.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://il.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ot.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://cs.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://bc.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://ca.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://ll.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rz.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fh.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://il.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ut.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fe.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zm.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nw.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tc.yuexingan06.cn

[F08] 遍历目录
来源：http://tc.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xq.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wl.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://az.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://mp.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wa.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nk.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://ds.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://od.shtwfgs.cn

[F09] 获取文件大小
来源：http://vk.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://ih.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://jz.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://yc.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://nd.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qs.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ij.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://sf.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://cb.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://rq.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ht.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bx.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rg.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://tm.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tk.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nj.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ok.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xs.shtwfgs.cn

[F11] 复制与移动文件
来源：http://os.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ft.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mk.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ci.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pa.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bu.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kw.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zy.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fr.colortex.cn

[F12] CSV 读写
来源：http://sn.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jt.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sb.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pl.chemitech.net.cn

TS:   // 同上
来源：http://po.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xc.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ns.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fy.huixiangedu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jg.yuntaijiaju.cn

================================================================================
来源：http://mt.huixinmuqiang.cn

G. 面向对象
来源：http://wl.asd995.cn

================================================================================
来源：http://qt.gzmigu.cn

[G01] 定义类
来源：http://uo.shxzskj.cn

Py:   class User: pass
来源：http://ad.huixiangedu.cn

PHP:  class User {}
来源：http://im.huixinmuqiang.cn

JS:   class User {}
来源：http://lk.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://rb.nszjky.cn

Java: class User {}
来源：http://tw.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://ci.colortex.cn

Ruby: class User; end
来源：http://eq.yuexingan06.cn

C#:   class User {}
来源：http://al.shtwfgs.cn

[G02] 构造函数
来源：http://cv.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://gl.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://nh.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://lt.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://ar.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://ko.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hs.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://lj.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://do.szsharing.cn

[G03] 实例属性
来源：http://uh.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://zx.9csxet.cn

PHP:  public string $name = "x";
来源：http://bn.huixiangedu.cn

JS:   this.name = "x";
来源：http://uo.9csxet.cn

TS:   name: string = "x";
来源：http://qd.shxzskj.cn

Java: private String name;
来源：http://ww.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://td.521024.cn

Ruby: @name = "x"
来源：http://su.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://uu.asd995.cn

[G04] 定义方法
来源：http://by.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://vx.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lp.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://jn.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://tt.jctech888.com.cn

Java: String greet() { return name; }
来源：http://ya.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xn.szsharing.cn

Ruby: def greet; @name; end
来源：http://ve.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://uu.jianghongdianzi.cn

[G05] 继承
来源：http://pk.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://il.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://yn.hahajie.cn

JS:   class Admin extends User {}
来源：http://ds.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://qn.gzmigu.cn

Java: class Admin extends User {}
来源：http://hs.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aq.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://le.lnxyls.cn

C#:   class Admin : User {}
来源：http://gb.yuexingan06.cn

[G06] 重写方法
来源：http://ne.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://yc.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ob.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://ml.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://jq.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://zx.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://em.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://lk.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://rz.asd995.cn

[G07] 调用父类方法
来源：http://uh.shxzukj.cn

Py:   super().greet()
来源：http://kx.shtwfgs.cn

PHP:  parent::greet();
来源：http://nh.shtwfgs.cn

JS:   super.greet();
来源：http://es.hahajie.cn

TS:   super.greet();
来源：http://cr.chemitech.net.cn

Java: super.greet();
来源：http://oc.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aq.shxzukj.cn

Ruby: super
来源：http://lk.newstarts.cn

C#:   base.Greet();
来源：http://pu.hnjuh.cn

[G08] 静态方法与属性
来源：http://gw.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rm.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://ty.nszjky.cn

JS:   static f() {}
来源：http://gz.yuexingan06.cn

TS:   static f(): void {}
来源：http://ar.nicolike.cn

Java: static void f() {}
来源：http://za.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jk.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://qv.muxihuayi.cn

C#:   public static void F() {}
来源：http://jb.huanxung.cn

[G09] 接口 / 抽象类
来源：http://bx.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://tr.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cv.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yi.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://bj.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://lo.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://jk.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jp.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://rq.bookmarksfly.cn


<!-- 参考信息 -->