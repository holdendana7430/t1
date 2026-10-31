代发 wailian999

[E22] 字节长度与字符长度
来源：http://zs.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xh.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gg.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cw.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fz.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jt.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gp.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://cr.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wx.huixiangedu.cn

================================================================================
来源：http://nw.bjjhwx.cn

F. 文件与目录
来源：http://jp.haigaiapp.cn

================================================================================
来源：http://xy.shxzskj.cn

[F01] 读取整个文件
来源：http://kz.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ru.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://hx.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mn.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vf.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ue.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jg.521024.cn

Ruby: File.read("a.txt")
来源：http://mx.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://pk.jctech888.com.cn

[F02] 逐行读取文件
来源：http://ww.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ta.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ri.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dn.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jy.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vl.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zy.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://of.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nv.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://jb.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://de.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rc.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jd.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fy.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ge.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yz.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://ly.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ig.lnxyls.cn

[F04] 追加写入文件
来源：http://od.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wt.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gu.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xq.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gj.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ni.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dp.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ac.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sz.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://oc.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nt.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://zc.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://ie.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://wa.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dx.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kf.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://ue.asd995.cn

C#:   File.Exists("a.txt")
来源：http://ki.muxihuayi.cn

[F06] 删除文件
来源：http://pi.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://yj.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://xi.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yt.lnxyls.cn

TS:   fs.unlinkSync("a.txt")
来源：http://az.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hb.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://ab.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://ly.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://qf.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://qs.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xx.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nr.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ob.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aj.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://px.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ew.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tc.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eu.szsharing.cn

[F08] 遍历目录
来源：http://sb.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hi.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ek.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://in.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://qz.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mz.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ht.9csxet.cn

Ruby: Dir.children("dir")
来源：http://pg.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://nf.bookmarksfly.cn

[F09] 获取文件大小
来源：http://fn.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://cg.colortex.cn

PHP:  filesize("a.txt");
来源：http://ry.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://nv.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://wl.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iw.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bf.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://yn.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://ha.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://mk.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bp.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iq.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qf.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://zq.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dn.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sv.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sj.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ot.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://lb.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jc.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://te.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://or.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://er.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ae.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vw.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ay.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xe.shxzukj.cn

[F12] CSV 读写
来源：http://qn.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bp.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hx.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zm.hahajie.cn

TS:   // 同上
来源：http://hh.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rx.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vj.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wn.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ad.hnjuh.cn

================================================================================
来源：http://bt.yuexingan06.cn

G. 面向对象
来源：http://dl.huixinmuqiang.cn

================================================================================
来源：http://qj.szsharing.cn

[G01] 定义类
来源：http://tm.colortex.cn

Py:   class User: pass
来源：http://cy.jctech888.com.cn

PHP:  class User {}
来源：http://mh.panjiajie.cn

JS:   class User {}
来源：http://tx.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://au.yuntaijiaju.cn

Java: class User {}
来源：http://la.newstarts.cn

Go:   type User struct { Name string }
来源：http://by.yuntaijiaju.cn

Ruby: class User; end
来源：http://fi.huanxung.cn

C#:   class User {}
来源：http://wx.asd995.cn

[G02] 构造函数
来源：http://jn.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://il.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://ou.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://rt.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://mv.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://yi.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vw.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://ta.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://fl.hahajie.cn

[G03] 实例属性
来源：http://kb.huixiangedu.cn

Py:   self.name = "x"
来源：http://wq.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://ix.wgjwhj.cn

JS:   this.name = "x";
来源：http://so.521024.cn

TS:   name: string = "x";
来源：http://gc.muxihuayi.cn

Java: private String name;
来源：http://mt.shtwfgs.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jw.hahajie.cn

Ruby: @name = "x"
来源：http://lc.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://on.haigaiapp.cn

[G04] 定义方法
来源：http://hp.9csxet.cn

Py:   def greet(self): return self.name
来源：http://ah.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zz.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://eb.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://sz.521024.cn

Java: String greet() { return name; }
来源：http://jb.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zm.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://qf.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://vj.shxzskj.cn

[G05] 继承
来源：http://oj.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://kp.newstarts.cn

PHP:  class Admin extends User {}
来源：http://rm.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://zj.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://gs.hahajie.cn

Java: class Admin extends User {}
来源：http://ki.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yg.hnjuh.cn

