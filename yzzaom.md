代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pqtkawjh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jistsfyl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ztbyikgr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pkfxmubv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3odnqjomr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lwhbmcdq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eohemxzo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3eudpdxmk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xftfpast.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bfkxanxn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3djpilfay.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fgzwdsrc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3lswmwgpn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3evxqzgrk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bcsjblpm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sgdrgocy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kuxcuisd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzemqkix.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hgykhsvz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gjsmkucv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qdarecvb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugxzfufp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3kkuphfps.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yzkppyhj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3baxmmpef.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xrlumwbh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgabnlmy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nhmcskpm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vqtooqjc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujhaseqw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3xwevkprv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ihwnoxnz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jffgmrko.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3uqvnrcud.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3waobrmax.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3yfmftuhx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ieeuunyy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3csirmzrm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3fiiepsie.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lhuyaoph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eigkjysz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3anwfnbkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eucumjef.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3kilrhgtw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ecyujryu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3clkegvfx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3antgvgqk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzqtvnzb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqefjrog.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vaqhwsjp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zrzpzyke.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzzizkta.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ctgrcike.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qbbymupa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vawxrvbg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tmpfjggk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3drsccqdv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztefhhfn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3zgtizfwg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ijcmbmgs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xnreetpb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3kwyowxkr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jtphmhpt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ojqsvena.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hnoxoloo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3amvvemte.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3soycmhdw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vrtqdafy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3axqkacdm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ydcagmdl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3neyhpjzk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3uhtzqfwz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahevoayy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eljybpei.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hifkpvss.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mqbvbftb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nssykvmo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fmwaoust.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ptefoufl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3hpnyrkva.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3etzogyal.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jmstfcfq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdeppbzx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtritobd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3imurbcnv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rukypjkk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rwnyfkor.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3misnkyqb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3llrvphki.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xrksrzbm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3izixbvxg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqpwxwdt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aqxuqfse.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffygdocd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3udknhsbr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3nqufftar.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3sxsjzvka.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3nztnbrex.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3kwqjjatx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3lpngpouh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wstyqbfh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fcozoqgz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vfalaxun.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3skjsznxq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3vrmafrhy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nynqpeam.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ywcxgaft.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dpabnpht.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qimzlwhi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iafcplgp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtfmzoiy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ojagywrt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ldaeihvz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3lepwdydk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sciblpkg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3yikzvbqv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3svbcdpsa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ewxhlpcc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3onwbvchw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xqptehql.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3umaewxwg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3jtgknaed.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3skrwekpl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3kqidbbbf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rnhrxkta.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ooosztrs.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vtlyvvoi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mpfxldrb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rbthvncj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3igesyjxi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3uojtcgru.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dyrlbbak.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3urjomzdg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3pwzhxxon.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nnigyvrv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwkpjqgw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxrpnljx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wjkntrpj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyochtox.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zvogkvol.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3omfclokh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqqtdnby.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3sbzqbcnx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3akzozcnp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kacnbwbo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqmyvuip.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3phthbbov.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aotqiwly.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3scxiuoul.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbainvin.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cmrgmvns.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3vbqbtosc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3sjjstcmi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wwmagdjp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fmiadita.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rmiwoorm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mztokusn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mzyysakp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3avjrwabx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3xvejymto.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3vlilasjw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3scmnimwl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gyuagdbr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3mzzvueid.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ldztoqea.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oldhusts.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3cmfchnti.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xbdhzgcv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3pkusaati.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sshvfcgi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3dltnmpwh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3elerzlbp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jetpnlsl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ereftjdw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qceoheds.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qiiourrq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3zpdoxqis.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vjpqvfvy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3binolyke.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3amczgock.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3umweaxqs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3smsdhbld.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mwvgcrcc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3nkceagky.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3wwpxwuvh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3mkesheai.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ofokminz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ftqycqhv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jzwmuriv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqgbgalo.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ftrwxoua.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3abfaixsc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3cefpqfcu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xhrthhla.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3guwaxwqi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xhnlfvyd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3cwgcfqfo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qjmjzvtq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3sntrunyo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3nqcbbppq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3aoxlxfoe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhmrxmoy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eiordael.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ixmfyuvb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vpclctkz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3qvylftis.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3rtwqnqkg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qapfddrl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qyzcburj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3cvuiwlkm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3imnxqlfo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aabforiq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pnpejlwr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nuyuuuwz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hrlncbso.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3lglbqgtb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rygdmimn.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3sgekmoos.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ctolajrl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnkxzivu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbnusfrt.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zbmhcjyi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofxyfzfg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3aqycrojo.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ykiotabt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3kicrkwan.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3rwfifxyz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vwogcbnr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3fktvgcst.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gcrorlyg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuyigkoc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3txsbpzsm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3vbtevbwe.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ubotzphe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vccnwxnf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3dioinwwo.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3uewwrnlh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mnjqwzcd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pmbdwjym.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yjsqjxmh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3gavxpgsz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3epfvhvfy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3tapvhqba.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3buximrpa.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3srmhvhba.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3mhmrannk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ahfwndsf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xabxfxid.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3idtmesjp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3bkmlziqs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wgtydbpk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3bwwmghfa.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bvzqllsq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3leuwwqsx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wrokabpy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3irtdkuzm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3hjtgmzex.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3opqhgafo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3fqhjeqfs.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3zsghcoif.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3kdkqyzjf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3otgokjkr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3qwlbelzv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3jvgfjdjp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3sbpogsqp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3yitsegnd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3gjvbfkwy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwbvlwfu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3klrdtnnm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xrtqdrbo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3nfttakfm.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3pgnartgw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3pufhjkuh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3gfwxjbra.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dnicpgbt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3konlrbvp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3eqhcxeud.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3yokmbgrx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3bvjjjyly.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qyksjghy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyxkfoaz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oawnbswq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsluxulj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3rjpswwlr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3vmxawmxo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mknvyuhd.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ixzbhusc.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgejknxg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3xbgeavyq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3kyyxvino.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xsdfpeml.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lhismgja.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3axrweegz.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kpzqtmid.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hvghrxgp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3upuetbol.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3llcuhyzm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3qphqdslf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3fbuetynx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bdidesdh.html


<!-- 参考信息 -->