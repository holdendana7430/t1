代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rxckroaa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jkoskvbr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bcjpvwiy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nkaxyomn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hrqkqube.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gptkhxdo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tqcbdwvm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2livswvli.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ilqwwqjh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vazkatgp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pgmrrinv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2klakmiug.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nibllsla.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wqwarchu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ntzzwrxv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mamvqrlo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2aruqflxe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mnuwcqsb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbjmgezx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pdryzcpg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aytkyzqc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nvpzyqpr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2droolhhc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cecsqwpv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2grskxcqj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdciqgrb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qadjsniv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jekcackl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2jccyhagp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryldmxxu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efplppuc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ummdppno.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2guxhlutx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ibperori.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2bdpbgciw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mwcljbym.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2gqblhtvh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kejtmzjl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2rkyluugn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2lxfzdmqc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gxqdoclc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hkzjcokf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vcletiwa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gmtmfqqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cltingdz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2bclzvdki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2moeqkgav.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2olxauknf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ybfgmyzk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2slkptuyi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwolfueu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2npkpzssy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2icinoout.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ycgoueir.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2oktbviyr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nliicxqd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ivpvthsc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2bgrbjtbm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxpdtlww.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2btmekbdr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2uozujiya.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2aoduxudt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2tykclqdd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ltmpcrld.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pdpsnrpr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vceejeiq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ejpjvuty.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xkppmamz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tjtshlwn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2fagesrad.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2xwvndvig.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2wlgquhgq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ztpwyjsx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qbxnvlbq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2plliyhhd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ipseedik.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fpouttvc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uljowrpp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mzbpjzxc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zkgwdwpu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mtbcgpdf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xlckgyyx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xfysgjyc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2bqvxnnwa.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2noecxuqt.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdesmfoe.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2svbbrljq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldwkdrkt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2heznuqxv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pjwgksrc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wsozhaym.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2luvzsmea.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rzscywzh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2mokezmme.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujdsotyi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrwrrobr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaniesqa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pxzfqccy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2hggvzfhg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fwvttxer.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ufjdsfkz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2uqizozgx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jrvpsfkm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2egskfqtn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2inedrbic.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tzrgfswy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mydgieir.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2qlzsgiuu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qlkhfrbr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2exjmzlgr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2jqborozu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2kywujwzd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mswsalij.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2piwxifti.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2yipssvsj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2lvgyahsd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xuymlpol.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2adjakrcg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kepfbovd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ajpozlqo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jvlmfvjm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2odkyaqyk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2dzskcaag.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rpjfyjyq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdmtttir.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2plonfrov.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nvgqzbed.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2wwvedynu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2surqxerc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2umkjgzvv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pzgyidsn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2yarpflpw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pomonmcy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nehtqgqk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zrwyuizp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dxohmvqi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ijovjybt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dvphwgjg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rwpjecks.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tslwnlah.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2njwlyvfr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocxcwfov.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2adxkakzj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tqipydma.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qxkolbch.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzvqqiju.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qiowgouu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ifuodxzm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkcvwjtd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sflsyaii.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zeeiwcbg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hjoqzrop.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qqrjtyop.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2faikjwui.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xpuswnii.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2tctqyoue.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dancaozm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ouwdjzyj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2btrotmfy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2shjsqdmz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wvxgurss.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2euiwsrpd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gszgsvzm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rpotzkwj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2znxigdos.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jfizefmp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fhcjprnw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2atgbezif.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2uyhpqetn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlnkdcwm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tvknqsdq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2cttukcqs.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2woqpxehi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ecmmskia.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jnmzmxfw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2hkxmbqmd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zsdqktln.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nnhwsrrj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2gzafaziv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2elhhzhxp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2carqvoen.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hobgvwjn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qsgehnin.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2xldveqzz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mfxgydwt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pnltnlje.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uruvhbpl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vnlmhiby.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2kcnhirmt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ckwxghoo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hwwdkmtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptzevmfi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2eaohsfgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dctjbhcg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2nmjfgcpp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pbabzvda.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpcrjpcn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvsaszoh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymisvhjl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ystmajte.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2cfucoduw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2chladxya.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbfbsvnm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2xaaqxzeq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xseaktzh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jtlmpduc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bawyxjnm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2voprcpjy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlvsthag.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2hxfrabok.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2njdptjox.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rjtdmnde.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nmqpstdd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ifsbzcoy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oodybubi.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wzbcmvvr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gcdskvej.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jeguszkb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2fvfdwwwp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2cepmbmxf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ahmlzfsj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2sbntnzij.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2oyjfjisb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yizxutgm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ledugzjm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rdmqfesp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcgaalzy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2newoleqr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2toivnutw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsmiwzcm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ktfdjuvf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2qwqpwmvd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qzeaxkxe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtiejryu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xiclwbuy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyskibqf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2kmuqxlda.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ygfrahqe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ondxxnrn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2kzjoapuw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2pfsoyiih.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2igjtxzyi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zugmjcse.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hykivzvm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2mchywdra.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2catusklt.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2lzzzqbsw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2tlsegkjl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2wporzspv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2zildkasd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2feaitrjm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ioidcrbi.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jyhhgkvz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2smzrzydh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2dofozchk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2wahajefa.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gsdpqzbc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2mcbovjpc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ohzqfwiu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2cfumqrzv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2efspqkwi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rvvdelwj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2kzpaerec.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2kwbaczmn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2vbbhxfnw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2yizmkfxu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2jjvvdmrm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2npysubhc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hmuqdlrw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2lgobfyhz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2mpfrwzwi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2esrhdlcg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lqfxyhah.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2izlwskxh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2cyoknlbp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2gnjfsanq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qofmxzhk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2sfnhglmc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rbsqtwta.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rxblghol.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2lssqlwbe.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2chrpnwnk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2wgibbdta.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jcxweypd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcbrcgmc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2pwqkngvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iikjjsuh.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wgbolebu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wajvqpyd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nkcwehqm.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2stbxwavd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pdbenvuw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2zjfycaht.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2atyribsl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cpbhfvls.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bwflamed.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2grfbjull.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hughnask.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2leortmgl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2gceufqxi.html


<!-- 参考信息 -->