代发 wailian999

PHP:  number_format(1234567);
来源：http://yx.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vo.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yx.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gc.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tx.jianghongdianzi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uy.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://lc.9csxet.cn

[E17] 首字母大写
来源：http://qw.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lk.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fn.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wu.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vc.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ee.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bz.shxzskj.cn

Ruby: s.capitalize
来源：http://st.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nl.yuexingan06.cn

[E18] 模板占位符替换
来源：http://nk.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fr.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sj.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dn.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cf.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xs.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ad.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hc.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ym.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://pe.colortex.cn

Py:   s.splitlines()
来源：http://na.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mt.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://cq.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://jb.shxzukj.cn

Java: s.lines().toList()
来源：http://wy.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://bt.lnxyls.cn

Ruby: s.lines
来源：http://ma.huanxung.cn

C#:   s.Split('\n')
来源：http://oj.nicolike.cn

[E20] 判断字符串是否为空
来源：http://mg.9csxet.cn

Py:   if not s:
来源：http://ul.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tw.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xn.nicolike.cn

TS:   if (s === "") {}
来源：http://nn.szxytkj.cn

Java: if (s.isEmpty()) {}
来源：http://mw.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://ki.jctech888.com.cn

Ruby: if s.empty?
来源：http://wl.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rd.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://bo.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fq.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nn.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fh.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://na.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cy.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://gu.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eh.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dg.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://mm.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vg.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gf.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hx.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cl.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ze.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qu.9csxet.cn

Ruby: s.bytesize;  s.length
来源：http://tl.panjiajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ti.yuntaijiaju.cn

================================================================================
来源：http://ir.huixinmuqiang.cn

F. 文件与目录
来源：http://bh.asd995.cn

================================================================================
来源：http://wp.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://gi.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tw.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://qx.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://en.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://it.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ix.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xw.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://td.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ys.9csxet.cn

[F02] 逐行读取文件
来源：http://vl.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://js.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ow.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kd.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tw.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uy.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hu.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iy.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jb.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://ut.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lc.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nf.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xb.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lo.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zg.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gw.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://gk.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pe.hahajie.cn

[F04] 追加写入文件
来源：http://yc.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pl.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jg.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xa.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bo.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lj.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://du.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nl.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ku.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://kc.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ld.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://aq.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://ty.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://nf.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gp.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vl.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://ot.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://mj.nicolike.cn

[F06] 删除文件
来源：http://uq.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://hp.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://bo.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tz.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ri.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ew.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://wa.colortex.cn

Ruby: File.delete("a.txt")
来源：http://nm.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://cp.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://cv.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kc.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nq.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kv.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zb.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ud.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oe.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://km.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kz.szsharing.cn

[F08] 遍历目录
来源：http://sp.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ar.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hh.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://dc.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://gp.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sm.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ge.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://xg.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://bj.gzmigu.cn

[F09] 获取文件大小
来源：http://oh.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://nt.newstarts.cn

PHP:  filesize("a.txt");
来源：http://fo.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://lv.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://ly.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://el.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mp.newstarts.cn

Ruby: File.size("a.txt")
来源：http://ss.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://mt.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://uk.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vx.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ja.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vl.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://ic.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ns.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wt.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tq.panjiajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fa.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://fl.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nh.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fc.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mp.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zz.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fs.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ty.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uc.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://su.jianghongdianzi.cn

[F12] CSV 读写
来源：http://cf.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kj.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bd.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mg.jctech888.com.cn

TS:   // 同上
来源：http://jg.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fx.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fc.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ls.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://na.nicolike.cn

================================================================================
来源：http://cc.huanxung.cn

G. 面向对象
来源：http://xj.nicolike.cn

================================================================================
来源：http://zt.huixinmuqiang.cn

[G01] 定义类
来源：http://tg.shxzukj.cn

Py:   class User: pass
来源：http://da.9csxet.cn

PHP:  class User {}
来源：http://zh.bjjhwx.cn

JS:   class User {}
来源：http://zl.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://uh.szxytkj.cn

Java: class User {}
来源：http://wm.hahajie.cn

Go:   type User struct { Name string }
来源：http://tk.muxihuayi.cn

Ruby: class User; end
来源：http://jw.lnxyls.cn

C#:   class User {}
来源：http://vi.panjiajie.cn

