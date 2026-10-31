代发 wailian999

[E22] 字节长度与字符长度
来源：http://ce.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xe.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://io.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://by.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qz.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cu.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ek.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://mz.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jz.yuexingan06.cn

================================================================================
来源：http://xd.gzmigu.cn

F. 文件与目录
来源：http://mt.newstarts.cn

================================================================================
来源：http://ys.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://ik.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hy.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://ie.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xv.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gy.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ku.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zt.9csxet.cn

Ruby: File.read("a.txt")
来源：http://rl.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://ue.jctech888.com.cn

[F02] 逐行读取文件
来源：http://ml.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ha.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wt.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xm.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ta.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xz.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pe.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://en.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://su.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://bt.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://il.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nu.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jy.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qp.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ee.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vr.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://fc.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ms.huixiangedu.cn

[F04] 追加写入文件
来源：http://uk.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qz.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tu.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tc.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fq.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lq.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mp.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tf.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tw.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://bl.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ch.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://lm.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://ke.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://lo.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gu.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://km.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://ci.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://jn.szsharing.cn

[F06] 删除文件
来源：http://py.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://tk.hahajie.cn

PHP:  unlink("a.txt");
来源：http://er.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qz.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://av.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ix.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://nt.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://hv.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://kh.szsharing.cn

[F07] 创建目录（含多级）
来源：http://qd.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ji.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rj.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ht.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uy.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://su.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hn.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://si.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zw.haigaiapp.cn

[F08] 遍历目录
来源：http://cc.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://od.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fw.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://ac.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://fc.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lb.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cj.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://ml.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://bg.521024.cn

[F09] 获取文件大小
来源：http://fd.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://ms.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://fn.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://hg.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://ki.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://va.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ar.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://ik.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://wj.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://dy.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qw.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dy.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fb.asd995.cn

TS:   path.extname("a.txt")
来源：http://sz.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uq.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hs.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zc.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jg.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://ah.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ee.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cg.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kd.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jr.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://se.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sy.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iw.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nz.colortex.cn

[F12] CSV 读写
来源：http://jz.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tg.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yf.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ok.nszjky.cn

TS:   // 同上
来源：http://ie.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bd.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kb.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dc.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jk.szxytkj.cn

================================================================================
来源：http://yf.huanxung.cn

G. 面向对象
来源：http://gs.huixinmuqiang.cn

================================================================================
来源：http://ik.shxzskj.cn

[G01] 定义类
来源：http://tl.gzmigu.cn

Py:   class User: pass
来源：http://xc.muxihuayi.cn

PHP:  class User {}
来源：http://ti.lnxyls.cn

JS:   class User {}
来源：http://eg.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://vg.9csxet.cn

Java: class User {}
来源：http://ho.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://ec.huixiangedu.cn

Ruby: class User; end
来源：http://fu.colortex.cn

C#:   class User {}
来源：http://gf.huixiangedu.cn

[G02] 构造函数
来源：http://vw.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://pm.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://cp.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://qi.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://uc.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://kh.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wd.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://hy.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://dh.nszjky.cn

[G03] 实例属性
来源：http://aa.huixiangedu.cn

Py:   self.name = "x"
来源：http://yl.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://kd.huanxung.cn

JS:   this.name = "x";
来源：http://rj.muxihuayi.cn

TS:   name: string = "x";
来源：http://si.gzmigu.cn

Java: private String name;
来源：http://yl.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ov.521024.cn

Ruby: @name = "x"
来源：http://us.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://zc.huixiangedu.cn

[G04] 定义方法
来源：http://yn.szsharing.cn

Py:   def greet(self): return self.name
来源：http://aw.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sq.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://ob.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://qj.colortex.cn

Java: String greet() { return name; }
来源：http://mc.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qj.asd995.cn

Ruby: def greet; @name; end
来源：http://cj.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://pg.yuntaijiaju.cn

[G05] 继承
来源：http://fv.shxzukj.cn

