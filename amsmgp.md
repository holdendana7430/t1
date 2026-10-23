代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3brjsxhdg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3fnfwumob.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3avprjfgg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3daimdqdw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jsdpgcpm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3qhjykmll.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3onskrxtl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lszljwir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nambqsfj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3fydxpgnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xpjqizui.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hqhubfzb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bfpsxbwh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhjjavtq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkxfpxwr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxtxhsyi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qfvjcvpo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ulhxdzrz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3yjzzzgtp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3evauomkg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ggbkqqot.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3blytcyry.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vakmofyn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vmfajdlf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xogmzyaj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tbtydzuv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3focilpic.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3usvoffqg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wgmwresr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dztjsofb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ltahpogy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nesothgx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ixmcbhuv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dxfmoxpz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hqevvekt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rkftbblh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fwkustln.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wrasrwij.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3pmcwixot.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lajpgmdp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gfatanyw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfbbhzte.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kjiybecr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esahreaw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jnjdiljf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jtimiuxk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3yxeaidct.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3woshaeys.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tggvxaum.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdojkgav.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mnmwdhrc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mggobzag.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iniocmxs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fkvqlztn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3irtaabvt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgywpgjw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3vfsfviyf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3msbpmrnv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oxdaqfwd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntomubcd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3clfadzrx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3niugubbc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wszzyxgc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3edlvthig.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3hhmfjbtn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3yrlbsmfp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ffnsqhmn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ubnwvnfw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jsprmsbk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yxmrmhcj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xejcnkrk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ivziogjj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3scrjfpcc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3trdwxsid.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gkbjkdnn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3evjdidpw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tnhjxdsl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtnbvoxt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3upzheeua.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3qlvcwfyf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kabzxane.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3uxvknxvk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vunftmje.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yjogzegx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ptrzywhm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruhozpgx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ihwiaqrc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ayhoispg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocaiddmt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wmsenvnd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gbiimbqs.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3prknjepg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3crkcpklg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hmcjazux.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mxypdsow.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3aaxyngja.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ytxsmpme.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3icheftjk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rnplhtci.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wlyvfzqr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fdhjtcwc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3npyrfiuf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3veupllml.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ujnyqtnv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ongoxoii.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gauaodlr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnwnspht.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aaadcsmb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3exgmofpf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtmpetyh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3okrysolt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jmvfyrtb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sieftzff.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3feeclkyf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vutuwwnz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tdccjivu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3flttszcc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3sivpspmr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3msjordwj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kmpksbah.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3celfymjf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wmyztlma.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3daxhrzjr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gzbzrqgg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qjpvpldr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3eokxwlqm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ewjibsjz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3imkgjsyr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3nvalscro.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3yqxhulqx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gjaidoqy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ygpcmivg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3zxrwaoro.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3leuppqvr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xbuitqcw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3lulxlrge.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kojhqxdm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3kxmtixaz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vrmkfood.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3teaicfwc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3upsvthyk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yrpdejyn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3dzcenqfk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3hvyifwfu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3stdnvvsu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rltlukhx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3eskechry.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3xqaawyrc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3nxgsiuvh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gbefwrfk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lwvserqo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3yakrfxkn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rwvuxfbp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3yclzcyeh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ifzmjlpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmryzfkp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3bpxgoazo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njjrsget.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3mxviwxws.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ieplntte.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sffddwyc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xqexyukj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3etljjplx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cckffcsq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3eoikmuxn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ltwqklee.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvhvzuro.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3lqysgvcz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3gshdisgq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tatzioqz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nsztqzbz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uevxnhwq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uuwfpgwa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3dqnglldl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ichihyjm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkofeykr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pfksztso.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3bycdrper.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3joopkrzm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qgasexje.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cvkjrwqw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rzzozpge.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3knmlqsqv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3hhhycxxl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nsorcvex.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3yesgxaqk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mzesuyqh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwsjyywg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsfsbxap.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfmmxivo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3weveohaj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ujmgipvx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3sftsyfdp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjcwypls.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3hsjojjbl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3fydfdvts.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3egkevnfg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kjhiaguc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unyadhip.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnvrqxvo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ccysadei.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3okeptaio.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqodfnct.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ekqjjuvj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3qaggazxw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3oersuaya.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3phfkblyz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iktowpup.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3okrdpuns.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3pzrsxvoi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3nzifiphi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3javssrsc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3xqbaxppt.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3tkvwhxrp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zfqhrolw.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3apawxbsp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qvzutqps.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3tooctxvp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3zarbajuj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3djpoqnih.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nqcjagay.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3qhyqwdre.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ihebdngh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3rpvgkbha.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3gvzclbfe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zahnspxp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3pjhrwuti.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3wuieyxxv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ezdcetyv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xupmyqpq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3njpxrfqb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3tyhecgtn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3erjxnhzg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3bzcxrvoz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3lzivatpt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3olgjvjld.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3xzdplcsw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3gxpvsgss.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3pjbchzjh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3izapvczj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3scltxovh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3mkssdtkz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3eudzlrfi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3udqjrogo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3npbntznl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3arbiclur.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3xwkgngmc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tuujstrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdapgobv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3slzfanfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aeraurut.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3npvhuexh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3velpefaj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gwzsthkl.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3nnkvwopd.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ntacyhky.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ftbgwnkn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3itqgsqqq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3khkouata.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eyamtnzo.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oebalxkm.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlrodnso.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3sltchozn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3rtovorvw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3grpldmvz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3eywxhmnk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bzfqieev.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ufqzawqz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mjvdukii.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3cmjlnypq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3kxduljdq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vrozfqom.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mnjdttrt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bsvgjqzq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3pjiobkwi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3xpdtdxwr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3eisukdzj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3uixfboxn.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kwepmjnj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nscogqhs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bexvowij.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gzanujsy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qbqxvdcv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3trfmrgam.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wgfhgjfr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3elbblwbq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bxhvpytq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rihkbwsz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3echyselh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ozhzgemx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gbizwhhe.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3kaqejcoy.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3llsybjtz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywvusaea.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tjlutqzc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3tsqsualu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3snxqyjjo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ludjhkal.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3myrujkkq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3swpmvyex.html


<!-- 参考信息 -->