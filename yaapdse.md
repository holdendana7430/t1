代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gvauutlqx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gpegwpwmv.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gaveeqjbc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gqymwbmwj.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gopzsxbrm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkvnwmtme.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gpntdxznp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gfsdqhqdx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gnetmxdwf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gfvzugyux.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/goyffjvuw.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnmsknqej.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gmmdhzhxr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gjgsvuwza.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/guonjwvpc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbzmfhlwg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gojatvsup.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gezpyrkkx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gahrojmiq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gahrbmebj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqlarjcwr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghsrhqyxj.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gddbaokoi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmqzmphjn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gkjoebyyk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gazueiabp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glftzudsf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gadcwnzsh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/grpgkmidj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxibipblo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/goxuhjfxa.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gqsdjbpwc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gdffsmdby.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gfnnufhyd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gxnwjkuhp.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gjjxyxoxa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gsuzvbvti.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gbvfpwydk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gjdfdmjhv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gusbrlmfi.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gudazhyjb.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gfndqyufz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyeijgghn.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gepjhctgb.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gcsyqtphs.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/glhqzbgkd.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdwleswhk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwfazjut.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gaxhvtzde.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gasktidto.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gqmwotaui.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/goczoqxeh.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gdrjquvaz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gcswhvunb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gnfapbfyr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/glxtafctp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/geoskmpdr.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gvwomnfxd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/ggzioiyvz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gtgmpbqjv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gmrmuqbws.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gkaajkbhf.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gvtqlzxer.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gboitxsbj.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gxjpnwdgn.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gmsoebolm.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gnogmvwek.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gaccyzolf.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/glyqxucgv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gwuoztwgj.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gcffpsieu.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gqaeiwvcs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gubqbvyig.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gberbxzyw.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gftasuwfr.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gaizdkode.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gegihbsif.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gsgqcesjr.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gflspoiwj.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/grrsjnncd.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gjimidxem.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ggpoktvpz.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gcswjtttp.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gkxueuhyl.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/geyoxgwxi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gebytplgh.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/grnmjcogy.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gebjtxwrb.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gerzuhbdh.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gxcnuzavk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/guqlwjxqf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjzqjzdai.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gfvevaqck.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkifwprrp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/ggcweybli.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gfffrbxdm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gpvbcibqq.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/geualuilf.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gaoxpzgzg.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gecipduoj.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gdterpcdn.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gafwrcgqg.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/ghdvixygu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gtmyjqqvp.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gkhmfbffj.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gvizwumnt.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gnoyxxqpx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gyfhsfwee.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gmjkvcvzh.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/galfrrnhr.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gahfjcjkq.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gecqeaivg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gunrfuklx.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/goutlkcrh.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gtukntaoo.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gqnlfeshm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gdmycuqtb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/ghrfxwpwp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gtfxgtvos.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gqacmjpez.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gnrnagtdq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/geiicbcdn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/guyabmovr.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/ggfuvpxik.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/grscyvlve.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gregrenyw.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gtdospxna.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/grnnacmvm.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gjrqwvpxg.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/glnvtypbz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gelfdygxl.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gpznocloo.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gamlpbqxu.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/glqatplpa.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gvruinfxt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gntevgnqa.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjevqonxh.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/ggoueyigt.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gasmpylah.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gubdkwmdy.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gwpsogwkj.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gptsxomvx.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gkrxojlbb.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gverzycfu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gzhnmlmtf.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gyrxdnapm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxpiyvqep.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gzsennlrh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gvbmorozn.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gihjdaecd.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gmybztvhf.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gsfwhxfac.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gnzvhinsx.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/grrgtggxs.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gqxzcirez.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gpsxmlzma.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gbnxbvcgw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gzvxxipic.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/ggzjmzweq.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gdbxhtmtr.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gkuvogosq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gjqipmkhw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gmphpgfuq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gwzngssmq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/guxxvtlfu.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/grjnzcind.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gjehjhkor.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gdskwrcxs.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gxrugdatw.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gpdijknqm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gkozlufkl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gjemqrjuu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gjuygqgyd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/grpvfexlx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gpctbdilu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gdpnirfyg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gmwygiiuo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gbpnhyscj.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gyjpkelrc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/goyawxqyz.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gwjzkrmyt.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gczhdgzkm.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gsxzdhzjr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gwywpmvur.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gibmbmgci.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gmjbjjkbj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/geegwzdmd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtyzzldpz.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gfbjtvvny.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvmpwoavc.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gcaebwhim.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gactlbhfz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/grewqbpuh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gkaverqbq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gcgwtcaov.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gbgfkpuye.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gfifmseoq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gphkonkia.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbhxenpx.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gcdxenvdf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/getutridb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grevvmyst.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gpcztmpla.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gpsegqpdt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gmhizqsje.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gqpbwhhhs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gltgrdlwz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gtgugvxwg.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gdbvulvis.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gwnzijyan.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gfgzrfttw.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gcffmyrqk.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gethbbolw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gfwxykqvf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/graispktf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gxjavcmbf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gdesxedtg.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gbcxpneje.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gwxynzgcp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gidnlfmgu.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gpjstelez.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gyhrdddwa.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/glsxbrpws.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gdwmzutrd.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gtvhmwnfg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gkwqyskgp.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/giyhkovxr.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gsfgmbnbe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gnxuxjuol.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gipulncnc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gtfugmppu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/golymkpxi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gmeuyszay.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gazyoemfd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gfdaqooun.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/guahupnit.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gfgrpjbmg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gksyrdxqg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gknejubrj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gspsytjrh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gzfmkcbkr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gwfnfcace.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gvlhvkxpn.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gxqehbfjc.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gkldelric.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gfvyygqjm.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gsvprqdmk.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/geqpjrkjx.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gxgccbeua.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gdgmwvrba.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/glalnzcro.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gviawufss.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gfxznxzkl.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gaoesmqeg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gjmimsgym.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/ghveqnnrw.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gjwjugquw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/grsjrocnb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gvhiquips.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gdsvokbft.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gahupptkz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/guhyjimwn.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gmmsyfsju.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gadlsgtrz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gclyrzhtl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gswyjbbvz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gtrgxwrle.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gihbrxufj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gkvuysovg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/ghoognrsd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/ghopcktyi.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gosojrkbl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gdyrzpyou.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gdvqelkii.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/grgdmyrhr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/getigrhat.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gefuyngst.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gkvsbntho.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/ghdpwdlrg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjgqbqxsw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtnzkbkil.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gpfmfrpro.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfdeqclzs.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gtpdhmkze.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gmzgkuhuy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gjepactfq.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gombswvma.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gpgrkpmjd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gxhlpneeh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gkbigzlnr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gbjmzfjvr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gkhaninao.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gqddgyvbi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gowmevgmn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gmkvzoozm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/ghzohtxbm.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gwashwzfb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpaltanis.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/gcaqkdctj.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gyxmustix.sHtML


<!-- 参考信息 -->