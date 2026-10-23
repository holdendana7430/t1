代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wfnwoipw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jjtkfqih.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jhhxgtlm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hmceagmx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ffgaijce.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hfrqdlpu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ovmhowhw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ldlsalqp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3jkhmnmsb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dennxids.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rzhokrwq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kczjnwkv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gshnzxai.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jrypyyxs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3zxmrqfpu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uxiyholf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3caqnacid.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qduedtji.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwezovmh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wdyyixxi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3acldmtcv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oyeclach.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3yjmcrhpr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3abaxvdhc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htozwrxa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cymrtqwn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3fixrnjdz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnxoioaj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nqfxgrmp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dotmqoix.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uancquvw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbqinex.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xvxnjdvs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ylipmpco.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wubqxcer.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wppakbkx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ispejaco.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3clhravdz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3xrljmzjo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bxjojwgw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ukrlwdpg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3cdcfjiie.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ojmppjsh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ckojwcbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwctmzfh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3lvqmbfip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvalkucn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3krbxkcdg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3cqyoajql.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3obvklahe.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rezilydr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3uudyjrzr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3saugqgmk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ideqdrql.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rwbddujz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kivzuuqz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3yrvalvqv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ftmejgsf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3etfxepvw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dylyqyob.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eioyruoo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjdkszot.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3hwsiwnml.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xwfhvvxb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mpoeyocg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3afomlfav.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uwdzlciq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xkzgorbj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3aeysglaw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gjrimtlm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bqrhqxlu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ciayucpr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mivnlbvm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hgkqpced.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3adzhfhzv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sgakwuil.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvibdikj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zuvrfgxr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkbqxgle.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gqpioksv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hpckkjrw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3juwnvppn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3iysimsii.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dtvoccmk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3asdarraa.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtwftwmt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pfypmubs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzgcfbvm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ukefvscl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3lsbddtjj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ukahpqid.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3rrirqeoo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jlqxyelh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bbsfsklh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vxutfhmp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3citcprti.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wdereypx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gajifsmn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3eqteevur.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tiwuajkq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kaqpqlnz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lfmwtusr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rdonwrvk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3znzovjaf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xoowmdcm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rjswdytg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hxldychc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qeypybfh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hrbucpyk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3chxfxawt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ghnlzpqg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3gxajctbq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3anvkangx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kngfatst.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lqswvogs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gukpgvkc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3pmztzepg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3xdwzuwln.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3alhocgap.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3fggcdnov.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3sopilajo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3fqvyuqki.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3bndofclb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rfascfqt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3scqjosom.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xybnfxko.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fugcanik.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3yeclmxto.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3patiplxi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hvkdlvkp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ffqgtjxj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3isydtvus.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yltructk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vzudyyrf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3hodfesqx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bujxgdsa.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jnfgjfst.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3smuslvfh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3weqscupd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3obwlqyor.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmflguzy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hazdvydh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zciumzvl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3szbrauzn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mrietqic.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xgzksggr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vzmfbnih.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yhyqdkhu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3sqeaanpv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3peczrjhh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fscftrpo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnuvwzvi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dgaxxoye.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wtccsbvb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mtlnzphp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3otvtljog.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3tnuzawwa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ennwwjlx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wbmoitlf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zfovfcdl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ekxbthni.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qfefmnjs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3rnprrzuv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fqggflgl.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3sdbyazik.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3nmpsztsf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rvnhlpra.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3vqstjjys.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3gqiotqje.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsmeijjf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ugjusbnz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3fgxcbzmz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3fshnlesi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3pujwbqhq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3pywhcjgc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqziaxpb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nklbmqfj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kiddivwm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3oxvsncxv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qweiddqa.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3bnvxcgyd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tepqeavl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3xqxxdrrv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ohjdafbc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3nvlhotly.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ekkgdflq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ldstjbuw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3qjgsxrra.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3tczqvahs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zwgahits.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tnnvokgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahfatcnu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3sonuoprl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejnanxst.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3dfiytbet.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3muyjrjop.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwesqyrp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uhzdhtnt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kntmffvo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhnxliue.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wksvmilk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3lbgafwwv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3glhwujep.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3efitvzgx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3wakvreav.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ioxdizqv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jdwqtlwa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bccomtgq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eyukcexy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3xohuihxi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3gpuqvfom.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3evnbkegu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rafyevkt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3qqucuuje.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hxmdfzgz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gsavqwrs.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cpnaltzo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dygteids.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3emkhngjn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3sardzokk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bggcowqm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3euvbrvrw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3junwwhvq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ilkqvsow.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3loiplsnz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3occljovt.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdkhfofd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3raelkcxu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3verknkyx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3jhclwzas.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3hievdpue.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3uxcalkow.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3nmteyzgs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tcaekbgy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3etfhicxj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkppxspf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3fnytehlh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3nsxxfrrv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rtekxnzd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3puunhjuu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3qdspezbp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3idjjbbua.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3whfolpxp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zpgiyhui.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mcwcrltf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3vbbzmlpa.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3zzeldilz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zxkuvfez.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dzumbhnv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3foccygxc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zxnzcnee.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3faaiedmg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kpwivapy.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3letsrwwc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3dnjvkbvj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3fmqudubr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mqklyaoo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ogxetjdg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3nzrrbddz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3jewbrfdc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3wcdflagd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3neunmiyy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3uxoqsluk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3vxqdzqro.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3douxycps.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xgvgofkm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3lhvnpcem.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3gtkgfiab.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3vrgzqekl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3drochdre.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3tdhfaatp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ztrfbpuz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3xtzndoec.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3nkapyzbe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3izxpuqjq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ohqflnfc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3gvgdilxb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ngljpudt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3qyjlkals.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3biswhlpt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3wjvvonqs.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3qehnwdat.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3nivulmyk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lzeucdlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxqndodl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3pnsskegq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlkojlhr.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wgyexltk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3deypevoc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kjlkrqxi.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xrcwquky.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xqxaofgw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3tucvyhqj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ltrnhqli.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3titgjvzb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3szzcwesa.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3dhdolssz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ptlukgqj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3muqmwvyu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3hpawmzaa.html


<!-- 参考信息 -->