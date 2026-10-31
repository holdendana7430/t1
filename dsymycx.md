代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bi.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yr.yuexingan06.cn

[E16] 数字千分位
来源：http://ua.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://ql.9csxet.cn

PHP:  number_format(1234567);
来源：http://vn.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ps.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gx.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xk.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lu.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://if.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://ou.bjjhwx.cn

[E17] 首字母大写
来源：http://vv.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ls.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fy.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cg.shxzskj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gy.wgjwhj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sw.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ou.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://ik.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rm.colortex.cn

[E18] 模板占位符替换
来源：http://ro.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iw.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vn.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bj.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://on.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://st.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fi.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tj.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rz.colortex.cn

[E19] 多行文本按行拆分
来源：http://zt.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://hw.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ty.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://nz.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://bs.9csxet.cn

Java: s.lines().toList()
来源：http://ex.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://bs.panjiajie.cn

Ruby: s.lines
来源：http://rk.shtwfgs.cn

C#:   s.Split('\n')
来源：http://tv.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://oe.yuntaijiaju.cn

Py:   if not s:
来源：http://rk.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xs.asd995.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://es.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://hy.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://rs.lnxyls.cn

Go:   if s == "" {}
来源：http://me.huanxung.cn

Ruby: if s.empty?
来源：http://fc.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ku.panjiajie.cn

[E21] 超长截断加省略号
来源：http://zu.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ak.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cw.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vt.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kj.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nm.chemitech.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://ty.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kr.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bx.huanxung.cn

[E22] 字节长度与字符长度
来源：http://uc.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rg.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fx.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zu.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ay.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ul.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dm.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://om.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rk.shxzukj.cn

================================================================================
来源：http://qk.jianghongdianzi.cn

F. 文件与目录
来源：http://se.shtwfgs.cn

================================================================================
来源：http://fn.newstarts.cn

[F01] 读取整个文件
来源：http://fz.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nl.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://dc.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vx.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vj.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fp.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ko.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://xl.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://vt.chemitech.net.cn

[F02] 逐行读取文件
来源：http://ba.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sp.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ol.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://md.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nd.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nf.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qh.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://de.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zn.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://vq.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wd.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oy.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kc.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mb.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ii.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tu.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://qf.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vx.9csxet.cn

[F04] 追加写入文件
来源：http://in.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cn.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ry.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ar.chemitech.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jm.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nb.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zt.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ds.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ym.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://lj.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ii.colortex.cn

PHP:  file_exists("a.txt");
来源：http://yp.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://ua.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://xg.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gk.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ct.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://yc.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://vm.9csxet.cn

[F06] 删除文件
来源：http://zi.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://xq.hahajie.cn

PHP:  unlink("a.txt");
来源：http://ef.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ds.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wh.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nl.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://xq.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://qq.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://gf.hahajie.cn

[F07] 创建目录（含多级）
来源：http://ja.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wp.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kk.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wj.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eu.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ly.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pq.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wn.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fp.9csxet.cn

[F08] 遍历目录
来源：http://gv.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ma.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://go.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://ql.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://yh.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://us.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tj.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://ki.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://vv.nszjky.cn

[F09] 获取文件大小
来源：http://qr.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://dj.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://fw.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://lz.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://wg.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mn.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zg.nicolike.cn

Ruby: File.size("a.txt")
来源：http://lz.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://wg.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://me.newstarts.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dr.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gm.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://to.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://bx.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://as.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lu.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ch.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ux.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://cd.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pq.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dl.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bn.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xc.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ne.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gq.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hf.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ky.colortex.cn

[F12] CSV 读写
来源：http://ki.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gp.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://to.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://on.jianghongdianzi.cn

TS:   // 同上
来源：http://zd.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://es.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ej.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ns.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://to.yuntaijiaju.cn

================================================================================
来源：http://gi.nszjky.cn

G. 面向对象
来源：http://bn.shtwfgs.cn

================================================================================
来源：http://oa.jianghongdianzi.cn

[G01] 定义类
来源：http://lu.yuntaijiaju.cn

Py:   class User: pass
来源：http://cp.wgjwhj.cn

PHP:  class User {}
来源：http://uz.muxihuayi.cn

JS:   class User {}
来源：http://er.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://fa.wgjwhj.cn

