代发 wailian999

[E22] 字节长度与字符长度
来源：http://dp.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rs.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ky.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://my.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gc.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iu.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wd.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://vw.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wj.colortex.cn

================================================================================
来源：http://cf.chemitech.net.cn

F. 文件与目录
来源：http://at.szsharing.cn

================================================================================
来源：http://nn.muxihuayi.cn

[F01] 读取整个文件
来源：http://ap.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bl.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://aw.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kf.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zq.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yz.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kg.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://cy.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://uc.hnjuh.cn

[F02] 逐行读取文件
来源：http://ws.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nq.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pp.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ov.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oj.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kn.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xv.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eg.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ef.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://zl.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nt.newstarts.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xa.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jc.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zd.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sc.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jk.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://zd.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yr.hnjuh.cn

[F04] 追加写入文件
来源：http://id.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://id.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zk.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ve.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tr.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yn.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nq.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nl.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vs.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://ru.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://py.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://nz.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://sd.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://au.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mo.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tz.521024.cn

Ruby: File.exist?("a.txt")
来源：http://nb.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://oy.jianghongdianzi.cn

[F06] 删除文件
来源：http://ct.huanxung.cn

Py:   os.remove("a.txt")
来源：http://rt.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://sy.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://iw.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bp.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wd.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://hh.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://ii.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://ph.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://al.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fo.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ep.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ka.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dc.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tq.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ea.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ao.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ow.shxzskj.cn

[F08] 遍历目录
来源：http://zk.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kx.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kt.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://ph.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://rm.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bl.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ha.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://pl.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://eu.newstarts.cn

[F09] 获取文件大小
来源：http://wo.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://fg.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://ov.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://hf.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://dc.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fo.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bf.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://vd.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://yl.gzmigu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ba.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hx.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xp.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xp.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://tk.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ic.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oj.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wq.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cq.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://hx.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dz.muxihuayi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bn.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nb.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zd.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qp.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ev.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lx.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ve.panjiajie.cn

[F12] CSV 读写
来源：http://hn.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ai.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xf.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://na.yuexingan06.cn

TS:   // 同上
来源：http://fs.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wq.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gj.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yh.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gc.yuexingan06.cn

================================================================================
来源：http://lj.shxzukj.cn

G. 面向对象
来源：http://wq.bookmarksfly.cn

================================================================================
来源：http://rn.huanxung.cn

[G01] 定义类
来源：http://ps.shxzukj.cn

Py:   class User: pass
来源：http://we.huixinmuqiang.cn

PHP:  class User {}
来源：http://hz.szsharing.cn

JS:   class User {}
来源：http://ui.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://vf.jianghongdianzi.cn

Java: class User {}
来源：http://qm.newstarts.cn

Go:   type User struct { Name string }
来源：http://gx.nszjky.cn

Ruby: class User; end
来源：http://oj.colortex.cn

C#:   class User {}
来源：http://gu.lnxyls.cn

[G02] 构造函数
来源：http://oe.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://wu.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://ab.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://dq.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://vx.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://bw.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fc.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://vf.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://no.huanxung.cn

[G03] 实例属性
来源：http://fq.hnjuh.cn

Py:   self.name = "x"
来源：http://mi.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://ij.nszjky.cn

JS:   this.name = "x";
来源：http://nw.hahajie.cn

TS:   name: string = "x";
来源：http://nx.nicolike.cn

Java: private String name;
来源：http://uo.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tj.huanxung.cn

Ruby: @name = "x"
来源：http://xu.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://dg.yuexingan06.cn

[G04] 定义方法
来源：http://ny.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://pi.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wn.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://bo.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://kq.muxihuayi.cn

Java: String greet() { return name; }
来源：http://kf.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://me.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://dy.colortex.cn

C#:   public string Greet() => Name;
来源：http://ye.nszjky.cn

[G05] 继承
来源：http://eh.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://un.9csxet.cn

PHP:  class Admin extends User {}
来源：http://ej.521024.cn

JS:   class Admin extends User {}
来源：http://ut.nicolike.cn

TS:   class Admin extends User {}
来源：http://vs.colortex.cn

Java: class Admin extends User {}
来源：http://ws.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hq.asd995.cn

Ruby: class Admin < User; end
来源：http://gb.wgjwhj.cn

C#:   class Admin : User {}
来源：http://tc.huixiangedu.cn