[G02] 构造函数
来源：http://ye.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://in.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://sx.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ng.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://vp.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://hs.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bp.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://bm.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://ur.gzmigu.cn

[G03] 实例属性
来源：http://xm.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://bq.nicolike.cn

PHP:  public string $name = "x";
来源：http://nz.nszjky.cn

JS:   this.name = "x";
来源：http://ax.bookmarksfly.cn

TS:   name: string = "x";
来源：http://nm.muxihuayi.cn

Java: private String name;
来源：http://ry.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zb.lnxyls.cn

Ruby: @name = "x"
来源：http://mi.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://me.lnxyls.cn

[G04] 定义方法
来源：http://oz.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://wn.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jn.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://hs.nszjky.cn

TS:   greet(): string { return this.name; }
来源：http://xz.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://vj.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zm.hahajie.cn

Ruby: def greet; @name; end
来源：http://tc.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://xx.colortex.cn

[G05] 继承
来源：http://zo.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://uo.hahajie.cn

PHP:  class Admin extends User {}
来源：http://ro.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://pk.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://by.shxzukj.cn

Java: class Admin extends User {}
来源：http://rf.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ao.521024.cn

Ruby: class Admin < User; end
来源：http://po.colortex.cn

C#:   class Admin : User {}
来源：http://uw.hahajie.cn

[G06] 重写方法
来源：http://oa.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://dx.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bn.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://xo.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://ju.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://ox.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qf.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://he.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://te.szxytkj.cn

[G07] 调用父类方法
来源：http://mr.szsharing.cn

Py:   super().greet()
来源：http://wu.shtwfgs.cn

PHP:  parent::greet();
来源：http://xj.shxzskj.cn

JS:   super.greet();
来源：http://wj.hnjuh.cn

TS:   super.greet();
来源：http://dd.shxzukj.cn

Java: super.greet();
来源：http://bj.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mh.szsharing.cn

Ruby: super
来源：http://za.hahajie.cn

C#:   base.Greet();
来源：http://sh.szxytkj.cn

[G08] 静态方法与属性
来源：http://xh.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://up.hahajie.cn

PHP:  public static function f() {}
来源：http://da.shxzskj.cn

JS:   static f() {}
来源：http://aa.bjjhwx.cn

TS:   static f(): void {}
来源：http://ed.chemitech.net.cn

Java: static void f() {}
来源：http://cc.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ln.yuexingan06.cn

Ruby: def self.f; end
来源：http://mw.hahajie.cn

C#:   public static void F() {}
来源：http://pv.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://qz.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://ic.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mm.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dc.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://ir.szsharing.cn

Java: interface Shape { double area(); }
来源：http://mo.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://hk.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wl.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://pr.haigaiapp.cn

[G10] 访问控制
来源：http://uz.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://rp.nszjky.cn

PHP:  public / protected / private
来源：http://lb.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://zy.huanxung.cn

TS:   public / protected / private
来源：http://zt.colortex.cn

Java: public / protected / private / 默认包级
来源：http://am.asd995.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ce.panjiajie.cn

Ruby: public / protected / private
来源：http://ke.nicolike.cn

C#:   public / protected / private / internal
来源：http://rz.yuntaijiaju.cn

[G11] getter / setter
来源：http://ui.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://ke.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kw.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://zc.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://ux.newstarts.cn

Java: public String getName() { return name; }
来源：http://ja.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vq.asd995.cn

Ruby: attr_accessor :name
来源：http://pc.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://zx.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://ze.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://eb.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ie.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://pd.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://ip.521024.cn

Java: @Override public String toString() { return name; }
来源：http://di.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ba.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://pg.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://yh.huanxung.cn

[G13] 判断对象类型
来源：http://ni.panjiajie.cn

Py:   isinstance(u, User)
来源：http://ty.nszjky.cn

PHP:  $u instanceof User
来源：http://ai.huanxung.cn

JS:   u instanceof User
来源：http://la.haigaiapp.cn

TS:   u instanceof User
来源：http://pa.gzmigu.cn

Java: u instanceof User
来源：http://js.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pt.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://av.asd995.cn

C#:   u is User
来源：http://zz.lnxyls.cn

[G14] 数据类 / record
来源：http://xr.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eh.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://wk.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yt.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://it.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://mu.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://zt.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gv.bjjhwx.cn


<!-- 参考信息 -->