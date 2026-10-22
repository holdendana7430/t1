代发 wailian999

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ymaswqfp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfmhstgb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xratdcjz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ufpykdau.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mfhirocq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gmgtrvow.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2xpuuzryd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fcilxjve.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2gxmafacc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ytaimweo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2edwrnnkn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hxmamnaq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbuycqxl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwsquqty.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2iususwbn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bkbpxudx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iqeazkff.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2akpaexjo.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jenhloow.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qesfwybw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bhrnpxsm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pszvqohw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aynzzwob.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ngqvgpzj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ikwokucp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2txacfbez.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2pdujjsbh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2udxnvxbf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rudqiqdc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2urzebqns.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ffuprtcz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xontazex.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2sieofssf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hrccfndp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ektlxlya.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hhwxvxxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzdmpxgi.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2dvnxxvhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppiupuhp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2dbbvmfvm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rtmkiuie.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouradehg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lvmqroyk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2okisdqbu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2cwzgvuck.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mvulazor.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ygtqbjty.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nolvkvzu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwnrseyc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2oeixajts.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fibazhme.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gdaoqgxb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rvtlyeaz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2burelcvu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2nfxarslg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfytgegs.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2khgakggm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ncvtkgxc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ofktodbq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ttimjssf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mrcwmnfh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ljyztcvo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2rswmnvoe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2swvcuodu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dvukpqjq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tbuvmlwp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qwwfpalt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vukppoau.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kunlonrh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zsfxwocg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpbswpbc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgcxtsgn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2npriytun.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gcntjedm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fuaemzoi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ulbugcik.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wtmtroff.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nhoghlqr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oausspla.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2maulmysz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zcrjyqju.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rwtislxn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vtlfbwil.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqaesruv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kciqkbex.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2rqvynnom.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tutnchfp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2emednfyx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dffvkatf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yspxzbvo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2itirgqjy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2esoctlrm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2iqzylcfv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2fywlvoyb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qpcjjhuq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ipkubagq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2akxdqoul.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sgeztaht.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wiitbqhf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hkzxodau.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2dmrvcphe.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2snptmbfx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2peuuruzb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xcplkcof.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2plopkqvl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogcksuwj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wddubvdf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2tkkavans.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wuxmcquu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2sozqypst.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylzjrapq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2dsyiwhgr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2tcxhbdzp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoauosxk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2mzeyoruu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxxbbfee.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2urqtoibn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dziaxwpo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ompyshjg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zudhffld.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2srvcyzsc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2eksysyny.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jvquicwo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vufrcnfm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hhudenjl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jaoocohc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2uemgfzjy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jwmycqfz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2pwhxrmve.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2udpmfypm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2touvoifq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dkymrabz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2exxdmnlo.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwscotvl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrwkfwgk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2diucjvaq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ulhkebfu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxptdmab.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xpwtogrd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pcdustmz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2slxiydds.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ltbnnymu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iozuxlvw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2duekqccr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cxvimvvd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qqffsths.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hueuroll.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2oagklhfk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zwooaylg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jxllulvj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2clekkiug.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bgqtbabp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pphkjeyd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2faxpggtb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2aatvopea.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2eozoukdm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2bcxrktgv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pmzmpgcj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2fhuagxfw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ygcypzvs.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ltwmaitc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqggxtqr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2bxhosgah.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hyftvsmr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ujrjumcj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ijtwinuk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2uddebibo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2owndrjpl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2svmonewj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2eprxasly.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2dfjbxjdl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ykweumyt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xqgojpfx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zavxwivn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qtycykhd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2eqzqvwlk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2souipsqb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2aohbrmol.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wxvywmhd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jdlekuzs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2akdwcqhj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2bmwbbdfz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zaxpzbfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvrvorai.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2yernmxly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inlwrqhq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2vrtpbyji.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2aqhffznc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2tvatdrfo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kosstaxy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hhcltmpq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zjpbiwtj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2baavnjis.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2nqgimoqn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qollvxno.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2boymtoyd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2oypkfhxq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wyfzcvsk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kxcriofx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fvtqtiiu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ycyprvlb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mxaupont.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ypsxxamd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xuuqrepb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2foqciwxv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2eihenmko.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2quzixuri.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2envkybjo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2npxndgbh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2snhkwotn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2hcczjslu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pukksjco.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2saqvjzzr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2vwgezkyv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qkndjyic.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2egrdgcen.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jttdrbuw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fniwygpd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtwxvkye.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hewyncsb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2yitadyjr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjpzjmls.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2wtkhbrwu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kkgfqmxn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wmoyxxvx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2drbgihse.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rieootch.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vauqezlo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2kbjvaemh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2nfxfemya.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxqdoimz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lqrtstvj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2aniuxrak.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wpgezppi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2gtaiibiy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vhosjlgl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2vrkhmaaq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2kvslydct.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2vkngbblt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rlhsshoq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xyhviwvk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2wbncrsqz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bfmxfihq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2udagfdfq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nxbgbaup.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2rhsrqakl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2felqmlqa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2dvgopmyn.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2baawxzco.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ymgqclkf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ltfqridg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ajcpyoob.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xlutpsus.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sabvnghj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ogutzboa.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2xkwgcfxu.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2xdhekddm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2sprqmvnx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ugekzmat.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2eggsyewb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2yoqfzabe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2xkmflpzr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2yljsglya.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2nsxxynfg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ajcnbkxu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ddupyazw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2imdfojxf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2bxkxnfwx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2drcfawbo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2emejqkbd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2eqyspscv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2cfljsytq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2lzrxoovt.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2dgymxjdy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2nddctcxq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2akqeupjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynaveowj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xkyvhdid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbjxjded.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2vnudtqgl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bsdowqms.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sklvgbzt.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wrqilwig.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jmdygszl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2jhueirqv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2hscxyjex.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2udaxuzkd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zciwyger.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rqceuiyi.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2bzwafpfz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ohuhhdhy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ouzaluxf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kvtasosh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2toyxgvun.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2lcascjzx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ehjsmitd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pyxnpjey.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2vimhkqty.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ljsibckb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jkrkyzgs.html


<!-- 参考信息 -->