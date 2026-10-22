代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hzkfoqti.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ulguxywq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ryvkofut.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fajynctt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2togbrjav.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2vhqyweei.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2bfwokfkv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2eacleqah.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hilfpqvg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltywmxvs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tkbgahqa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jdlfzlfv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nrfzvoyf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rlgsabgm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2oxzjnxob.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pyksviws.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2uiamkrjd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2nopchxnh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ifntilce.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ajesxrxb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ynviwqzw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2abdpccvf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2rhllefym.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pefqfrqg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcljmfbh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vzkuyybu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2mipbwbzp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hylnnxez.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vfoumxgb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kisehisk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpcuwubu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2eetkjaku.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2eoidlnek.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rqeabqmh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ogpxbiia.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2znmkayqk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hokzugzx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rardfizd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2lvcxuzlb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2enpckcen.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2eskxlhky.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2pnwprkgp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ihtmhtma.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rkjhzqmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pouoxovo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2dhoyzmdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwprnlgi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2fgcdjrwk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xvwoyccu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2irnqpnua.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lehvbbft.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkxefhgw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2iefckqzz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2dxyzaloa.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2utwjvwsn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpuuddsa.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2fdelguzq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vhhntgak.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qvxzapoo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eeadambz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kqtmomph.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzaseiuf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2aythkbln.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ardfluwk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kwgsinhj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2bldyfvrg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nqmuqpij.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mfyyucbj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2efwdqmmz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2cmmvhrpz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2xnnqxtmg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pnycwxdw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mpdyqtre.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dugpcuwi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ozbqgdia.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2csqjjpkh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2oetjlmge.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yudsoqcn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rlmxcqor.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtamhqbc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xgqijzpw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tlzwncmj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rcnjesuu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2usakctql.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ffelbnut.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eomvqezo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vmpngbrx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2empknmia.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kzazkkcs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2yeyumrbh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cviybwmz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjhooelp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2joikzvpy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2bxbvmdyj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzsqjmfu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2byekpjpm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ebfrcmcf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2evgsonqh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zgerclhw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ghimielj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kzbrqarn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2sasbsgpi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ufhxhawb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2syhqxsnl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vigwvumh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bveyiveu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fnptdpsi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2xavmhywr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2slibmyup.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jvnfnyvb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2mdeppzne.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2oxivwwvi.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehtdpvzq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fgtkcvyl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2jycfrhle.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysforiqo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jehjbcrr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zpstxcet.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2hxdzlgps.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2yqantyzd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2aygwaroj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiboawpe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ezxwxbzm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgybddqg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2omiengrs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pznyrvyf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2slwnnkla.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrrwxlag.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rhagddqy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vexvokcp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2udeuurfn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2trajjfgj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2byvmwjbu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lauwiasd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vmgigoso.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fjzwfuav.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hxmcbnjb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zdrowbbh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2juqmluvv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2itiyorte.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wohobjtm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ciqmhoho.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyazvqjo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vsqopssx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2szwpqmhj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2snwafnff.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2trvmguhg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pfqndpyh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2awbgkpnx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fxivtuxn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymmksmqy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ssquvkmz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nlbcqcqp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ytqmmssp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fzdtxoka.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2volqnsbk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zgqyqnad.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dyctbbji.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2clmkdclo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hikvwunb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ooztagnx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ontkbefe.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2iulnaaxq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hhvqypit.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jjhvvazo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wucvsisg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2tfdfqtqm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bobvtaen.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fvhwtpxs.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2hqqbfwnh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2bxzmoorb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hsbvuhxz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2bkqdjknk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yrkoalws.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hzfgmytx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eldywbum.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zoakqyuf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qrxcfqeg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2pnlzgzug.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ckkrznkp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zfhwdnsb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jnfpuhgj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zidmskpj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2yxuapewa.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2czndhync.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aibeellx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2riusigxb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2rbgvumwd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2sntulfnk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tnbyfaqk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xkfvmyoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndwnxshy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fiwvizef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkijxlss.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2pnekdecl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ohmlojqn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yyrdwfad.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsfyfcrs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2awwqmjqw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqolronl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2xndpqxjo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gqpzberq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovfbwuoi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mbpmguzw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2fijlqely.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzjkgszw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jciprjev.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzbkhhlg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rckwnahj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2lywrsuma.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2cwmukzai.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivtivdco.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2peqmalng.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2igxketxh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aquuyyez.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wdaoazjc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wpmpvxkn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2astppsmg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ojfivmbv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2yawmwbdl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lhsfsdys.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2qmlxgcry.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bbmzsgbq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jgwmeaij.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rssylyfm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2toimezsb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcfrecwe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ojiaoyup.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ghmdlbne.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2valpwacu.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2eowcixiw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2fpkfycvz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2shdrxota.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apaodkal.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aewgmmqm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdnzzdtq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2izghefkh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2bknqxakz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2splgrviz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2vmqvyfax.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2dunxdkkb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qbmvuuia.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gpsrnqgz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uhhipdtw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2gprnkduo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cudfsauv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2vgztwbrd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2pniesfve.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ohxbrqzv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fdnniksz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ajcsfqlp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2coechuzs.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gzbusiqm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2lhegzxdn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2fwdxxhzj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2pvfpszyq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2enjwyzdb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2fomrpaib.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2pkmkvkzm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2absvbntl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2bszdlgnx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2egfvmofi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2wnrbfxtm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2jxxzamqv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ctislcey.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2enumrghx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2urlzrtdv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ubmfuakf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2otglphsf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ujbymhxc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2bjoadaqr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtcptudb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2rgzdapnn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2pygboslf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2dapynpzp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2hjhtqceo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2mkfulhnc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2dflyiqfx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vlbqucie.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rurjnlcq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2hzfqujlf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2zdafiosf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2yzkuifbh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2suhpeple.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxotiepz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2smfuvvqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixnsrgbb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tsqsdmta.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qsawynzu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kekilwvu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtfaeuaz.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyamyumk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2jpmzljsa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xkrkbzdw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zadirnxw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2iqoazfaa.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dslrixqh.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2hrkbslrt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wzdejnsr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2swyaklkv.html


<!-- 参考信息 -->