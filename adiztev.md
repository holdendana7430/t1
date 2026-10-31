代发 wailian999

Go:   if s == "" {}
来源：http://ae.wgjwhj.cn

Ruby: if s.empty?
来源：http://zp.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uq.lnxyls.cn

[E21] 超长截断加省略号
来源：http://ai.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qc.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fb.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lt.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rw.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ew.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://jl.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rn.nszjky.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qr.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://de.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bk.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xn.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qq.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://py.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mi.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qd.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://cf.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mw.huanxung.cn

================================================================================
来源：http://qp.asd995.cn

F. 文件与目录
来源：http://td.chemitech.net.cn

================================================================================
来源：http://et.wgjwhj.cn

[F01] 读取整个文件
来源：http://qu.huixiangedu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xx.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://tz.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tc.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gw.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rv.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fe.nszjky.cn

Ruby: File.read("a.txt")
来源：http://cf.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ht.shxzskj.cn

[F02] 逐行读取文件
来源：http://mb.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vb.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://op.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://te.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pw.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yp.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zf.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qb.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ze.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://hg.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lr.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mn.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qq.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zn.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wc.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rm.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://cw.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ct.gzmigu.cn

[F04] 追加写入文件
来源：http://ub.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ed.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hp.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mk.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ok.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xk.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oh.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ck.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gz.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://kh.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sc.colortex.cn

PHP:  file_exists("a.txt");
来源：http://wg.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://ht.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://zu.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vy.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bc.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://lw.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://rt.colortex.cn

[F06] 删除文件
来源：http://rz.9csxet.cn

Py:   os.remove("a.txt")
来源：http://bb.521024.cn

PHP:  unlink("a.txt");
来源：http://hb.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ho.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ay.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kn.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://ap.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://wt.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://ha.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://cb.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mo.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iu.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://on.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xa.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wv.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jt.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://re.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tt.yuexingan06.cn

[F08] 遍历目录
来源：http://gk.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zx.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fu.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://yf.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://gw.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zp.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xm.9csxet.cn

Ruby: Dir.children("dir")
来源：http://cr.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://ac.hahajie.cn

[F09] 获取文件大小
来源：http://pi.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://qt.9csxet.cn

PHP:  filesize("a.txt");
来源：http://uh.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://yf.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://ua.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bf.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nf.huanxung.cn

Ruby: File.size("a.txt")
来源：http://vj.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://ex.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://ut.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ux.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bl.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tf.szsharing.cn

TS:   path.extname("a.txt")
来源：http://ee.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bz.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kn.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ht.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ak.521024.cn

[F11] 复制与移动文件
来源：http://xj.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dc.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rm.huixinmuqiang.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fd.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xb.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vu.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rj.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cv.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://if.521024.cn

[F12] CSV 读写
来源：http://io.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fq.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tc.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ne.shxzukj.cn

TS:   // 同上
来源：http://tq.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iq.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xt.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tb.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ie.haigaiapp.cn

================================================================================
来源：http://et.gzmigu.cn

G. 面向对象
来源：http://jc.huixinmuqiang.cn

================================================================================
来源：http://lj.nicolike.cn

[G01] 定义类
来源：http://ny.hnjuh.cn

Py:   class User: pass
来源：http://gx.szxytkj.cn

PHP:  class User {}
来源：http://lq.shxzukj.cn

JS:   class User {}
来源：http://xb.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://mv.bjjhwx.cn

Java: class User {}
来源：http://ar.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://nu.wgjwhj.cn

Ruby: class User; end
来源：http://sf.chemitech.net.cn

C#:   class User {}
来源：http://ba.shxzukj.cn

[G02] 构造函数
来源：http://qd.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://lp.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://hl.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://sx.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://cr.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://lz.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kz.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://pa.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://ng.huixinmuqiang.cn

[G03] 实例属性
来源：http://jv.colortex.cn

Py:   self.name = "x"
来源：http://ti.521024.cn

PHP:  public string $name = "x";
来源：http://jm.nicolike.cn

JS:   this.name = "x";
来源：http://da.bjjhwx.cn

TS:   name: string = "x";
来源：http://it.nszjky.cn

Java: private String name;
来源：http://bb.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fo.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://mw.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://mq.szsharing.cn

[G04] 定义方法
来源：http://ya.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://kx.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tp.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://af.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://ht.9csxet.cn

Java: String greet() { return name; }
来源：http://xm.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dz.hahajie.cn

Ruby: def greet; @name; end
来源：http://za.huanxung.cn

