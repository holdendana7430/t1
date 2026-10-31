代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sq.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://kn.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tm.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gb.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tg.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sy.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jg.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nd.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ij.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zw.asd995.cn

[E16] 数字千分位
来源：http://yi.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://nr.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://xx.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ma.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cm.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gq.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eg.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gt.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://zd.hnjuh.cn

[E17] 首字母大写
来源：http://wi.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://il.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lz.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yn.nicolike.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://us.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ic.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fy.bookmarksfly.cn

Ruby: s.capitalize
来源：http://yo.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jg.gzmigu.cn

[E18] 模板占位符替换
来源：http://yq.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fj.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ui.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fr.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ti.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://is.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dq.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uk.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iz.521024.cn

[E19] 多行文本按行拆分
来源：http://qz.jctech888.com.cn

Py:   s.splitlines()
来源：http://nl.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oj.gzmigu.cn

JS:   s.split(/\r?\n/)
来源：http://fd.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://mr.haigaiapp.cn

Java: s.lines().toList()
来源：http://ds.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://dv.newstarts.cn

Ruby: s.lines
来源：http://df.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://vr.lnxyls.cn

[E20] 判断字符串是否为空
来源：http://bx.chemitech.net.cn

Py:   if not s:
来源：http://wy.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dr.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xz.9csxet.cn

TS:   if (s === "") {}
来源：http://oh.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://yb.asd995.cn

Go:   if s == "" {}
来源：http://hw.wgjwhj.cn

Ruby: if s.empty?
来源：http://sx.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jp.gzmigu.cn

[E21] 超长截断加省略号
来源：http://bj.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ot.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vy.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://og.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ws.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ia.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://vs.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ve.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pb.colortex.cn

[E22] 字节长度与字符长度
来源：http://ih.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fh.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yq.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xn.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://au.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ky.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ay.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://xv.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ov.jianghongdianzi.cn

================================================================================
来源：http://ar.shxzskj.cn

F. 文件与目录
来源：http://ft.shtwfgs.cn

================================================================================
来源：http://kx.yuexingan06.cn

[F01] 读取整个文件
来源：http://yg.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sm.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://jv.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fh.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ht.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nb.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yt.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://gr.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://jl.yuexingan06.cn

[F02] 逐行读取文件
来源：http://it.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fh.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ud.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ee.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zt.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vd.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qb.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ws.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://be.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://nw.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ve.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ll.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rj.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zs.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wr.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://li.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://dg.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bo.hahajie.cn

[F04] 追加写入文件
来源：http://zm.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uy.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vp.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pc.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fs.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://en.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dc.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://io.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vn.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://zo.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vo.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://zl.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://cc.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://xr.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zf.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pd.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://fk.colortex.cn

C#:   File.Exists("a.txt")
来源：http://lg.521024.cn

[F06] 删除文件
来源：http://xp.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://hw.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://rp.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uh.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ks.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oq.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://dm.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://yy.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://hw.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://il.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wg.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://og.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ms.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lb.colortex.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://td.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gl.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bj.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rz.shtwfgs.cn

[F08] 遍历目录
来源：http://du.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://be.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zy.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://wo.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://lk.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bf.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kf.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://df.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://xd.hnjuh.cn

[F09] 获取文件大小
来源：http://gq.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://kz.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://pb.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://zi.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://nn.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ww.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xe.nicolike.cn

Ruby: File.size("a.txt")
来源：http://mi.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://ph.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://jz.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ct.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zp.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ch.bjjhwx.cn

TS:   path.extname("a.txt")
来源：http://te.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rm.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ve.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hb.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sx.gzmigu.cn

[F11] 复制与移动文件
来源：http://wk.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uy.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vr.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gn.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rs.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sn.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zz.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://os.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wx.jianghongdianzi.cn

[F12] CSV 读写
来源：http://gj.9csxet.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xh.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wp.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kg.nszjky.cn

TS:   // 同上
来源：http://xd.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kc.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gd.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ag.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ef.huixiangedu.cn

================================================================================
来源：http://qy.bookmarksfly.cn

G. 面向对象
来源：http://qw.chemitech.net.cn

================================================================================
来源：http://zv.jianghongdianzi.cn

[G01] 定义类
来源：http://ok.nicolike.cn

Py:   class User: pass
来源：http://hi.jctech888.com.cn