[G06] 重写方法
来源：http://wb.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://ht.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ul.asd995.cn

JS:   greet() { return "admin"; }
来源：http://ub.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://uy.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://tv.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rs.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://qr.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://ec.shtwfgs.cn

[G07] 调用父类方法
来源：http://hx.haigaiapp.cn

Py:   super().greet()
来源：http://qx.jctech888.com.cn

PHP:  parent::greet();
来源：http://en.jianghongdianzi.cn

JS:   super.greet();
来源：http://vs.yuntaijiaju.cn

TS:   super.greet();
来源：http://ui.nszjky.cn

Java: super.greet();
来源：http://wa.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ea.gzmigu.cn

Ruby: super
来源：http://dg.huanxung.cn

C#:   base.Greet();
来源：http://nc.wgjwhj.cn

[G08] 静态方法与属性
来源：http://zk.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ye.colortex.cn

PHP:  public static function f() {}
来源：http://rt.hahajie.cn

JS:   static f() {}
来源：http://zd.hnjuh.cn

TS:   static f(): void {}
来源：http://ha.nszjky.cn

Java: static void f() {}
来源：http://kl.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ey.szxytkj.cn

Ruby: def self.f; end
来源：http://mm.nicolike.cn

C#:   public static void F() {}
来源：http://oc.hahajie.cn

[G09] 接口 / 抽象类
来源：http://xs.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://gd.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rg.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vz.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://jv.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://qu.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://en.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cx.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://up.lnxyls.cn

[G10] 访问控制
来源：http://qw.muxihuayi.cn

Py:   约定 _protected / __private（不强制）
来源：http://up.nicolike.cn

PHP:  public / protected / private
来源：http://em.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://dl.huanxung.cn

TS:   public / protected / private
来源：http://om.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://vp.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mc.szsharing.cn

Ruby: public / protected / private
来源：http://mj.gzmigu.cn

C#:   public / protected / private / internal
来源：http://wj.newstarts.cn

[G11] getter / setter
来源：http://qy.huanxung.cn

Py:   @property 与 @x.setter
来源：http://bi.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ab.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://di.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://jy.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://sq.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sa.colortex.cn

Ruby: attr_accessor :name
来源：http://at.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://in.lnxyls.cn

[G12] 对象转字符串
来源：http://rm.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://si.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eo.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://tk.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://ev.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://ow.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hu.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://pl.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://od.shxzukj.cn

[G13] 判断对象类型
来源：http://be.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://tc.shxzskj.cn

PHP:  $u instanceof User
来源：http://ej.huanxung.cn

JS:   u instanceof User
来源：http://mn.shxzukj.cn

TS:   u instanceof User
来源：http://qy.chemitech.net.cn

Java: u instanceof User
来源：http://bx.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ws.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://fe.asd995.cn

C#:   u is User
来源：http://iu.muxihuayi.cn

[G14] 数据类 / record
来源：http://xa.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ik.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://xn.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://do.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://di.asd995.cn

Java: record User(String name, int age) {}
来源：http://hd.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://ba.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qg.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://gn.gzmigu.cn

[G15] 枚举
来源：http://oi.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rn.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cj.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pw.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bl.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://zk.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sa.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://tx.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ci.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://xb.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://we.colortex.cn

PHP:  get_object_vars($obj);
来源：http://cs.szsharing.cn

JS:   Object.entries(obj)
来源：http://ia.nszjky.cn

TS:   Object.entries(obj)
来源：http://jw.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ik.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pa.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://yl.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://uc.huixinmuqiang.cn

================================================================================
来源：http://eg.nicolike.cn

H. 异常与错误处理
来源：http://cx.huanxung.cn

================================================================================
来源：http://nc.shtwfgs.cn

[H01] try / catch 基础
来源：http://kq.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nh.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fu.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iu.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xf.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fd.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mo.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ly.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oi.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://in.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uw.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vy.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zx.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gr.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kf.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dc.yuntaijiaju.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fe.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ap.gzmigu.cn

[H03] 主动抛出异常
来源：http://qh.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://bi.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qn.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://zg.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://xk.yuexingan06.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ow.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pn.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mq.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wk.huixiangedu.cn

[H04] 自定义异常类型
来源：http://zl.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://yv.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pv.muxihuayi.cn


<!-- 参考信息 -->