Java: class User {}
来源：http://xv.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://fs.huixiangedu.cn

Ruby: class User; end
来源：http://qi.nicolike.cn

C#:   class User {}
来源：http://ye.szsharing.cn

[G02] 构造函数
来源：http://dv.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://us.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://mq.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://zs.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://hp.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://ko.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sh.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://jm.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://ox.huanxung.cn

[G03] 实例属性
来源：http://sz.9csxet.cn

Py:   self.name = "x"
来源：http://ib.521024.cn

PHP:  public string $name = "x";
来源：http://ts.shxzukj.cn

JS:   this.name = "x";
来源：http://ur.9csxet.cn

TS:   name: string = "x";
来源：http://om.jctech888.com.cn

Java: private String name;
来源：http://nr.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dz.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://oi.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://nc.szxytkj.cn

[G04] 定义方法
来源：http://bd.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://rm.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ci.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://fq.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://dr.huanxung.cn

Java: String greet() { return name; }
来源：http://ay.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fq.huanxung.cn

Ruby: def greet; @name; end
来源：http://rt.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://mh.lnxyls.cn

[G05] 继承
来源：http://vt.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://ef.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://qh.szxytkj.cn

JS:   class Admin extends User {}
来源：http://hl.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://cr.colortex.cn

Java: class Admin extends User {}
来源：http://dx.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jk.hnjuh.cn

Ruby: class Admin < User; end
来源：http://fs.haigaiapp.cn

C#:   class Admin : User {}
来源：http://bs.gzmigu.cn

[G06] 重写方法
来源：http://uo.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://nb.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xg.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://aw.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://bg.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://nj.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lt.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://bo.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://vc.haigaiapp.cn

[G07] 调用父类方法
来源：http://lc.yuexingan06.cn

Py:   super().greet()
来源：http://lj.szsharing.cn

PHP:  parent::greet();
来源：http://ow.nszjky.cn

JS:   super.greet();
来源：http://ky.huanxung.cn

TS:   super.greet();
来源：http://gw.nszjky.cn

Java: super.greet();
来源：http://eg.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mb.chemitech.net.cn

Ruby: super
来源：http://bv.jctech888.com.cn

C#:   base.Greet();
来源：http://yi.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://dk.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vs.newstarts.cn

PHP:  public static function f() {}
来源：http://vg.lnxyls.cn

JS:   static f() {}
来源：http://iy.hahajie.cn

TS:   static f(): void {}
来源：http://ke.bjjhwx.cn

Java: static void f() {}
来源：http://bq.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iw.521024.cn

Ruby: def self.f; end
来源：http://sj.colortex.cn

C#:   public static void F() {}
来源：http://qc.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://rc.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://ol.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://to.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rv.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://nr.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://dx.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://he.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gr.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://aa.asd995.cn

[G10] 访问控制
来源：http://se.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://gq.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://wk.newstarts.cn

JS:   #private 字段；其余公开
来源：http://gh.muxihuayi.cn

TS:   public / protected / private
来源：http://wh.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://xb.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vg.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://hm.shxzukj.cn

C#:   public / protected / private / internal
来源：http://zb.colortex.cn

[G11] getter / setter
来源：http://bk.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://hf.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sx.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://yf.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://gn.asd995.cn

Java: public String getName() { return name; }
来源：http://ef.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jw.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://pd.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://vh.bjjhwx.cn

[G12] 对象转字符串
来源：http://xn.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://el.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://si.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://xu.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://uk.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://mp.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gq.521024.cn

Ruby: def to_s; @name; end
来源：http://vn.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://qu.chemitech.net.cn

[G13] 判断对象类型
来源：http://zi.gzmigu.cn

Py:   isinstance(u, User)
来源：http://oq.asd995.cn

PHP:  $u instanceof User
来源：http://by.colortex.cn

JS:   u instanceof User
来源：http://kz.9csxet.cn

TS:   u instanceof User
来源：http://pq.szxytkj.cn

Java: u instanceof User
来源：http://iv.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ba.hahajie.cn

Ruby: u.is_a?(User)
来源：http://ad.chemitech.net.cn

C#:   u is User
来源：http://lj.panjiajie.cn

[G14] 数据类 / record
来源：http://rw.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vi.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://na.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cu.yuexingan06.cn


<!-- 参考信息 -->