代发 wailian999

[E14] URL 编码与 Base64
来源：http://bh.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mj.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lx.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yz.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fe.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pk.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tq.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ze.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cp.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://nj.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yn.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bd.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ig.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ta.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cm.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jr.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://we.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://am.huanxung.cn

[E16] 数字千分位
来源：http://ev.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://tt.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://zc.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fa.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ci.asd995.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ve.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ej.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ah.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://rp.shxzukj.cn

[E17] 首字母大写
来源：http://yh.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ey.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zf.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cm.shxzukj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cr.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hk.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bo.huanxung.cn

Ruby: s.capitalize
来源：http://nv.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ll.szxytkj.cn

[E18] 模板占位符替换
来源：http://ee.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cl.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hh.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ew.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ny.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zf.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qj.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bo.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fw.yuntaijiaju.cn

[E19] 多行文本按行拆分
来源：http://lc.shtwfgs.cn

Py:   s.splitlines()
来源：http://ev.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yl.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://zv.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://uv.asd995.cn

Java: s.lines().toList()
来源：http://yz.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://wl.muxihuayi.cn

Ruby: s.lines
来源：http://sj.gzmigu.cn

C#:   s.Split('\n')
来源：http://bl.newstarts.cn

[E20] 判断字符串是否为空
来源：http://tg.asd995.cn

Py:   if not s:
来源：http://zr.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mc.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sd.panjiajie.cn

TS:   if (s === "") {}
来源：http://fi.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://ng.szxytkj.cn

Go:   if s == "" {}
来源：http://nk.hahajie.cn

Ruby: if s.empty?
来源：http://ru.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zz.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://dn.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ea.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aw.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iq.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rr.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zn.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://kr.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://so.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vi.9csxet.cn

[E22] 字节长度与字符长度
来源：http://ky.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kq.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ja.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wf.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iq.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bl.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vf.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://tw.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kd.gzmigu.cn

================================================================================
来源：http://wo.yuntaijiaju.cn

F. 文件与目录
来源：http://qx.yuntaijiaju.cn

================================================================================
来源：http://fx.shxzskj.cn

[F01] 读取整个文件
来源：http://zy.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ej.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://vz.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fc.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dn.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://il.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ay.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://rt.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://is.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://ql.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tl.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kl.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ob.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eg.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tv.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qa.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dv.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ke.huixiangedu.cn

[F03] 写入文件（覆盖）
来源：http://vk.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ig.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jx.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sh.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uh.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qd.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jm.szxytkj.cn

Ruby: File.write("a.txt", "hi")
来源：http://yc.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ms.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://ed.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zp.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yp.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jh.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zj.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mb.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://at.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qz.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://an.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://te.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://df.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://lr.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://hw.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://zc.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vf.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kt.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://xy.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://vw.bookmarksfly.cn

[F06] 删除文件
来源：http://wb.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://hr.521024.cn

PHP:  unlink("a.txt");
来源：http://lh.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ce.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fb.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zt.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://hj.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://fm.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://nf.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://qi.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ps.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bn.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rh.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sz.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zz.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kl.9csxet.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yk.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cc.huanxung.cn

[F08] 遍历目录
来源：http://oz.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://po.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jo.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://ko.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://sg.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oi.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pj.szsharing.cn

Ruby: Dir.children("dir")
来源：http://jp.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://nc.haigaiapp.cn

[F09] 获取文件大小
来源：http://if.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://cz.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://mx.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://sb.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://vi.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ru.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ib.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://nm.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://on.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://jh.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ap.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jc.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://th.nszjky.cn

TS:   path.extname("a.txt")
来源：http://ub.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pn.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ga.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dt.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dm.bjjhwx.cn

[F11] 复制与移动文件
来源：http://kw.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pr.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rk.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pi.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://da.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gv.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bk.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ml.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kf.9csxet.cn

[F12] CSV 读写
来源：http://sx.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ow.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uh.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yq.nszjky.cn

TS:   // 同上
来源：http://kl.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iq.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oe.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lx.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cq.nszjky.cn

================================================================================
来源：http://ce.yuntaijiaju.cn

G. 面向对象
来源：http://jg.panjiajie.cn

================================================================================
来源：http://ky.shtwfgs.cn

[G01] 定义类
来源：http://qk.nszjky.cn

Py:   class User: pass
来源：http://ey.bjjhwx.cn

