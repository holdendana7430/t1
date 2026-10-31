代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ul.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ay.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xt.huixinmuqiang.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mm.panjiajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ka.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://wk.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rc.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dx.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aj.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ux.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ku.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://md.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zd.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rm.wgjwhj.cn

[E16] 数字千分位
来源：http://xh.szsharing.cn

Py:   f"{1234567:,}"
来源：http://kg.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://ty.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nf.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ee.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vf.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ll.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eo.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://hj.yuntaijiaju.cn

[E17] 首字母大写
来源：http://sl.asd995.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://um.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yq.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iv.wgjwhj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wf.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://up.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ex.shxzskj.cn

Ruby: s.capitalize
来源：http://co.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kg.chemitech.net.cn

[E18] 模板占位符替换
来源：http://ah.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bj.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nf.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kr.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tg.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pd.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fv.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ve.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://km.asd995.cn

[E19] 多行文本按行拆分
来源：http://bn.colortex.cn

Py:   s.splitlines()
来源：http://by.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hh.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://gl.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://uk.szsharing.cn

Java: s.lines().toList()
来源：http://an.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://lh.yuexingan06.cn

Ruby: s.lines
来源：http://ct.shtwfgs.cn

C#:   s.Split('\n')
来源：http://iu.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://gn.shxzskj.cn

Py:   if not s:
来源：http://tp.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fu.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ji.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://wv.wgjwhj.cn

Java: if (s.isEmpty()) {}
来源：http://rg.shxzukj.cn

Go:   if s == "" {}
来源：http://qi.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://qh.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mk.nicolike.cn

[E21] 超长截断加省略号
来源：http://th.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kf.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hj.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tj.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wp.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uk.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://ou.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ii.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vp.hahajie.cn

[E22] 字节长度与字符长度
来源：http://hq.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pk.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dq.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pv.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vs.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wb.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ib.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://da.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xt.521024.cn

================================================================================
来源：http://ek.yuexingan06.cn

F. 文件与目录
来源：http://eq.asd995.cn

================================================================================
来源：http://kc.lnxyls.cn

[F01] 读取整个文件
来源：http://us.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kl.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://nd.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://by.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://at.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zl.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xn.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://hh.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://dv.521024.cn

[F02] 逐行读取文件
来源：http://oi.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://he.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fc.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ed.yuntaijiaju.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vl.nszjky.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jt.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kx.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rv.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eu.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://hr.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qw.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nh.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ir.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jy.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cj.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wi.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://cf.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ro.huanxung.cn

[F04] 追加写入文件
来源：http://sl.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ny.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nj.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ox.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ln.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hw.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qt.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jh.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yg.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://bm.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ei.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://eg.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://sm.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://dw.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cp.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ae.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://yx.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://ea.lnxyls.cn

[F06] 删除文件
来源：http://br.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://lw.hahajie.cn

PHP:  unlink("a.txt");
来源：http://in.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zj.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rx.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uu.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://xi.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://fs.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://xq.huanxung.cn

[F07] 创建目录（含多级）
来源：http://qe.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fe.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ro.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ed.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wg.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tf.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tq.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ec.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hh.gzmigu.cn

[F08] 遍历目录
来源：http://ba.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ln.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://se.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://gf.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://ac.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://as.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hs.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://ux.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://sw.asd995.cn

[F09] 获取文件大小
来源：http://wo.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://jn.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://mf.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://hp.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://ri.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oc.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://db.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://ey.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://qu.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://db.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bo.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ca.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://as.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://xv.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aa.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oi.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bg.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ev.gzmigu.cn

[F11] 复制与移动文件
来源：http://su.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wy.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lf.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sc.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uc.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rk.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hs.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mt.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dz.chemitech.net.cn

[F12] CSV 读写
来源：http://dt.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oj.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rg.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ny.bookmarksfly.cn

TS:   // 同上
来源：http://wb.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lh.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hr.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vg.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ln.wgjwhj.cn

================================================================================
来源：http://ls.bjjhwx.cn

G. 面向对象
来源：http://xc.haigaiapp.cn

================================================================================
来源：http://tc.chemitech.net.cn

[G01] 定义类
来源：http://mt.hahajie.cn

