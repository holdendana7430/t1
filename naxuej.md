代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2msnjxqwg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2nzhisvmm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2pzzvzulh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lazeosre.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vtckjrth.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2advapraq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cieflhri.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nbjxqrpk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uevqrzbw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qlxjrvde.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tcumtafn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ggaudhxd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2nyqhaxmf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eyuoexbl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xhyahqio.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tllkdeai.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xzehrsuc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2njrnpmax.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2znooffhs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2omwpvjeh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2eopijbrm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dyssusug.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asoogaom.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uxksnmta.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqrqaiyh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ermcnylw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2neprgigc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ebfrfmec.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2przwhamd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nnahodog.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ifxirwnv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajlyromq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2jzxzklul.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gqqindfd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdyczanl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2buowiboh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2pridousz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebhmaccd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jdyuykex.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2zswzvrhd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qejclebp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2orphhxke.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zogylctb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hvktgiis.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2aswgjluw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2dqwwjngk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lgvpnhdk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2wmeuvzfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwxdonqb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2hkztxhvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lfyxxbjp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cjrallss.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rttizzru.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jezsecne.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gtbamago.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mvkdceup.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2asvywijs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vcwkiamr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ydcoqxrf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ooghvrjj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2uwfpgokg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2fawmpuzy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfvzactn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2brzbgukd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2konulxbx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pqrevauv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2sfmefuqa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qcievuwd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2twtepool.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ncocvsop.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jdxmngsy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jkfzjhyj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rkxmexad.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jgeqzsmf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2amjmkhgu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wuilaxjl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dnhjdgfq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mqaybohh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nywkonkc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xvmcukfh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gybnnevk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbfoodla.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2npkecsib.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jeggopov.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ghgyxlxm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rxbppltq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gflolcox.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ybwrbzef.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2yjfmmnup.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xvflfwzg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2syygijlr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hfnlsmab.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2aatnednk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ahjgkqzh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2enzfqvih.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2liwfzzze.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2yzrfyche.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lcfrvcph.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vorclebj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2foiwnaog.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2avhvxutl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgnqcrnb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2fvzcdeac.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2aotrjlty.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2njgvbzzo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2iwhnlaze.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2cafweixr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2snvtpwgs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nqlxejjk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wjnvwosu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xiywjzvg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2avcgetpg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2cmuwqgmc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ulxwlfnn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fvsbcfwf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2igsvpwae.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2snnkwgke.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2elxudfhh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2audxzqns.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2odpidhhk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2azjsflmp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dqiabdhx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ugyizdod.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zngdyvsr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2bxzaodyf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2syffbxwg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2owqfwddo.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2duvihbpr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hhtpyrzs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ejrtdhgc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2sifnziel.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nhuquehb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2uqczldfj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2fgfhdjwt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2euoyavyx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2aouqhkkp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zkwgvqoj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2pfwjrmsx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2mhmxmjpa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2giqmtgjb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wgjrwstr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2tnwlsdow.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2whxhbgcc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tnwezywg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mbufeweb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ofyjzjzz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wbeghtgm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tcwknuiv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2peqvfaxz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2skdumfnt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tavlhmnr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ycfgocur.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2stkwqyry.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2saulrcdc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwafhjvs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2daelpetf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xborztle.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qhqxalwy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nchptmvg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2utyssrxt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2xbekfeqj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kmlzkjkf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2trbezgps.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xxqqnqsj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qfalqqjg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ecsbannf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2dfdoodzp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ukzshsli.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2vsogompc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2zsgwwwcw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2tyxyglyd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ylxgthua.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mejkvcaq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zldrodww.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2caezihti.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2nwnehaxo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rnfzssgd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2pqmgxsgj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2phkdewut.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vflwbvch.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2afrojras.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cqvnamtk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vmkzwdjo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2eqtepqbi.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nhlvjjbp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tmtvweoa.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2amyvbdhq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2loedunim.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bpuknnmg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tnvqhodu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ceblijxp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2khjgxdtl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2knuhutzo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2hvtgwfqo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fmuximpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2udffrwhb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2oehktdtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnuhxbso.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2djpecolb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2mxifbxpn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2twcvnicw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hblhaide.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iermmlkb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymugmyfr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ynfkqsfx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2dmpesfqk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkxsyixz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2bxgtiwmf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2efjcdfjc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hnxrgipf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgohxufy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbfvoxnu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikzmajvy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2rbhqhlal.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ijddoqnu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zarrqqwi.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wlwmujjy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2foyepcvt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ujveppeu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lmaigwho.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rosiawnc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ichtpqhh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2oykbjtns.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2scqokoik.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ykrdwbgr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wpdreipv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rprrqboc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcrvuzys.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2szextzoc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2meyyvhzo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnvssido.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2swgqkgab.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2fhktcwun.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lqiptvci.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2zfdgpysm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2aoxwgnuf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2mcagtwmm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mceirfbq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfetxkop.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2eygusizl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2yywkteti.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2dkapviwg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2bcnhyney.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2zptaintv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2uuunyboa.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lelgaogj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ojcuudke.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ghwlhczm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwuvwjk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ppprnqac.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ucrwnmxx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ypnvbhoi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2dbmuuhxy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2vjhqvuwq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fulcrldp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lccapmxf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jemkeyqy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2hqushzhd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2wuwkkaep.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2hsapkkwo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tpcuxmlk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2cissjtal.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2yywrjpld.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xtkeiyiy.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2rywqesbc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2gzjphtny.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2dgemauug.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2wzsslven.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2readkxdr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rscusqjp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ixihpccl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2cwntkpkr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2mnjlvynj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2wmhbeczg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2jyatviou.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlatcgcx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2mvbujzbd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2kasdxnui.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2uvfronwu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2wnowqzeu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xtttksgs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2bhesmyjq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2dqmnxzsu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xrrwvkum.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2eeckairw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2exqqsekm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2zuaemart.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jgwnqryw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvztpeiw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ktgqtien.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnxckfjm.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yujhchan.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zanvwkmy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ubcpngdx.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vurcfmnc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fgabxmqy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2japxsbkj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2vnnvhgfe.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2agomceso.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ysfchgis.html


<!-- 参考信息 -->