PHP:  class User {}
来源：http://wa.colortex.cn

JS:   class User {}
来源：http://yx.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://tz.bjjhwx.cn

Java: class User {}
来源：http://ek.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://us.muxihuayi.cn

Ruby: class User; end
来源：http://zw.nicolike.cn

C#:   class User {}
来源：http://oe.huanxung.cn

[G02] 构造函数
来源：http://pv.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://wr.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://jf.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://bu.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://zv.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://ro.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hs.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://lq.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://vj.yuexingan06.cn

[G03] 实例属性
来源：http://gy.jctech888.com.cn

Py:   self.name = "x"
来源：http://ge.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://lw.9csxet.cn

JS:   this.name = "x";
来源：http://bw.nszjky.cn

TS:   name: string = "x";
来源：http://ek.jctech888.com.cn

Java: private String name;
来源：http://mm.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://us.szsharing.cn

Ruby: @name = "x"
来源：http://tb.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://hz.huixinmuqiang.cn

[G04] 定义方法
来源：http://wh.newstarts.cn

Py:   def greet(self): return self.name
来源：http://zg.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://na.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://mj.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://cb.gzmigu.cn

Java: String greet() { return name; }
来源：http://kt.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://td.9csxet.cn

Ruby: def greet; @name; end
来源：http://hk.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://yi.jctech888.com.cn

[G05] 继承
来源：http://jy.521024.cn

Py:   class Admin(User): pass
来源：http://ic.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://tb.shxzskj.cn

JS:   class Admin extends User {}
来源：http://rl.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://xl.shtwfgs.cn

Java: class Admin extends User {}
来源：http://ot.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hx.szxytkj.cn

Ruby: class Admin < User; end
来源：http://qf.asd995.cn

C#:   class Admin : User {}
来源：http://ty.huixinmuqiang.cn

[G06] 重写方法
来源：http://on.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://is.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fi.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://uu.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://kb.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://kc.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ab.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://hc.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://os.chemitech.net.cn

[G07] 调用父类方法
来源：http://fv.muxihuayi.cn

Py:   super().greet()
来源：http://em.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://dd.colortex.cn

JS:   super.greet();
来源：http://wk.asd995.cn

TS:   super.greet();
来源：http://dq.colortex.cn

Java: super.greet();
来源：http://ft.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wm.chemitech.net.cn

Ruby: super
来源：http://ip.gzmigu.cn

C#:   base.Greet();
来源：http://vq.wgjwhj.cn

[G08] 静态方法与属性
来源：http://gf.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ei.bjjhwx.cn

PHP:  public static function f() {}
来源：http://fc.newstarts.cn

JS:   static f() {}
来源：http://mu.shxzukj.cn

TS:   static f(): void {}
来源：http://cf.huixiangedu.cn

Java: static void f() {}
来源：http://ta.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ce.newstarts.cn

Ruby: def self.f; end
来源：http://bt.haigaiapp.cn

C#:   public static void F() {}
来源：http://vn.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://az.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://xy.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pt.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ii.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://pv.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://yc.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://nj.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zn.521024.cn

C#:   interface IShape { double Area(); }
来源：http://mq.bjjhwx.cn

[G10] 访问控制
来源：http://zb.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://dy.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://ly.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://av.huanxung.cn

TS:   public / protected / private
来源：http://jb.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://kr.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mw.521024.cn

Ruby: public / protected / private
来源：http://cn.lnxyls.cn

C#:   public / protected / private / internal
来源：http://pc.muxihuayi.cn

[G11] getter / setter
来源：http://cm.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://kh.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ei.newstarts.cn

JS:   get name() { return this._name; }
来源：http://sd.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://rt.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://gb.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vi.lnxyls.cn

Ruby: attr_accessor :name
来源：http://js.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://mg.lnxyls.cn

[G12] 对象转字符串
来源：http://lh.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://jy.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://or.szsharing.cn

JS:   toString() { return this.name; }
来源：http://ol.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://th.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://zo.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ga.huanxung.cn

Ruby: def to_s; @name; end
来源：http://iq.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://zp.colortex.cn

[G13] 判断对象类型
来源：http://oj.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://qg.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://vw.shtwfgs.cn

JS:   u instanceof User
来源：http://gf.shtwfgs.cn

TS:   u instanceof User
来源：http://lk.huanxung.cn


<!-- 参考信息 -->