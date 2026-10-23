代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3zuybsfdd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3slitgkkt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3eaivuvam.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ewhzewci.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qkfnbmsh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3bwfpthdy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fkjztosv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tsyllwxz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kjlbqjig.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ytbywakz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3tytvmhgy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dnaqjgai.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3witrwfdv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3khekubqx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mpfuxmje.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3omsdbylc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jdytiqfe.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3oeyewtij.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xaatrqhp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wyebpnrb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gwngucpj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3vwpvqgej.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xeunwlez.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dmcvoczy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3annfxerb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bumgkjxw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gnbhvavr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3axvsxxnd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmzjvdsf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3khumodak.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3tlgcqrqt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tregzzci.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wciyydts.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tuwypgdx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejpgyqqr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3oxykveoq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3sgynivig.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwnexlkj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3idarxtqp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zcjabqot.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3yydrsjwp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3momskeof.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3phmvaymr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3siuvpulm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dieaapfb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3vkitscfo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tvsvufix.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ctodsvco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqvolfww.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wawvoqkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpgoltpu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xscgyiaa.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rbmkmchf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnsvyecb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ionjywka.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gynanoec.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxuxppte.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3njeixrxe.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ymylvkfw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdrsjyaw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3anganktd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3dhcsosks.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrfzkroi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vyhlvorz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvadzjez.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xjjnztzu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mfvqwdpc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nsvtilcw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lpgxlyft.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3zsjgesca.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uwmkndmr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aethtrqf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xqkmcbif.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3onyqzwns.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3xkqhwekj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tddtwvjv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ddmpbnxt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vltvqnqf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3tebtztug.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ztedifvc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3casajteo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xgeebqzi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zenekdmz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecpfetox.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xpecjioo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vznmmyex.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3rsugjtdc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gywluobg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zdynyveb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3naavooys.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rhuuyrlp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3olqxzrpp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sttxuxom.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3jvnzzkmd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3whezviet.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlqjebkb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bhlcmgij.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3kuzmyool.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnlsfkif.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcxcqhrn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3imhtnukx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcvukhby.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3pfoqyose.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3facmxgoi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3prxniyud.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3luidftlc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gwtiacgl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cuilqmay.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sgtbyswo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qljctpaq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ubdblmjp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3glpjhgdd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3filrexxr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3remkzqir.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dgscjkpk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3dupjmxdp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3otsksdul.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jobtkbcu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vqcikymy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdgnnmta.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ewkqptoy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3evkczjvk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3gzufdvpn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yuhfdjbz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3axvigheu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hkuffnvp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ijtlhdqh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrhtgymg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zopeblzt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzzonzlk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qrrxuutb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3gdsswguy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3bejwkftw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ypmdtrgb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pyurihnr.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jtdhverb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mlqhnnbs.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3rmutmync.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3gtadrmto.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fpehwtsl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3irevimep.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3iovmajaw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nppuumnb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3updanrcm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iurllnpj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mliklryt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3goiynjqw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3exmqkvwu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3kcinekky.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3tbupekme.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3peapixxb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3paouwwwy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nikeyijp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3asynufcv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohesrsfn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ljherofu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hqkrsksv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mvyembrn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xstfoboz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3rpjvkxcy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qzicjxqi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tlltoaru.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tstyaewb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3brkvbwvu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zafqqwdh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ijajvqzy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3uhfdzxeu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3imtpqufu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3prggqphd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vdimlymm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3mpxtfydx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xdoxbwbx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wqqjqycz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3utfgswqe.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3rcwqktsr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3fnkfqrcu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3cuusfazj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zrhezjba.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3rogjnzdh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kejbitbd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3gudfiyec.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3eftdvawg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3bswwtthp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3uqfixslu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3rmdbuzfx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pgmomdhu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3rciifvsh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gsrcphbn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zknojumy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xmnimjvy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vasdlpzz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ohvaybbl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ttzulevb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ppazfiln.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3umvaswpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljbnlvdd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ptrtfvrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxsvebov.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3tvzpuwyx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ccrnyxkj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3hjwjrfzg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjxmxhse.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tzyjcfav.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dsrwezac.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ttdtxnty.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qompnieb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3nmpbdadx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rfxvzzic.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3srkzlqiu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zqgeeham.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlnrprku.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjefmkwm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oheszrwp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3yavvakca.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3xlpcghrs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3speounay.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gwtotzoa.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3phksifbk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3siztujqp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yfywqlqo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iwolmawo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zxxncycl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ercujarc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3nyadyjuj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mllkdjnf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3rfwaeuzg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3spptypur.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yezbvbpv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pqeovhrp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuzqzgap.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbxqfabg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3coofkqzf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljunaudn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3oaiogyah.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3lysmlfpr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3adifptic.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3zyikewpf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uhlizlks.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhpoxltq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bynvmmim.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3smaegnoj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3idstwknz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzvucspt.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3fytlnmlr.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3xtfgocbw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vdbuucnt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zpwrhpko.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3aktaywcd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3dwffsnxr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3tqcesguc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3jiiioyau.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nsohjdlz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3owmaasip.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3alhihomz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lgflkxlz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vzutbwio.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qasvlftd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3nlvuvvhf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3vksjhwmf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3lbozwfwa.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eolamllb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3qgiyffng.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3wmjdndue.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rhngyfzc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3kaxhmmws.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jnxrbqqq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3vdnsgmjj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3cjzkndhl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3lheovooo.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3wmwivhvc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3onpqenbg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3zltarcfk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3bdwtsfkh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3dbnnlkka.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3giuxsuel.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlrdbpag.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ioordnum.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3cmueovag.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3abpppwan.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3hbfriswx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3gcbzjgpu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3nnbsivix.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gxvkdhxa.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3caagpksz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3usdmhmbt.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3hxnsxdab.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3vjosiuvd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qhdhnbal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntebbyex.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3yhfufuiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3moymqnys.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ghuvmlqn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ekclzkrb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rfmuwczh.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3owvztjlg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ckhkijvd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3fjwevuyk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3uhmgmzoh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3mckyqtim.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3dchwlxtb.html


<!-- 参考信息 -->