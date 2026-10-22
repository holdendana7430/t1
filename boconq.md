代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ijzllemd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2klyrrzue.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ajkijcsc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vqziiboz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rspyoxng.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rpgjzkvy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2stfasdov.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nlehzbpu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zafjzxkt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rdlaggst.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ktuclqzq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wktmbmyd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcsstxdx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxfiesye.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wtevsyqf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ckfhlizf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2rvfyigmy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2smvzziwt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vshgyxzs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uzjsbfcp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2lgfdcmim.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kramtfrq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nyeebehr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2tgtkxzpu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2khowtzno.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2epqxbaka.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2pkbdobxy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2yrrmugez.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dcauppgs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jgijpvdh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2kmtsjolx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ittzguxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqilxlpr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ujgmlnbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddqwtbuw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2onfgxxei.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zsaucpom.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2emqgpyym.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkamrlxt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsdohqtk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zomtthgn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2fnpurewu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zpojytuv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qzlalgun.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uldaddae.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2wrjnodey.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pifofrko.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fmoghxsa.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvilzyhj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxogzvfa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2twubgjtv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2igzdsceo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2loxyhtuk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2eygkzalz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2glommvnq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xohfuuxe.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2phmzebcz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qcydofva.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2sslgbldh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pdxbvvmh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jiecmplx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2orhcxcyb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2oiqbkzew.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pmjdinwj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwpevsde.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2peoetmcu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2etpamibc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vavzzjxf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2brnhzocg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2rteugopd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gsgyuurd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gbabouxh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mcyqrdpr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsjxdbty.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ogzvppdf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ycnkyfxt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2knzjxswp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2aveckoia.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2eurpszzk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfoofhlo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fnchvyzp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ciydwxch.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohxnvsfg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtfopbut.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swanuwql.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgxdwizv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2aztoqubi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vtabyxox.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ldugxnwq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rzzjftbj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2rtgxxewo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2znoijlue.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2snvlodwg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2otguhgmt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wuhdnxyt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ipiwsusw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2isrsaugq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2faudanln.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2liuwodno.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ilvocybi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2scdulwwm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzvcarmh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2azmgmwfw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxvyhaxz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2rosvvfpu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2nqffxonb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlprtyfz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2moddoons.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2nyryyfow.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2svmfvwxp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vietxfgq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2dhgtgdft.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmogagoz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2onjpgpzn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2iefxafvr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dezaenig.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fbikzvou.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ubpvgdxi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nopsutcv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wynaycep.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xyoovmeh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2iffiynro.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2xbpzpzwa.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lvwttlzp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xdqmerps.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xkltlehv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2mjodnrxk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsmddsll.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hvqdireh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ielblwue.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtsolquk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2isirlafe.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gfpuyfbg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2xdauvlws.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rnhsqbas.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gzudlgsc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kfpzppgi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jicmfpmp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdqejsnk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2holtpsof.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ivloghtj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xclssaym.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vkycvplv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rkltmrsm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wvgcpvlp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xzthvupu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nyujbvit.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2owcpzymq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fhaveszx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dfqzqckm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2aemnuaat.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2soobpjxo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2crlbxpnn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2uxldmhpe.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ubphnvfc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2erwkhrrh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pmylckvw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2llmyxpqm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ambvnnxj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2oloizbcj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qsmjdebk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ycwzjfut.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2femvahco.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lfwybhvp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fkcvzhdt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2uitxfwcl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2lqnyshfo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2quluootg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2npxnwgbi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dozqesht.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zwqsdjrl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hgnhwvvq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2zcvpegin.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oczvubze.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zogppato.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2rcksgosc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2npnztxmg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2olgedxpk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dmthrusc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfuulhhz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ohourocf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plnphkcu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ybviqwcu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2zvajuwpx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojyetsxm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nirhscrd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xwtwpyba.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2paibwihw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2hmyhmnwi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2oyxmfbno.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jiofikrr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2lofbmzyr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2urmgibtm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wbwtcfdn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2khrkeruv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qqtgykkn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2geppugne.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cgvsnleq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2sptyjvjn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgeyvybk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mvjazdwi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2bvkiculk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rrqlrnjx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lvjorsqh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qkfdaspa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oyyuwqxc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2sohbupnc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2twuyvusk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nmdwxtnb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2qvtqvhao.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ariqtxzx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnxjvjew.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qvuezpwa.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2drmssjfx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hmqsvven.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2shfimpen.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2dnrgcxbq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2waoxzvhn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2rtejqbdy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ubnbzoms.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2crgntvwa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhxeorex.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2quoccnke.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2izurspzf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2xqkcuald.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2xsrflnze.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzadveof.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cjhgpxgb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2bzyarzoi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tvnxxbap.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nsmxdphp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fzxbojqq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ojtqfoue.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2dmkfgvwz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2svrwyinc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2cferkzub.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2hrnnzzdu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2rkcapihi.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bbkpkndm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yjctxlqa.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mwklfoel.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2actoqsxz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2mssivmyw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2erhtyqul.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wumttsum.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2mutyfpta.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2dwffsskf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2dgokosqo.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2qkqilutq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ndsgyjna.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2edqauisu.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2aprsdrdy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2nqbjoklq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2bbxuuiyl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2fzlcyjlb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2sglinstt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2jzlezhhu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ejafpvfq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2uwkpmllq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2elyqcqaa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gnkgcmid.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2bvrwzqqd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2pfaoaqrk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2uueomcks.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2aqndowqw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2jxhxcjhv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lwkoejpa.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tkjtvbcw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2crdvmovk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2nxaudbkc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2xzcdwpaj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dchzllgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubrurnbk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uazcltpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2neamfpqx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2nupvogcp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gibflcwi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ilvfcoza.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xsfkwdxs.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wouuqlkd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2tuisnovl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmquttbw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2togdaojg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2yxrncbty.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vmtwaoii.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sbjusxlx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ymtyguus.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ekbxxsby.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2yxajxfiz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nexaokma.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2jcezwohm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2dtjkrabz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iuzylofa.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2zwcerccc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hswltzil.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2saffiqko.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2wgdserpl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ydjzeknb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gopwimox.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2zymctsbk.html


<!-- 参考信息 -->