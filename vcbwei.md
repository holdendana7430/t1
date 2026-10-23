代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3wegxwdun.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xhcpgibj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pznwywby.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lomgmdcg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3pssdoeqo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3epgkruyj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3rohuxlzm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3tykebtme.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3aeikfena.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qvovakab.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3inlglkyu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vgaoaxvd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bfkhetwx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cahdtwxm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xexfpvsu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ntbiaoyb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3bycmprua.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mzzfvfnr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iyucdzkv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xdjwodyg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wsexiaym.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xdfivpgw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3snibxgyj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qiinrbdh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3nhezchhr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ufnrwshs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3enzzjkop.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dhzasnpe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3enkohqaz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qhnsyieb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jcwdawme.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxifevxz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dpgpthhr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zcmpivdg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zazphtug.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgghdxjg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3onazyqxq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzswnyme.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbajzfsc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rlpstfgx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3sqjlkmat.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zqkrwxlh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3jdigippk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3bkfvlvwu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3eqczmymz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lframlet.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bkqeyadr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jaeutjal.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3gvwiythw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3eassthpl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3wczofotj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ilsmsisi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnposuqu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3amalpbac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqdfyyuy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wwgcobzw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3vrxcmeqi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ycmddoqs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3eyabymev.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3abfcnupy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xactsaae.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bcabvhhr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3gmkbmpgf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3roljyvpd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3uuwnchss.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3uwytyncu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gppjvbaa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lskpkhju.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qddwpnjb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vcmtkgtp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3uqfbiwjo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3uicatkvc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yiloljgi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3anxpiccs.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3syoipphi.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ypcgkexw.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yguhyawt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rrwgwyvx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3junvcfrn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3gazzuded.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3losnebis.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qnhxqzmm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3jbmzxykj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wrvhnfbb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3epwbzhpe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ndkxksso.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdbyqadi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzkcimwl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mipgcjzc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pbzypjol.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jzpuskya.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3hzytjnei.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3edcqequr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfxnukbp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3othhfdln.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ppxcjxvc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbcoxkbc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3blptpfsl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wpjizprk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnjizmzs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3tksatlzr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3msmkyqed.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sxcgtohj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rnuuhcna.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3riobrpnv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xgyqweow.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3kwjkpwbk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3dtkzhzua.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3jiaidrlr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3fwxuzkdb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3soewmjop.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3shpxlzex.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3snebtmlf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hejsqczi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tqngkias.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rkewczrp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3duazjvaz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3acrucpbh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3cboishhs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hasifxfn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3dtqqccyu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eepqunyc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ixevpbrf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkcgjuan.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3uqjogmlz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3dhrekxpl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zcypaeqq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ihuqtgle.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wbhszjuy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3qbkubocm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3inxyxmki.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kotuhkwj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpkenbrp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xzlnwzvz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3lspkevbb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkhxzhwz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3aepuhbto.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3jmzunukc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hfvrjpbq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3juvkxhed.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qgerntxh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3rdoivktj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3bqymtppq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nsjbtzxf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vrqsntag.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3tlkmlbxv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3uvviyvar.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3acuovucc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtsmvucf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjhlogae.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iteurvlp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lhbdxyjr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fisskqyk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3nllcvvst.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3onjgdqnm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wccpgzlu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggyzwfwv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qpnvzirz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulettqgc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3egrhdkll.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qwarwbfq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ekddhxfn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ewdkrelc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qcafsykh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3vfisxqti.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rhdvskjn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kbaoillb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vepwjcog.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3klhwkdbp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3gabimiox.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wickmfhz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3rcjdotgf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ktdbktno.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3hinpfvek.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3dbddsrzr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ilpdebss.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3upljbrpw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkfwjxgc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3cmnauqvy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3fxygriog.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3oexhvmvc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3uciztphm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3przweras.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3etlfbquq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3dqpcwtry.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cghzmwlm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3yhtfvmvn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3amhonnic.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3yvaiatcl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cghqhxcx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3yowlbohe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jwqgxoie.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3uncotces.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wcqzmnyg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xfkzyxzs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3rzlygomb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3yuiarmmy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3gatazaqk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3oslmigmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vehhwhaz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ypaqopry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkvenqqh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3depvwnbe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3lokewurq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucjbcyta.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyukdpru.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qebpecdb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ukojwbag.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3kvkbwffe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3olcuvkkj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngrpuqzf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3llrcskmk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3kqxtmdlm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hntyfwrc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3huhjxmgd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yaynvmhf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oaaivjgl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3cmbiyqmo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3uqnzosqe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bokubmii.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3maxbvunq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3erufisys.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zikjzoyn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vxiqqvvm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gspwpkyf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tllympym.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3fehauxti.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3yrrmswcv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zocsafrz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3uzowkyac.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ohxpsyjt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xytxxlpy.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3csjtxphs.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kiznlbwz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pjrgcwko.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3skoygnqk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3henauvzq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3vedembto.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3xnvssbii.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3rcfqsujj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3cbpzktzz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qtorqjcm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yexckdwx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3moojmvut.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3sprtohwy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3bmielerh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhzxgyah.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3vjncmoix.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3bzfuumir.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vpltydlu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yjxrbtje.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qycortqx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3vmbwtbrl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3awxwwkuv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3qwnnbapd.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zktygrvj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3wmsyjjem.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3uztnyyrv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jhoqzzvn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3idjymlhx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3slxyvekg.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3tqrumenn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3hygzbajd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3vyiexhoe.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3leabkzgm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3colwygwx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3pxmewllc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ezqsfhgg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3kpdmlqwk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lkaapnhk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3xiennpal.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3yznfzgtx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3whefaerz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jwxqqizl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3wuneijtl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3zndiskuw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3juqmsuba.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3hcvdiftg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3fhqkypfm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3udpretlx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dfdotkem.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3rehfymsr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3shyfskyx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qawgbsmt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3yrgywkul.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3oltahvvi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ajbroudg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ffglbpua.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3wzpbbbbb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3zqagdxtt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3gdchkqjw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3izmtgycp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eggharfx.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rwgdostf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyoyoxrs.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sppuvlad.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3crowvznl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3myyozmcb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3nsxnupjl.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3biybhzod.html


<!-- 参考信息 -->