PHP:  class User {}
来源：http://fy.521024.cn

JS:   class User {}
来源：http://zx.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://in.jianghongdianzi.cn

Java: class User {}
来源：http://mh.szsharing.cn

Go:   type User struct { Name string }
来源：http://wt.wgjwhj.cn

Ruby: class User; end
来源：http://mw.haigaiapp.cn

C#:   class User {}
来源：http://ax.wgjwhj.cn

[G02] 构造函数
来源：http://ok.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://sx.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://fs.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://ct.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://bq.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://ip.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bk.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://uf.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://sb.jianghongdianzi.cn

[G03] 实例属性
来源：http://zt.gzmigu.cn

Py:   self.name = "x"
来源：http://pm.lnxyls.cn

PHP:  public string $name = "x";
来源：http://xi.lnxyls.cn

JS:   this.name = "x";
来源：http://us.shxzukj.cn

TS:   name: string = "x";
来源：http://yq.shtwfgs.cn

Java: private String name;
来源：http://ga.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gw.shxzskj.cn

Ruby: @name = "x"
来源：http://gy.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://wy.bookmarksfly.cn

[G04] 定义方法
来源：http://if.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://ro.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://px.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://ne.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://jc.jctech888.com.cn

Java: String greet() { return name; }
来源：http://uu.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ak.9csxet.cn

Ruby: def greet; @name; end
来源：http://bz.asd995.cn

C#:   public string Greet() => Name;
来源：http://de.lnxyls.cn

[G05] 继承
来源：http://ba.9csxet.cn

Py:   class Admin(User): pass
来源：http://rh.9csxet.cn

PHP:  class Admin extends User {}
来源：http://qu.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://he.hnjuh.cn

TS:   class Admin extends User {}
来源：http://ht.szsharing.cn

Java: class Admin extends User {}
来源：http://fq.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sj.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://hz.shxzskj.cn

C#:   class Admin : User {}
来源：http://qi.yuntaijiaju.cn

[G06] 重写方法
来源：http://um.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://pr.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mc.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://zp.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://zb.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://to.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://au.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://fo.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://fi.szxytkj.cn

[G07] 调用父类方法
来源：http://bo.bjjhwx.cn

Py:   super().greet()
来源：http://ad.shtwfgs.cn

PHP:  parent::greet();
来源：http://iw.jianghongdianzi.cn

JS:   super.greet();
来源：http://ll.chemitech.net.cn

TS:   super.greet();
来源：http://rf.asd995.cn

Java: super.greet();
来源：http://ye.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lk.gzmigu.cn

Ruby: super
来源：http://rx.yuexingan06.cn

C#:   base.Greet();
来源：http://sh.jctech888.com.cn

[G08] 静态方法与属性
来源：http://eb.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dy.szxytkj.cn

PHP:  public static function f() {}
来源：http://gg.yuntaijiaju.cn

JS:   static f() {}
来源：http://ke.9csxet.cn

TS:   static f(): void {}
来源：http://xb.colortex.cn

Java: static void f() {}
来源：http://wq.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zq.lnxyls.cn

Ruby: def self.f; end
来源：http://vd.521024.cn

C#:   public static void F() {}
来源：http://tp.newstarts.cn

[G09] 接口 / 抽象类
来源：http://hk.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ia.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bk.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vk.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://jg.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://eu.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://sp.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vz.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://re.newstarts.cn

[G10] 访问控制
来源：http://zf.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://il.hahajie.cn

PHP:  public / protected / private
来源：http://tu.asd995.cn

JS:   #private 字段；其余公开
来源：http://rg.hnjuh.cn

TS:   public / protected / private
来源：http://yx.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://af.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://px.gzmigu.cn

Ruby: public / protected / private
来源：http://zt.shxzukj.cn

C#:   public / protected / private / internal
来源：http://xt.bookmarksfly.cn

[G11] getter / setter
来源：http://ik.nicolike.cn

Py:   @property 与 @x.setter
来源：http://ou.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oq.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://jp.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://bi.nszjky.cn

Java: public String getName() { return name; }
来源：http://ke.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://id.nszjky.cn

Ruby: attr_accessor :name
来源：http://hd.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://nk.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://cm.asd995.cn

Py:   def __str__(self): return self.name
来源：http://am.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xr.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://zq.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://dp.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://dz.lnxyls.cn


<!-- 参考信息 -->