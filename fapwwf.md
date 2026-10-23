代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3uxmjmhwz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3toeuqqsp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ddhmskgm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vceagpin.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kkffhvmd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3efrbfvks.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3abpbnvdj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3equqgtuw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ezmrzfdp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3litckfag.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ubudkofi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qyfychjf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3smbvqqzl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wntfnici.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3kzziyljf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dzmxduxg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3scksxskq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3jvnhfitw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oaupahkr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ihsqtumx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjxjznqr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pxkfciwf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kaetawyp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uixvcnee.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qjbzhbxf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3odonvgoh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gynutprz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jklsyzrb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pdlsjnhv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3orjiftjy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kogdohnv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pbuhwtid.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3hssdifgz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3upunhgig.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ockspqen.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mhzncupz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ccurvvoz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ljdpekzq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vipjlyqw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3oxulcifv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ajjxuynb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dxtfkbzc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3qzaqkcra.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ymrajzra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjbbbjsw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ltnusakm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fmproazu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fukisked.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3sdczbjkg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eutgvfyk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3afyfnwxu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgcneekm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3tcxkbyxy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3szsipqif.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ckxpuwdu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3figdupve.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3dyzrxuyr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zguywhwb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wzaeyruz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mofinfzi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3phngdmik.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgrjxmew.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3eylbwgra.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3cyxgutkt.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wiwdqfoh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3iyhvyxzy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bmlwyzkp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3upbbqovh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wtwyezul.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jhsipxxx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qketwccz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ggkdhjgd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3igmlcitw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3elyzjxow.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3rcbfozjc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ysbjzctp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ymygjffp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mmzduosg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3biszajxu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpylbjao.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3moszgbwf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oyoarcpy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hbhukorz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3omtytrdc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3dlhwegsv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jomvvvew.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kysyiudl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cplgetql.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3brbqaxho.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lficattj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3submhtse.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3skjwdlkx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dzwhmleu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ouszaqcv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zvpoahew.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mojedmhf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwalihhj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ywbcogkc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3wjvjvknh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3bkggmyqe.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3gspiyrcr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vihimzcj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wxmpnewz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3umnvtgtj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xkvlsbpk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3antyylxt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rdfyfemu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3gdbhiyqa.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ctetgymf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3pslgsjej.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ayxiygju.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ulzjkyjj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmsvmmsf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vsiwmrgu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3yrooduow.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lkfrskxh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mvlbxjcr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3botmtxep.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihugdili.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3cefsuwdd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ilkroums.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3qcyqwyfd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mxqhmlux.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3cturqobp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3mkrriyfl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3umfznhas.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gwyncsnm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mffhuwdr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vlvllwbu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3auvodfxv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3klgftvbk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3szefcpbe.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3eohhfbpp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3okvvbhyo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xcoacdoo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jbcouuxf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rpcjtlwo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3slqofyrc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ictwekhn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3seedjfjp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbbmioqj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3azmysony.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhtiyqhh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fidjaprn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3uvrpmnqy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrugfdxf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vgvyhpxw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yzezjveu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnhxrlwm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtrnliqd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3akgvvwom.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lclxrqih.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fscsduzr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nxoeyyxv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fnzwdoop.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3txrtysxj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3liqsisfj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kpygbbqo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jutvrydz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zxgqyili.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bthztsnr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3seyryjsv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3srjgtdtr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3rwjhweqk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qasycegv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ffxeuvkb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3fatvkfnv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3hokcczws.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3uryhnhmi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wppzubdd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mrdmsgjl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3dapaiypp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3dhqswara.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dysxovnd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kyrkesdp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3fdcnloyn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3yhppxuom.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lazrozvl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3outhqixp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3yenhviap.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3yzgvbbeo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xtvtphpg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nwbvmgpl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3nmazyvbs.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ocypvulq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qjutdtyf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cidgyidf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qeptsouq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vmuiwioj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3khtorovc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cdbgabtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydrvrflo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3alqwyehs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eabljjjt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ruxtxsuf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pqkydkkn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3osatffea.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qaqyjmpy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztcyrkaf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3qabjifbj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jccngown.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3okrdvyit.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3znqjguyr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3lvgqgpvi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3cpnkulop.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qukzbtue.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wzkutorj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xydlzwee.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwfcgtxo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3uokncrji.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qzbpzdev.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vhkgbdbe.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3doroikav.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3akpsuhzm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iczwcnbv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nmrabzbr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gsmzsnzb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ikgcdxie.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bxgzokno.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pjhnyttv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qzvlggnm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3srhapjxm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dfhbwtcp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ukwsxoiw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xuvayutt.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3plkvabba.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lqttsbok.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3mysgtbpn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3bamzfdrp.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3omdexcbm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3vzzswmrn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3obwnvmws.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3rvnpmrqn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wqpcxekt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzlkvxrf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjcxrtac.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3jozlpkyl.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3gdnjjgtn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3slnetssh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ckkvdarz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3mbflzbqd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xcjxanvk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ouentcrc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nvorpwhh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3jfwiqiwd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3xalzhrsd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ywadkdmr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3czucgvos.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3rliswhia.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3yzcobnwa.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fjbbkmss.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zezqxdzv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yxgagnwv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3pstfgduu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3tyizdnin.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3byczucxz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nltegnho.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3pctjhfet.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3tljeakgn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ibzbijbz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3fzvrbvwz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3seceyooy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3xclyvpbw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3voqizkgt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3pwlsgtlr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ngvjmxbl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3zkqqnfcu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3sdskdzuu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ukrzdown.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3lydwkbze.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3cjqrmuuy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmoavfzn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kahxvnhj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3eyfhwurb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3uohnhtuv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3bhrzqhme.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3fjxboykq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ghnvxsvk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ozyoyelu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3bcqsznvz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3qelgducq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3fgyzjagv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3uahuudqy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nttmsrbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tigtlzan.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rdotvdma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlpddgrv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3wifcybiz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3yrsgqpru.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jowvfmdf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mxwlzamz.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwlfvtxg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3rszfjyhd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fltkcqcq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3gsvonmvd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qfpytbxg.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3txurjugg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3npmkziww.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3iugfbmad.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ybkdxheo.html


<!-- 参考信息 -->