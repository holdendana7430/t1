代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tlaipmda.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2wegqvfgz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2emduphed.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fdvssxnq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ajjycbfb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2usnhychc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2snsdzrnh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fqiknygs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2yybmahty.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pclcinyd.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dvuzesqy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zkmrctwt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qyjirljy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jfozohnu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2lhdmhfwd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwdxfqas.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2lmzwqdpz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2witqtngu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vqemwjma.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2drhbhzhz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fbbkkcau.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixuyuvdp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2czpvphgt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bcmpmpar.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vjehvxwp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gcisstad.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezqfjwnl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vsevpqbb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2evepaabr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2twvvkxow.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2miwiykmi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qxxdoaid.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2oeeiavwf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cbgtdxev.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rdggkjao.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2nlccdvdc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dgxmgnkp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wffdhapj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pzrhtvgm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ytijyodl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2uauwjxmo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bynrigmu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2olxyadlk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2bacvecsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpvkkjrb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2piforbpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2poxalqpx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2juxrejqs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fzedordu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzejqwov.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2onqkejbv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozxlzkmb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qxnxynsg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2psxhxqxe.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wiwskyri.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gevojxns.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2nkwfdizr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ullzpsnk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2etljpiku.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2boewnmqc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vshukmrr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbenevci.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nnlopffy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xghprkug.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtaeahmp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2mhtalmmz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xernvutz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bqlpauch.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uyjowmca.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zvhzcvnx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ayepxdbc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2nfblssue.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2efaswovq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cgythoac.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2poqbabra.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qwuyfais.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmrlahhu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2llbyvquq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubngndzp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jxefobmv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2luzakzmb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2johydsaq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gkwmgvge.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2phssljbk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2usiufgnm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2truzzsdl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kejvwict.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jaibhwnz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hysbxyfz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ksqhcxel.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wffqhxoq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bwuyoxhh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2oxctvtwd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2wfvidvkx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehahbmbe.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sseywzwg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2willudkt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhkwnpoh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ogwqofiv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fldbllqm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2odvodkuk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2sjeiwahq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bjpsuvod.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2voqlfgem.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wnxwowkq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xwzarfkh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ffccdbie.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dgjdfkfu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2uikneicx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2vzwnkxfx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qzxmjedw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xtwfyfba.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wmlblwdh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rdrhpoyp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2tqqsrxhj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywuonydr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2rgdcemgr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2eduqizvi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2nlitingm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2wlkfwzxk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2fnrkwwrh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2weefjlca.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ohsyqryn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rwhckmcu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2easxowgz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ronlodqd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ysjwcyef.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kpzzaffn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2fslwekxp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hlejmtfi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rbgnmlfr.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2gukrpdwe.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hplfemmb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ybzhmdvi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2obltzapo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oldyrijw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2cligeupj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wscmptog.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2svcnatzt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lghpzngn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kolyrvwt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cypxniuz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tljnbzfa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pvbokrfb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2pybdkaja.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2phagxnle.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mgaryuxn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fiafzcpi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pwrishvm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgmsfkwb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjxxjpcz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdecsuzm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wpdnhqxm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hnbtkuna.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gixdhovk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2tumuhfwn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ihdozgjj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rpbamzdc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2whcymjkg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pjxrywmj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gkfnngyw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2muutkjjt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2tpuierfc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hdwnsjyv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rmamslvy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2doypejpm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wigjoqnt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2asyrybxe.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rqhrxeuj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2iuqtljzr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2kcqjqacf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2kylechwt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2unspqjfg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qyhenmzk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2exosinhd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuhsitky.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bzjdhqih.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qqqfshrg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tuutbubk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mivmsrly.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2rygbfbdi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vyqksokr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2gzgumxkv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2sfltdrgj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ivkwceks.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tulngzgl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kjjviilc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2uheusoym.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2xcocibnh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2kvlcrnzn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ntencmqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbvcesll.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mfkevqey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swfnmqxy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2lyjsaqec.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xusqhxuj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2izghuxqo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nasdzmol.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bkuhftux.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mhqmmftz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2kruqzfzx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2dxzibneu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2bvpxlkib.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vwdkvcxa.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ueezunfu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pkhazkzo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bfexdtnp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2egdiacpg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkwoshuy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2jeymecic.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2bvvwmpxc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfxqqkis.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vdngmupl.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vseepyuo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zyhphhby.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gyofbekr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vetvdhmh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ivmzaxrj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2wlmnjhwg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2bmpomlmk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2afshldmo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2lnmqkjjx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cceuxljd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2oublfwob.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ldzenkdv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bvapjufe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhytpjug.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2jcbjlxhr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2hokkkvph.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2xatmlmfh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ymmbxief.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ttyvjcwv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2pvnjpvmo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lxlsuntx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzkdyyln.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2diehqvkf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2whywjudr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2jruvrnha.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ajhwlvla.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lxtciwkc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2jgdxfkwf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2eyjmyzsh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vwtmvgoa.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jiypfwqf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2bfbrigye.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2yuuadbxc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2tprijnya.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2nmiejruf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2fwvqncoz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ursbkged.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sghalunx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wbsqsqoj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xfbbvskx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2fbbudwvz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2iynnzrhx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2vboouclf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dgftafgj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ipcnncqb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2qczfpugr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2troawwzp.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2wtmdvgwt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2hjxnlvgl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2jxavrlql.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2xnjogzpe.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ragizwia.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2sncbgyty.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2rqgrzvog.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2tpcmwnud.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2wkwjrpyb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2okcuhtkw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2wvnsnquq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2txcmxsan.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cjwebiee.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2hcpqzutc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ouidokht.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ladymney.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ckmlyukq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gahezxpl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2sbebezrc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2aszjlpsx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2kpiyukgm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2xfmrtrmj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2fnagppae.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mbdsrsde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlakjolb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nutwyetm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eddvsfdd.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2rgennvls.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvokcfhs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rgqsjwve.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2tvmssxoq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zqmydwxc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2ctnomvrp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnthwtiq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gxvwvmzk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zqfsfsxr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ecaxjxra.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ibzqgiob.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dozjlrhy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2mvwcklqv.html


<!-- 参考信息 -->