代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hvsfyiiu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2yxhccsym.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ynzbnemb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lpfbuskm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ktiilylj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xmvwsbny.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2utvhkvdt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wvwfnmlq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ceaceyys.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gbagcqrn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ukrqmkgd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxbcppux.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2lwykjfzh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2tenlhero.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ybjzmqvv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xqwehypg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mkmjyyqg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jirctvyp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mnxujehl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tjyhfmko.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2myzhwtrr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pujjvwbj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nwgtwyhf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkqjxphh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nikgdwjz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fgijxxvj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkrtanpz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2crmcnwzu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2oznybmsh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rwgfrsnb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ozzykrfh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2uadoptuj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xezlhqcm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rgekglje.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2bzbhnkrz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ozmcuftb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2tqdjsbav.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ffqykuql.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2yhmibbsu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2wfatnldg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyzqgnzm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2roiuxgmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wafyjlka.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cnvhbnjt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rwptcrls.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymwipjhi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ryhnchsc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cjvrahhi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rphjikrd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2rwlevufm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zacnyvkq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nufjhwcw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fpifbobk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2vkljysuu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrxqvxny.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfenmahz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jbgzfltw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ojamxvmf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2diiggdax.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jifqdjfl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkdwdpfa.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2sjqwfqdy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gsezukzd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rbxfuwit.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ygmimkmy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2skszvzlg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vehelkml.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2gaixacoc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2butpjplv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kidaylfp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2roqtiycl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hhqkxnbw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkthezzh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsofexfn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qldvenoo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2geozxgxk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xcsyduqu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2taouwsii.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2odsaltyu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wikekzkm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2sgrtbgxv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqvtngoe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iqbedzdu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2coefguja.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2erpiywif.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wqlmbdye.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lgmpbtcm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2psltahhb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mltepwqw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zvufbnxy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyvrsbla.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2odnuyefd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pwygssrl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qmkvpous.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ivlowftu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xycgmbix.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xjcsttie.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2vtwpxpxi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gtytdruu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ciswfdwz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pwarxbct.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ccgdceoa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yatiylqp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2egbrkxut.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2kujfheoo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vryybvzz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bmakowfd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ogxshvnk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2svwtwqkr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2frrkcuxl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2bttxruum.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zeenswrv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2zsayyqoe.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fltqqxti.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2djqwpzss.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2aonivkwj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bdzjxoan.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctcyoeco.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ruxvccez.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpgvwtia.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ttlwjlhc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ppxqkpwq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2yhgiaryz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2msgcqwgc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2tzyeqdoc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rbzfdksx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tdvdqnsv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2yhoyvexx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2imavfbxe.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hhqussgt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cjtqcdcb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cfhjwljh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wxaryljw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2nswuksuq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2vscorrap.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbmjeevy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vzagwwrx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fcxbfzcp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2czzcameb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kdkqfhkk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2sznuusmx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcvedgue.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tbfjeoho.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mepgnhqo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2empjonuw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtkgolzr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajmxxcyi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oexnwwir.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wnshdkky.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2txtdwlto.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jxkymzog.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2begiulbw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2qzsesqxx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iqmahejz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nljorcwt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2btoudyzj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cdcxkgef.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zkpfiwfe.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hmvolbrp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2uebepvxy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hvchjnav.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wuvhttje.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2sxramvrt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vbpzorik.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2kvctfkbc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2getfuaic.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2owpwowuk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tqelnzmx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2gtyqqzpy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nxtzrxpp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2uyrhtseb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2erzvnvyr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2juxqkkqn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2euyodyoj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2fmbwjdfg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2maklgqmr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2pvksfncj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vusdldlu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vnpjyfhq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2safvaxly.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2adrymxif.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zjzdnmdp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sybfawvj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2btyzjrpv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2fhgfjsgw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ceqofbvb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2afnpjetz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ayqzcawo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2fpwbxfyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bocvtmqq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2uqlneujw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2njqluhef.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2kaiiqvgq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ymqyhgvp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkvvapjv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2almjlxbo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2fygrofho.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2pcqwjahm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcyagzii.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wcdzdwjq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2pearawjb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuenytrq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2abhutbhx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzvtfbhb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jujzugfk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2sqkaoere.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2qopsisar.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhiflzgd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jtqfdtmi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ybkmbkuk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2phrbrgjw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hxmmwbiw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oxgcavyd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fcjlihva.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2fqltbjsy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ijgmcued.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rqhkimfb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2tbdybqfo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2udjsdais.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kwyroviy.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kypstdjb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2sknmeyym.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pijrxqxn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vsrydsws.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cefoaaws.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2gewksaal.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ktsqggju.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2iyygfbdl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2bvugqano.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ozqzfqhq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkuguhxo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yutbhidf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2gxevqmvv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2tlqqocsi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2kmcfqilp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ugccakps.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2mzkigxgn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tyjphugd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vmqrbazu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2stoikpgu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2hjiborer.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2alvvubsg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2miyifbjj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2txbitgks.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2jakyvrbn.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fjkbhwkj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wkskkytm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vurkiwvi.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kitymmxs.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2btvcgdqa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2kuxhflof.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2yjlmttfj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2motkrfmq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2dbxyatyk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2oobghyro.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2uffrdbyh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2yppxqbwb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wuihmpbx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2aamiqstp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ldlhnoml.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2hxgzofnm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2dxuhioop.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2evqzmevo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2gpdkwwmi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2qlrbosmy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2cwkxyewx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2gkqmldiy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2twxowcrk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pbubmrkb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2vljskcya.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rkbjkzfg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2gwmjbiqz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2okvvcxpr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ovvjynwj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2phwoopom.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wxljzrrb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2itukewll.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2syslgvcc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ixusoene.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xlvplcuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgkcgrex.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2unlogydm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhcwqzbj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2mncocurb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nqjpfuvm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wmvbhrcj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ofxsgqfv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kldyokfu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2mnicimcl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2gebpzzfh.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zthbtuah.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vzydahcf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2hmorjinq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2moggzutz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2wqwyoauh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2rzpglbxk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2drrxqfsp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tkgiibsh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2nfbpkcwu.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wksgxjhy.html


<!-- 参考信息 -->