Ruby: class Admin < User; end
来源：http://xu.shxzukj.cn

C#:   class Admin : User {}
来源：http://gx.newstarts.cn

[G06] 重写方法
来源：http://zd.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://wb.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://co.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://fj.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://jz.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://hm.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fs.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://mt.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://bw.panjiajie.cn

[G07] 调用父类方法
来源：http://lp.shxzukj.cn

Py:   super().greet()
来源：http://zk.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://xo.szxytkj.cn

JS:   super.greet();
来源：http://ny.yuexingan06.cn

TS:   super.greet();
来源：http://kx.colortex.cn

Java: super.greet();
来源：http://xo.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ds.huanxung.cn

Ruby: super
来源：http://fs.yuntaijiaju.cn

C#:   base.Greet();
来源：http://ad.lnxyls.cn

[G08] 静态方法与属性
来源：http://sc.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bt.yuexingan06.cn

PHP:  public static function f() {}
来源：http://uj.huixiangedu.cn

JS:   static f() {}
来源：http://ta.hnjuh.cn

TS:   static f(): void {}
来源：http://aq.jianghongdianzi.cn

Java: static void f() {}
来源：http://qo.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ya.newstarts.cn

Ruby: def self.f; end
来源：http://vp.panjiajie.cn

C#:   public static void F() {}
来源：http://uv.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://vt.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://vy.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bu.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yt.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://aw.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://rn.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://yp.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ec.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://wm.huixinmuqiang.cn

[G10] 访问控制
来源：http://hk.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://cr.huixiangedu.cn

PHP:  public / protected / private
来源：http://xu.nicolike.cn

JS:   #private 字段；其余公开
来源：http://ec.newstarts.cn

TS:   public / protected / private
来源：http://ch.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://vt.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pq.shxzskj.cn

Ruby: public / protected / private
来源：http://zv.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://ca.szxytkj.cn

[G11] getter / setter
来源：http://dp.newstarts.cn

Py:   @property 与 @x.setter
来源：http://wa.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dc.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://lz.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://jj.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://if.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qk.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://mp.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://cu.lnxyls.cn

[G12] 对象转字符串
来源：http://vi.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://uk.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vx.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://pt.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://ga.521024.cn

Java: @Override public String toString() { return name; }
来源：http://yq.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ma.9csxet.cn

Ruby: def to_s; @name; end
来源：http://wo.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://wj.shxzskj.cn

[G13] 判断对象类型
来源：http://uq.colortex.cn

Py:   isinstance(u, User)
来源：http://yg.bjjhwx.cn

PHP:  $u instanceof User
来源：http://qm.szsharing.cn

JS:   u instanceof User
来源：http://vc.huanxung.cn

TS:   u instanceof User
来源：http://ij.hahajie.cn

Java: u instanceof User
来源：http://ac.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sj.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://tp.521024.cn

C#:   u is User
来源：http://ft.shtwfgs.cn

[G14] 数据类 / record
来源：http://mw.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bp.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://qw.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ri.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://wz.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://iw.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://qp.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hk.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://dv.haigaiapp.cn

[G15] 枚举
来源：http://ll.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sl.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://am.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tw.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rl.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://fv.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dk.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://au.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wz.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://cj.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uk.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://je.nicolike.cn

JS:   Object.entries(obj)
来源：http://wq.9csxet.cn

TS:   Object.entries(obj)
来源：http://qr.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fg.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ki.newstarts.cn

Ruby: obj.instance_variables
来源：http://ym.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://zc.nicolike.cn

================================================================================
来源：http://ke.huixinmuqiang.cn

H. 异常与错误处理
来源：http://tm.bjjhwx.cn

================================================================================
来源：http://pk.wgjwhj.cn

[H01] try / catch 基础
来源：http://if.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gg.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oz.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cq.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jj.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bo.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://an.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sm.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uq.nszjky.cn

[H02] finally / ensure 收尾
来源：http://ap.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mv.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tm.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kp.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ar.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hf.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wz.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nn.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vo.shxzskj.cn

[H03] 主动抛出异常
来源：http://wp.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://mw.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://so.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://fe.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://hn.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nk.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nd.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tx.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uc.9csxet.cn

[H04] 自定义异常类型
来源：http://em.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://tu.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sm.chemitech.net.cn


<!-- 参考信息 -->