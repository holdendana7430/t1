代发 wailian999

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2yqlmtdvu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kujlbtzf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nzwcnwev.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wfmnsyen.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ydfnygkh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2glojylrk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2klbzizyu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hoiawipg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zzugqvbe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ivztsyss.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpgzpmhf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dfozfmut.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbiirdhv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkqsuvjl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qltzsrwe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ccrfsjcn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czztxyct.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vbefjvmt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qpwsqrey.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vukhcmtw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gztggkga.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fsgyozcf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vupcwste.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jjrkmjtj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2iibonlrn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zsynoesk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nvojmvir.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ybchobhz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2rgalkaoi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ndtfalzh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vevljbsh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mcdvpunm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jfeyktwm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rgnbgtel.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2qdwaudkt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pnrqkkfl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djxvlcpx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2rtubyxmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qokqerhu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ogklfiah.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2tivethxb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rvljpxgc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tzfwttqg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mggauuib.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgulbzvx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tdnnqfai.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zvbribfx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jstdjsgr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rpiusejj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2layiobef.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2doplabml.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uauocssh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jqwcvftb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjlcidsn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cbxdslvl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ghddzhkj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsvyttzc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2dmaarsbr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2soepbfkj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pfmcafpp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rmxkgjlm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jgkiabxj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2xpvubjku.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kusczyke.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xyvvgmwu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xvojvzvd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2yvscqebu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dqsetung.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tojcwctf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dmzohfmq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvhqwptw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ihzgfeck.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vybsfnkh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wbaoforg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2otkstsyi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xlycrlxx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xrjrxopt.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxepohvn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hyobzgbg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxskbgqg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qpmtfsdn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ckdzvfcj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2llgobnfn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wisxymni.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vgzytzwk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2snedcoyo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypecqpqb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmnmbjid.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdrtefgl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lezzafpt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2trriwbof.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2zlxtnlan.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2rkhlqxph.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qsirclll.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2huzptldj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jazhnnuu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2czvdrhmj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2faxrxxjg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gwmsgmvz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2sqwaxsry.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vffqklzl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hgfcdepa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2mliifcrn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2fvzmjzmn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zyikvdbx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2srucyizi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2smcqoonz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ikvmfzop.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2quxfeoim.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bhzepmss.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2audomgpm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2fnzysnrs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2euvuiasg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwmwwfav.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2spzfcgqj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2qqilxvzp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2fubftquf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2udzfrwig.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fizfmboi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mneogtya.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lkbdrhim.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2sisopybe.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iawkucsw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2aincjhcz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ybsqxxyk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ynbcgyel.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2opddajta.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qxlthuqt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ohzdwcdx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bccoqsys.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2fpqjofwv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsaslkzt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzvpsgsh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpaefpjn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xjozmwyd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pxggoghi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jiyciktk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcyjnyku.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xnfnsixr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2iwjidxmh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjzqejsk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzfkclue.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxanagbx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnojsnsd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2olumkusa.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ehqqmvoh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xmdcwyqj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2kwobchxy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wcwujarv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vibxewgd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vhrejetm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cggpigjx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ncpabwee.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2iwayibps.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2fidioxrw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2avnkguxs.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jrukkhmd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2cavvzypj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2flhxpopk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2pudtqwvg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2seoqifrz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bywydhmv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2qtxiamcd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2upgobeyh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2gqtyoetm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2viwlchjw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2mgrpwjjc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2enfddbpc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2fibbkcan.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bcwephww.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2asmiunrr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2cybdfpll.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nfsufmdz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lnfdadwk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vvaitnai.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2xbucwumt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2lipixyii.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qjqqvijk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2upvalgkd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dhbfbtyr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2cxgojtme.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2blqxonuz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gprrwopg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uemyhcsk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bzgsxzlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmhnsctt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2jzmbcqjk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ksstffqa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcytstin.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2akdelnzg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfmbasiz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2lynmhjas.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2rcqwtwjs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zqcwftqu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2byqiifhe.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ykpytgrp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2tweetyyc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2axrkncgb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kfzedoqg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wtuculdn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2doyblsjd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ckabphee.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ttmggyos.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eehgitgo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2insxyytt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2bmamieka.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2doeysuop.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tyyicmsd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wkgonedh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2glcdpove.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ivcbeooq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2tqaaajqb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vigfcqbi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2pdgibrpu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2wngkqsjh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnfjurqe.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xekaeeov.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cmziiyek.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnqsanpi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cclnfqip.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2mrhmtupf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2njejzmpl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bncnpzsy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2pnrcdfvk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2hewoslxq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gevopvub.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yquvnjse.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2isxcctnw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2njvlqxuz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2iokketud.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2tncnymys.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2wwgydsza.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2zoaliotm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ztfnepjw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cvdstuea.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2skwcamhb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ttgczeyg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kucpjwbo.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2rskdhagb.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bgjzelts.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2xudbpyae.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2eflofgfv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2eienfuhn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ndhzzuhq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jyvwhynw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2rwgnjfsg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2olxoprks.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2hstwwopw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dlwynkeo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2hliijqdn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2zvervgvp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2dlbinhsb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2tkrsyknx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cetpctjd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wemyqdfl.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2eulieebp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ezciipyb.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2sfuwsgjc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2zttlusmi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2yfjbebub.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ycdhuvrp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2zybktyfv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2algzjwbx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2cakkfatc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2twgonias.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2wsnairea.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2gzekzbvd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2bzpdkxap.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2rmndaytm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2yppjibdh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rehpssro.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2txhjzpen.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ulpkwptr.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2zymfnhhg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2pvbkntpy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iepjdivl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpxnevbl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2hvmmwkkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itwdikgp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ojukqaud.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2aejdgsdm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wosuujag.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cpmdugcy.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ttevsrtg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2hlevhzvb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pfoexupk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gtcbzrxw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2myejheoi.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gqdekmyz.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zmzpyibi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2mceqpxht.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2wtnswloy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xlvaxcno.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aakxndsv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jzvinoad.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cpkvbztt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2isfsfgfa.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2klgngdlx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ovoghjtz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2vxxbvrsi.html


<!-- 参考信息 -->