Py:   class Admin(User): pass
来源：http://wz.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://li.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://te.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://zq.jctech888.com.cn

Java: class Admin extends User {}
来源：http://jg.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lc.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://uj.panjiajie.cn

C#:   class Admin : User {}
来源：http://en.hnjuh.cn

[G06] 重写方法
来源：http://nz.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://ji.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hl.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://ps.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://ca.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://yc.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kd.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://sv.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://xw.haigaiapp.cn

[G07] 调用父类方法
来源：http://av.shtwfgs.cn

Py:   super().greet()
来源：http://ac.szxytkj.cn

PHP:  parent::greet();
来源：http://qy.szsharing.cn

JS:   super.greet();
来源：http://zg.chemitech.net.cn

TS:   super.greet();
来源：http://na.nszjky.cn

Java: super.greet();
来源：http://gn.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hs.nicolike.cn

Ruby: super
来源：http://ti.lnxyls.cn

C#:   base.Greet();
来源：http://vw.shxzskj.cn

[G08] 静态方法与属性
来源：http://wq.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yo.wgjwhj.cn

PHP:  public static function f() {}
来源：http://md.jctech888.com.cn

JS:   static f() {}
来源：http://gz.colortex.cn

TS:   static f(): void {}
来源：http://in.huanxung.cn

Java: static void f() {}
来源：http://ik.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eh.nszjky.cn

Ruby: def self.f; end
来源：http://pz.bjjhwx.cn

C#:   public static void F() {}
来源：http://lz.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://im.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://uo.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zz.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bf.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://fh.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://jg.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://km.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qh.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://sy.9csxet.cn

[G10] 访问控制
来源：http://hw.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://pq.jctech888.com.cn

PHP:  public / protected / private
来源：http://tw.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://os.shtwfgs.cn

TS:   public / protected / private
来源：http://le.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://hp.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xp.panjiajie.cn

Ruby: public / protected / private
来源：http://ik.9csxet.cn

C#:   public / protected / private / internal
来源：http://dn.szsharing.cn

[G11] getter / setter
来源：http://ej.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://ay.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pn.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://id.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://sh.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://fq.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ac.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://zd.9csxet.cn

C#:   public string Name { get; set; }
来源：http://lp.bookmarksfly.cn

[G12] 对象转字符串
来源：http://hk.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://ok.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ap.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://dv.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://dk.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://yy.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://md.nicolike.cn

Ruby: def to_s; @name; end
来源：http://cl.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://ji.521024.cn

[G13] 判断对象类型
来源：http://wd.gzmigu.cn

Py:   isinstance(u, User)
来源：http://jm.yuexingan06.cn

PHP:  $u instanceof User
来源：http://on.bookmarksfly.cn

JS:   u instanceof User
来源：http://uj.huixiangedu.cn

TS:   u instanceof User
来源：http://an.huixinmuqiang.cn

Java: u instanceof User
来源：http://gg.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xo.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://rv.wgjwhj.cn

C#:   u is User
来源：http://zi.newstarts.cn

[G14] 数据类 / record
来源：http://sz.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gf.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://sp.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fk.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://sk.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://eu.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://ke.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jx.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://gw.newstarts.cn

[G15] 枚举
来源：http://tw.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hr.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://db.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ph.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://se.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://ku.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oq.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://jc.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sk.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://ff.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fy.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://tm.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://gi.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://fg.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tt.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bz.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://mn.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://ul.bjjhwx.cn

================================================================================
来源：http://xg.gzmigu.cn

H. 异常与错误处理
来源：http://vb.wgjwhj.cn

================================================================================
来源：http://ir.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://kx.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://st.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ru.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://um.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pn.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mj.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cb.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://an.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ee.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://df.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gl.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zg.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sa.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xz.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zt.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yd.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gp.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gz.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://si.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://ri.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xn.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://zs.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://or.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zr.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hd.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vp.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cz.nszjky.cn

[H04] 自定义异常类型
来源：http://we.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://dh.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jc.shxzukj.cn


<!-- 参考信息 -->