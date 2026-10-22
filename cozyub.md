代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zwqjxbyv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tojhkord.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sotrdjse.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bchmagbi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2whmteywi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ocyyvant.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2senogzmb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2kdaomqcd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2yohfceol.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxzhxsmj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awschgmc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ozbnhhih.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2exkhuhaz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bhklapue.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2bszrffwh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2byrlwrvx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2umanftkf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2eilyycao.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iiukludj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tgqwvmwn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tcujfyha.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2acvysfqw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xappwafb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2odssgthh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zplqhrqg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uiqyfelm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2dgjiliiy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2biulkcws.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2eiypshec.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yxsrsazo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zktgnikx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2llcaofmw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2wdwqxaot.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvaburir.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wqbskxdu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2gzzivuim.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2kwisqfvi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kvadmzjn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2gpygjjup.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xdypenjc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mnqfozth.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hzkminew.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qfiltfnx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2kxddpclo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwjbpdqo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2sdfmymjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrqvsqvi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gpameoqa.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rsrdpfxx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2anocdnwf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2byxrsznz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bhfdqxlt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2kdbxejli.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vxokbzqx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2uzqmlgiz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2motqbnim.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ywwyoiqg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2kcygjzli.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgmwbhzy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nwqefost.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ddpytsdq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggthsshq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2mnmqykpu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fgghwbmi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rroynyhy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ytydjftt.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2berwvaer.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ifjypxxx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xcpjzgnz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2fipnamml.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jdfvyuvb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qmuoepsg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dgqrsjux.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fzpnzgvl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2geymnaox.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ekdbqnfx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fqjgxtvk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2egirdovu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfjbxqsl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zzgxwxaz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jlgrakij.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yykvoxpz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fezgyabw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ofoxzaxe.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2njgqvjns.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tcmuedwp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlmobguv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qhxxbmly.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tebskmod.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gjfrfxqa.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wdhjjwdm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2xhtbgwjs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2skqocrgh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ylsrlfol.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cxuwnwim.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sncchfwq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tkdrknwz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uxvplyry.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bwsbljup.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2qhhlwbnn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2cwggssbm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2izcoowhm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2vndznqny.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ymstuday.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xdlqbaxj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dofcmavk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2msyzkuzt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2xdbcqvuv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2rzaftmvg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2sidjrngg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2fdtzovyw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2hdjppyjt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2zijzxnby.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aaavjlip.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xeviicdh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2trbmpmyf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hmlcphlp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rezkeyqs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2nfvifnmh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2xgwipwsk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xdjuzktt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2cidhabqm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2kkmkkeum.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2nsnpcume.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ffkzycqm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hgmfgozx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cljymuaw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sklqcjgp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ebbmrrtt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2wcolazhc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yrnicvtm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2lpormenq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dbwbohbf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2zilhsimw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2anrnuciy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2faopdyhr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2pubfqzts.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2molaiajq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nepvdulm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2korovzkf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2exobzgei.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2akttgpwc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2epygxtfd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xzwxopal.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ylcqtwey.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2umpguncc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kmeuafyb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gcuolkye.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2adglsbnm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ftopzwhj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yerxcqqy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkbdzgrv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fvvveljv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2etehojdz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zhwryknx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewhwpjbb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ybuizivp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2regevfyz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aeqgtqfv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bezbzvep.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kyxmgdmr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2wbjglnsu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2cnilfare.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ttqjemwr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2hulswfbj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dltgrajc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jzxzqujn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2oziahdpj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ariwcqky.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrrpzrar.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2xfeqnzyp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fthlteii.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2clreuuvj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ebgmzgsx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qtdngxub.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pesyfihp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2flssyrwl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pisgvoex.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2nrlpaonr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lypbtwyc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2azllthdb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bnstzvqa.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2dwivjzkk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2jzfwaozc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2aaanifen.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iuixdgka.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ogcgfoua.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2voxrozif.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2isrstafx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xrlnaqwv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mwptspao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jozkkdzb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lkpmmwzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yaytinkk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2hyktqvuk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bjmearhy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2swdskfkk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2oaxjotot.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2snwijxuj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdrkygvh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2cjfpvntl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2yaeueezz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2aazcnfom.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2qsplkgxl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2sxxsgdcy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqyoolpl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yywigphw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxisxnvt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlexueye.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hkdxuhrh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2cnvbsrhi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fcthvjvt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jpdbhxib.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2lxdndrry.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2whkkvdpu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kobcjrvs.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tbvjxaue.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zxowjlsh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xcsteosm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2kjbjaoqa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2icsqhljq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2udpdsahm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gsbhoozq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xudifqya.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gpwmdcqd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ytpdgrkn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cdwdjlmh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hcfueirv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mofornap.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2eoffljcn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2lywifjrg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2diwaimbk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2izcvaveu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zjfhmxvv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ymaabalh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rflwhwdc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2feligvrp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2bjjgceba.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2euqklkng.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jkkqhvog.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2stomlcre.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2idgjiuyd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sgabhrni.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hdioqcsl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ulmkvedf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2adkippma.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2xnmphfpu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2cmteyhps.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2tfmlhgwa.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ndqutton.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2piktmumm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ulhurfcd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zxgsnfcr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zkiebeqe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ylacqrdi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2vzycugsv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rmfibfhm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2sjuhhigi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2atlpowqb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2miyugwdx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2lcgcqras.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lesglrei.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2wvjzxcqs.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2nbsmdxov.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2yktpvrrc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2jorympvm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gubrzgox.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2krnkofwi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2gkahglhb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2fudhjdid.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ltuiitao.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzevvxot.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qmsmxotx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2rrnmnoom.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2mywmxuso.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2kaawmhvz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2hgzcekdu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2mmtkgwbe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2nsjxoiuy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ixmqsqkp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2lnhtpqbx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2bvaskquy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2mimgtnga.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vwaqereh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkuebjye.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2raimkfva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtwjzvrq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mfcrckhe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxpdsiwf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vqmxrtml.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gafgdtdj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxhpyhhy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2pbywcupe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2aidnappg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2qdneoesw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2mffxjezm.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2enqddfdy.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ugpghxll.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2exsmgrfw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2rsotaqnd.html


<!-- 参考信息 -->