Py:   class User: pass
来源：http://kc.huixiangedu.cn

PHP:  class User {}
来源：http://wu.colortex.cn

JS:   class User {}
来源：http://qm.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://zx.nszjky.cn

Java: class User {}
来源：http://dn.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://ky.asd995.cn

Ruby: class User; end
来源：http://ze.newstarts.cn

C#:   class User {}
来源：http://jl.yuexingan06.cn

[G02] 构造函数
来源：http://rz.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ed.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://pi.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ti.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://hc.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://wk.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xs.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://lw.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://gd.asd995.cn

[G03] 实例属性
来源：http://sb.shxzskj.cn

Py:   self.name = "x"
来源：http://vk.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://mv.haigaiapp.cn

JS:   this.name = "x";
来源：http://pc.521024.cn

TS:   name: string = "x";
来源：http://st.lnxyls.cn

Java: private String name;
来源：http://hh.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bf.newstarts.cn

Ruby: @name = "x"
来源：http://fd.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://on.hahajie.cn

[G04] 定义方法
来源：http://zj.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://yr.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://eq.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://px.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://zb.newstarts.cn

Java: String greet() { return name; }
来源：http://zo.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ix.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://vw.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://si.bjjhwx.cn

[G05] 继承
来源：http://ki.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://pm.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://cq.nszjky.cn

JS:   class Admin extends User {}
来源：http://er.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://td.haigaiapp.cn

Java: class Admin extends User {}
来源：http://ng.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pf.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://ck.jctech888.com.cn

C#:   class Admin : User {}
来源：http://ue.jctech888.com.cn

[G06] 重写方法
来源：http://pf.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://dr.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nc.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://tl.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://am.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://wv.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hm.colortex.cn

Ruby: def greet; "admin"; end
来源：http://lz.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://ty.huixiangedu.cn

[G07] 调用父类方法
来源：http://pk.bookmarksfly.cn

Py:   super().greet()
来源：http://ar.szxytkj.cn

PHP:  parent::greet();
来源：http://bh.szxytkj.cn

JS:   super.greet();
来源：http://qs.szxytkj.cn

TS:   super.greet();
来源：http://jr.jianghongdianzi.cn

Java: super.greet();
来源：http://ux.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qz.jianghongdianzi.cn

Ruby: super
来源：http://jk.chemitech.net.cn

C#:   base.Greet();
来源：http://mq.shtwfgs.cn

[G08] 静态方法与属性
来源：http://sp.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://li.gzmigu.cn

PHP:  public static function f() {}
来源：http://oy.bookmarksfly.cn

JS:   static f() {}
来源：http://vn.nszjky.cn

TS:   static f(): void {}
来源：http://aq.wgjwhj.cn

Java: static void f() {}
来源：http://co.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rn.lnxyls.cn

Ruby: def self.f; end
来源：http://rk.newstarts.cn

C#:   public static void F() {}
来源：http://sb.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://ko.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://rb.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kd.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ez.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://az.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://eq.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://bk.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zc.521024.cn

C#:   interface IShape { double Area(); }
来源：http://sb.jianghongdianzi.cn

[G10] 访问控制
来源：http://bj.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://rw.hnjuh.cn

PHP:  public / protected / private
来源：http://jj.huanxung.cn

JS:   #private 字段；其余公开
来源：http://dg.wgjwhj.cn

TS:   public / protected / private
来源：http://xg.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://ln.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mq.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://tr.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://iu.jctech888.com.cn

[G11] getter / setter
来源：http://bp.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://dv.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gm.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://vk.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://ej.asd995.cn

Java: public String getName() { return name; }
来源：http://rw.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tq.huanxung.cn

Ruby: attr_accessor :name
来源：http://re.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://av.newstarts.cn

[G12] 对象转字符串
来源：http://xt.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://ge.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ft.nicolike.cn

JS:   toString() { return this.name; }
来源：http://xx.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://jk.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://xy.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zy.hahajie.cn

Ruby: def to_s; @name; end
来源：http://np.colortex.cn

C#:   public override string ToString() => Name;
来源：http://rr.szsharing.cn

[G13] 判断对象类型
来源：http://pn.nszjky.cn


<!-- 参考信息 -->