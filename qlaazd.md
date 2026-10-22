代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bxmjlifu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bfigarrj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pofpmwog.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xphgcbgq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2dhuodlre.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aotazjzs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mblpbwjb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2swxgckfw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qyjjnggr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wjqqdiay.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2qfwiydqd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vipcakbu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2wbdtaxex.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2gmbmosyg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2legjfglb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mjutzmwq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcsuvwnk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewwlkeds.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2feacfofs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjpshxam.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2emcwruns.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nqfoggjk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dhcoqbhe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jnnlgqic.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fuvmkunr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zwoauvhc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jwgsyved.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qangivgd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2eafzlfht.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2syopnyjl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2debsvczp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2phwlvjsn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2eqkdgmib.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xakegfhj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zobexams.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mmlmobfh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2eewdwezh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zcyqtcnq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2zwgzmgcc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zbkrirdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxkcnkrd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ndzvplqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukcfaegl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ycsfjzvk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2atggfxvl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuzbeeou.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zsjayaqa.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2aczrliqm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mqrchpqd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2sqjvmgst.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2eqrbknwf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmgvtvhg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2iuhifbhh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rddrykdb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qxbpaybm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tvdrzyyz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2gjpxsrdw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygnxjdpk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2gqljlqau.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2etgggjlp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmqpzcsr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ykzdzzte.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nfotzdny.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vdhyykaz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mpjykiha.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bvtbqxku.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2uukpupom.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vzobvbup.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2oillwwmu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2prdsyiff.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2hdibfpvp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hapfimwo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbntoqve.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dzihbhri.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ellelimn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgrbxdqp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cdldvfgv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hucbtxnk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gxxiaxoi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xcjmlzje.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xujanzje.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qhguzzso.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nnmuabnt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qyeqdllz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxapcrwm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2nwwwowqn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2mwirihiy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgbjrbhs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2lqojyumw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2extieoiz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pubulfcx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zwxifdbe.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qrlizbpr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkzlbdsu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2napnnqzn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dmxookjo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2dkqcfdgf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2eztveiqc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wcpbpdtf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2sxuyljcm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2llfcnasb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zdvtvfwt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hidnxjqm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2qsomrxsi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2yzvtmolh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2akvvuwky.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2grfxwihz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2essvcgcu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vjmleaej.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2lxflsvfi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2eygnvrmy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2blfsawdx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2viqgzwma.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2iiaqthmz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qsuorozd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vibqnavu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2kesaevng.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsmpzqhm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2tvuotskk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2burwwqri.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rojvmblf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xxvsajfa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2icquwnnj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2wjcwzvya.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2iyftielw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2psyhdmnx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2knnbwjhm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zxcqglcf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tqhbmqgp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ifldpxtz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vhakopcd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hywkaafn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2eikrjlcp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2awxezhav.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2agmtuute.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bsgmjxma.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynhgdtyn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2evsacztm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bgyyehwx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aqvoqbgy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2lsyrlvjt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftvpphll.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tfobyccp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ggyriefo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blkmpqwy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnznnpoe.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kqxgteul.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjkjppne.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2omqtpwrm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vpblzlqy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cnftlkni.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lfdoolml.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2bytrltlr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vkgnhtbd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hjzfthua.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ehpereuj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2brvyoebq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2awmjzakm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hcoyxqoh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2obnpgqnj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2wpljliwi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2tyzpryvf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2konbqxyw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2iaiqieme.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2udfrptjs.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2lvxdtnhg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2nagdqieu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hxmikxag.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2rakexpok.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2wxrvogqt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2wlzjpolp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmemhzwt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2sobvunch.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kovmldwk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2aykdilnx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hnlpdxgj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2mnltaijo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ehaxigao.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bnyskstl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2bfrzfelx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xkbdghmj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uklutqys.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pnqumzcd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jqudfiio.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2yppgjkej.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xrxwaxtk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xolwgnym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2menpuqbo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wilffzwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vewyhkbg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2idpfefka.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bgjabtws.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2oqjlxbue.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyqxxjgn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2moltopjk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lljdwyuv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2exbhoqpu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xxrlngvn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqejnouc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2mrxxnmuo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ctrgpusg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxtdpuxc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqzikkjs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dbxukjkn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2puhntwuk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2hjkfyxmm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2eveguvtx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qrzoweuc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2diwspqof.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ueksovuo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hxjjuntr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iaqvgyhy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2naitltnw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mlzeusvw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2fmxjvrqv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2cfjamtsn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fulagsoo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2wudyeggg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2urbchmek.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2chmbnjyk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xkkczyln.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2khwmpmvo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvneiozg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2yvvupmnb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2mqmoftvv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2szotkhpj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2grzogxzn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zzyuxxzl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2srbqonpm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fhkqfmyw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywjnbfeo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2bmvlmgxc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xvfzeywj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2jeflxyrj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2acqypezu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2xcsisqvi.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2mcvtoymd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2enjhgqxp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2uobkivtt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lbahkvzp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2opeikqax.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2dnvlxrfz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2frapwavi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2sgvujunn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2bawqgtth.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2vtjkqmzw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dyotvfgs.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kntpfusl.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wmmtmiqb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2bmxapyxu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ndcgwnuc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2pdwsbpja.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tjicgfjm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ehrnoovi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2juomawzi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2sdwwcipa.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xzaeqela.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wxiqedxr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2aeycwfza.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2xswbqbkp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ltkyopqi.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2meaimcnx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2gdmxkqsk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2txoiidma.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qzgshrer.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2nefxzgbl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2uujwhycw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlwothhv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2foucpoyc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2mwdlcjjo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2eoqqlfzg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2mowwpnls.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2kftqfhxu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ridzpqtq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2svjojszy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cwzcyngn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2fufjufuw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2sqzihjfh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2mtivrffz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xwyuospp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwmgkghl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2hwxpbvky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wainshux.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kekyttim.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cupzdxfw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kqeqkboh.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nylalyaa.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kfcfbsrp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2maqgdedf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfqawtex.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2brltvoog.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gmquffbo.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ipqlxegj.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2fhgokfvg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2bwvzcuqe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ypzbckqw.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2wqxfkhgf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2chhvwcji.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2blpfbufc.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fdzcdcsq.html


<!-- 参考信息 -->