代发 wailian999

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3evssgzrb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bhhzvrav.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wzrehikb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rpykdwwh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nuhohyic.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lqwbazyy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wkbqjieg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxirldbe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3fzqmtdyo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3gacjgjyo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzmexdog.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lnfgpeky.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kowjqyhe.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3henmkpaf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qnewjoln.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ogcyfnnu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3spqgzmmn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nlifbfna.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wanwrowf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qgyybvqp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aoboaghg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgirtmur.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dkbnvejr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gtdtfglf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3cifhhbuz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gjftbnpi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3duoefbcx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wfeceebi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3clowfjbo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ppgpjjnt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wkisyray.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3tlhglpxn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3wriefqwq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3oggwvihz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lhmyhzkp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ocmgrwdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zptxvmvb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3xvsfjwim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpbvudkd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3obmmygmf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3cdrlzijl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3pyyeyoxh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhkoayik.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3enhptfgf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3exahkxnf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gxefgmyg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yafhrryi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgedvdjj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bpggljcz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3fcfjfnnz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfgdfhfw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3owcsozhj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aarzqwbt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utklelnl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kmhlknsp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3scgdjdfi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dusaemzc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bysutsbf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3opaeuhns.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fasgnwzo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dwmbuqet.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eznqocmd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3dfswgklo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vvlpsmah.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kjucibav.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dmweqhge.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ncxewzvv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pqsfmaxu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3thufpdwr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rqimcbbp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xhfgnldz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfakmcnb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uhuifama.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fpctndoh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jkexrnmk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3adfmwstz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3fnvwclbu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3teoibtne.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vrpdfmgd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfrougwj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kxqcowhv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3itfrbbpg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3gfiyjmhq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3uzinhrrg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3cgaamyiv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3wntnbaxz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqfwjjkc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rdisvlwu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukpugzoa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3riornmmn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xjmdseuo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3knvhigfz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ktjpaakn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wtqcdtvi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3mogqxfou.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3bleumzeo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3afgeppbn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3grenqdvd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hwztckos.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fdsyxmpo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ogzqgysl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bcupptyj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3umwlmxhb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vnomslyw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3dwgssgzd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ncsyqkme.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3yywymluw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikaqfoet.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3nzqgwhco.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3altoiypv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzoxdbcl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zmiekidw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ovriqwgc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wsxxekfe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3esxcbity.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulqsgiqc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pioytcfn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xlzorzwo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3mvpoirdp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxfgjtny.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rihocviy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zwyiiifl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xnfoxpac.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kuvkslcc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pyuucmzt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ycsqddzn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3agwcltzg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vohfnwyo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3duusoomy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jbpckxca.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3krhsyxvr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tftknswz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdjdqqta.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kokccagx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3adnkoudp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hrrrkhdl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vbwzyahz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3muusxoyr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3holnfjgz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xchoorgq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3apohcmsw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sjenxssw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffetnfee.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mvtfrfta.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3perlggit.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zuylgdbp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pshobxhj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gfcesqqz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3prrxqhme.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kzvwogjw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aaayccjg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3iandjmga.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gpncuwhb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nyazazfb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xpiockat.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3znepixea.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3steehufw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3vuqcbugj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3nyiwxfqo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hpbarxpi.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3uiepdhop.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfqhrvtl.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3azpwzakt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3knwqafdj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3blxhjzso.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3timgkflj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ufhzsgmt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3umwnzqtz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3grdjapeh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jolydemm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3swbokwlw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3esewbexb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3essbucie.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mqidrsct.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ympohjty.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3deofvsvy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hwcukneb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3akvvqshb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rqqneqts.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3oufmnvzq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3viiofdyt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3xjvkalvm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3txbonjpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpwvsyxg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jyhrgrgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqjarxho.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ogffcghb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3jhiuujfz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3klwgbojn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nvyxmfzs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gaaqkcxf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmjacekj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mlbhchve.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jltuutzj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ivpsrbwl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ewexneep.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3drcbcfex.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3euvvdxwt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcigchzw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vyswhmwu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3upievrhk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3roqahlcs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3wzcenusa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pfzpuqac.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gafxgmja.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3locddmud.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3efppmupr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fkahudmu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mwyszjns.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jysmsimi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3unwvylll.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ikuzfhdu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xlgadcqo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3tkecznrw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vnbmhwgt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3cutxtrpv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mbddczyw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wwjaymqm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3oghlqnxk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3qcmqndni.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ioafemkm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzjtcvtp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3esmwndhc.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3yaqedxng.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3umexvzmn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3blfezxdb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rykaprav.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbujgaxh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ggmujjrb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xsirwtrg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qrxtsnjv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3kbugefrb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3plcjntec.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qpsnwdca.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3azkaxmzs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bcklbztn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3jfzuesex.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ecllbefs.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3muoyoqdm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qzswmrsj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3pjprzogj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3cebhkaxh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ouhnrycd.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vpsnjada.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3npjtmasz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3btzmtqco.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3lcwnyhyw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ygehqhjr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3eojasdmt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3chgedlxg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3erabxswp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3oiysffrd.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3zfsrwuym.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3uswwcceg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3kogjepft.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3usxfaocq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3aslgxlbq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3dtcqcjnr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3dchfsinb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3dawgbygy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3egbsvkvn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3rwnggyit.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3jmecnwbo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3gazhyufq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ixqksjxb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3iurwpmjz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3xdzgfdej.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3plfmiidw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3dzgadlvj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3usyzdewr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ppduvutq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vksvjidn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3udzqsnmj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ekssfbfw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ugxhawks.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vaoproqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfqtsppn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3wtqlnrks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oraemkdv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3zevqrtvs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ybptvyoh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dfjaiahl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3osiudxyt.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ourgwtib.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3gpprfffp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nzuscqes.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kwfwkuqa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jfyhljuw.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ibwkrqxx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqovxoaq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3kqplftgc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3vawdgnls.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3zkdyasat.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fppkobbg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3rrivuxmb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bxghhigj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3htnnrbze.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3joojvdcg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3spxcomtz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3wxbilvty.html


<!-- 参考信息 -->