C#:   public string Greet() => Name;
来源：http://zb.chemitech.net.cn

[G05] 继承
来源：http://cq.colortex.cn

Py:   class Admin(User): pass
来源：http://ro.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://nb.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://fq.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://mz.nicolike.cn

Java: class Admin extends User {}
来源：http://cl.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mc.shxzskj.cn

Ruby: class Admin < User; end
来源：http://xo.lnxyls.cn

C#:   class Admin : User {}
来源：http://nz.jctech888.com.cn

[G06] 重写方法
来源：http://ka.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://wj.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qn.colortex.cn

JS:   greet() { return "admin"; }
来源：http://pz.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://kn.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://tz.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zm.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://sb.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://qu.hahajie.cn

[G07] 调用父类方法
来源：http://wd.shxzskj.cn

Py:   super().greet()
来源：http://id.wgjwhj.cn

PHP:  parent::greet();
来源：http://mp.hahajie.cn

JS:   super.greet();
来源：http://wc.colortex.cn

TS:   super.greet();
来源：http://be.jctech888.com.cn

Java: super.greet();
来源：http://jv.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ut.jianghongdianzi.cn

Ruby: super
来源：http://xy.szsharing.cn

C#:   base.Greet();
来源：http://ov.shxzukj.cn

[G08] 静态方法与属性
来源：http://ei.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ep.jctech888.com.cn

PHP:  public static function f() {}
来源：http://nk.shxzskj.cn

JS:   static f() {}
来源：http://yp.wgjwhj.cn

TS:   static f(): void {}
来源：http://dt.wgjwhj.cn

Java: static void f() {}
来源：http://id.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jm.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://dv.yuexingan06.cn

C#:   public static void F() {}
来源：http://en.nszjky.cn

[G09] 接口 / 抽象类
来源：http://ss.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://ru.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gd.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://re.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://na.521024.cn

Java: interface Shape { double area(); }
来源：http://jm.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://iz.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ut.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://no.hnjuh.cn

[G10] 访问控制
来源：http://rf.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://ar.bjjhwx.cn

PHP:  public / protected / private
来源：http://xl.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://wh.jctech888.com.cn

TS:   public / protected / private
来源：http://ov.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://sh.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fe.haigaiapp.cn

Ruby: public / protected / private
来源：http://bu.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://of.hahajie.cn

[G11] getter / setter
来源：http://zu.hahajie.cn

Py:   @property 与 @x.setter
来源：http://nh.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hp.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://dr.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://su.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://nf.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tw.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://he.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://zk.wgjwhj.cn

[G12] 对象转字符串
来源：http://wk.521024.cn

Py:   def __str__(self): return self.name
来源：http://gw.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cz.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://pl.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://kw.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://qt.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ty.asd995.cn

Ruby: def to_s; @name; end
来源：http://zw.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://pi.chemitech.net.cn

[G13] 判断对象类型
来源：http://vp.colortex.cn

Py:   isinstance(u, User)
来源：http://do.521024.cn

PHP:  $u instanceof User
来源：http://gl.hnjuh.cn

JS:   u instanceof User
来源：http://nx.huixinmuqiang.cn

TS:   u instanceof User
来源：http://bd.shxzskj.cn

Java: u instanceof User
来源：http://qh.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://be.colortex.cn

Ruby: u.is_a?(User)
来源：http://rm.nicolike.cn

C#:   u is User
来源：http://bn.colortex.cn

[G14] 数据类 / record
来源：http://wk.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://in.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://mm.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tk.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://nx.nicolike.cn

Java: record User(String name, int age) {}
来源：http://zb.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://lc.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yn.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://lf.huanxung.cn

[G15] 枚举
来源：http://ur.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fn.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ol.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hq.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yz.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://mn.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rx.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://im.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nx.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://md.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://by.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://ji.hnjuh.cn

JS:   Object.entries(obj)
来源：http://ee.colortex.cn

TS:   Object.entries(obj)
来源：http://fx.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bx.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ur.9csxet.cn

Ruby: obj.instance_variables
来源：http://kr.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://jy.jianghongdianzi.cn

================================================================================
来源：http://nz.huanxung.cn

H. 异常与错误处理
来源：http://fd.bookmarksfly.cn

================================================================================
来源：http://vh.nszjky.cn

[H01] try / catch 基础
来源：http://ic.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://un.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fu.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://us.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vz.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xk.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wo.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iw.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oy.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://uo.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ey.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xo.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rw.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fv.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jl.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ua.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sy.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xj.shxzukj.cn


<!-- 参考信息 -->