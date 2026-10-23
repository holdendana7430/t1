代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3atmivofj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbsqhahr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nllchgpw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qunkrsdm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3uatpczlh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3sytcihvv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fgsaerzl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wyppmmja.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vylqczxw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3vgukijiw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3djksxcly.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3gtizeqnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsvckycc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fhdzddlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3juzbmkfr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3gnhskvtq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mavhsjog.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ptpqsbmb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nsfcryik.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzwxxfyd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsrshgdc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bifisztz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bjivqiag.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfsgwkje.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3dlwwkwoo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zmgtjmks.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3idnivzpd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3enfcmskm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3uarrpcpz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zisowedr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vcpiowkq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3pnrhnqxw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbucoznl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3weaqprzn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qvcetxkb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hgjwfrsv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3atxzqpog.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3nnylrlgb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nwwavzdb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3uoftvegd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fadqtqoi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fvltcchb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3dcwcmnri.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cmbaactp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bazxelcb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cppcezay.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwsaxmwk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vdvielbl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rrzwfiyz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lnmaoovp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3goqaeivy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dmnpahft.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lobpihme.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouixijwk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiairffi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yoehruql.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rhsngria.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3wjvykpdb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zezuzxox.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jiurlxue.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mtlyauti.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3pyfeoojs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pqoifpyt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhsaadax.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhabajvv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmjslson.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3nahkjtyt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3apxswybp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ryzigzaj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gllcnbvy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3rldwpbwd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hfmpiigc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xrsmekng.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ihbmtgty.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xuokszcz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3gebnnqnl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vfghcriq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sbycuxrf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rushiwhg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3buqzdahq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3kylncjqr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdhdfyvl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ritvoqaz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pevgubyc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3chmltcnp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3gmgfelxe.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdwegxgw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3aczceiye.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3pluxpmqo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzurvbja.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3trpzkelh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3uaepkctb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3wqmpzelo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3iibtlqaf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ojxzlmth.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfoupnmb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vjmezzah.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gowjtonu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3drablkem.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jcejauex.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ggukismj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ckgiwock.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3khbnlowe.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xobvahkj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3uxxxctdy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hetckwsd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qlaycwxg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ineqetbe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qoycnvig.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pahffjjy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbuizute.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wdjwmouh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3baozcbwp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggnvviqp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sjjluata.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hnqkynqb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vcvdywuq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3glmtpxev.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uflkipuc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sswmhhdg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qnyycvcb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fvdrjdaf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zkqrchrr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3wurtldvp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3niilcpom.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ryovoesp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jvqhukre.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3doevejjt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3worqlytg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3hkaacobl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bhsqnqaa.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ydjtfnfg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3homftwpg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dawbouwa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qerqhvgr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3phozolnx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3pnwpfnur.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujaeemqe.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3zvdtdiyy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3yjjgjavq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vbijknvk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wmwdjbtl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3bjoaymug.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ygxinubk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lpveexbp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ugjwfixq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vqxxkalu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3kvgcnoii.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3trofaxyb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pomabiaf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3kalfthax.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3jkiyvqnd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3djymtpty.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nphqnvfy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pcikpmjj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vzrmbvew.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3syebvevg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hpcfcygg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hchxyxww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykhgapzl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3fyrcqzmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqhnexjh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3uyqdvuin.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wdsnjzyo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3yicoyrnq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gcdykzlt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ybazayac.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnzpcdfd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ornckcyf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wrpadgtb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3lrhroewy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3bawnsxbq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qmteqfws.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3slzcyuzv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lihawxwo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qinqzehi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oeczwogy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3rdmnycvx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3wvazmzfy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mcphqubc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wjwsgcwp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3kglldiuh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ncufdvwo.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zpbadmyf.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mxsdzplx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ttrahwwp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qepeyrhj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3gmzkhlzl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wevwrcyh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3nsakzdwk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3necbjrhb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fvrljiom.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxwthrcc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hysazooc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hmwonnqs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3jxdwrdtq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bfbrgbvf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3vyjaradh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jcawbynb.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3guysxsbw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bsnzwaeq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqjjjkgx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xxhdsnnv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uopavrab.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3fxczdlfm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3tuljfexz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngycvcxq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3uweduejk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3qygpmpnq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xsfwitsy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3sclsrwtu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wqaerprb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3pkqurmat.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ttzmurhy.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3axfyxclq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3uwmqhhds.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3rrtcfkdu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3sxagbxuf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nrmwlatk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3piptkjgy.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vwmeqyub.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3fbkuhmdo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ngjnphvc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ncsnryia.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3baaestma.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lwuvvjnr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3abpfqhsn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3vbvekyem.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3hejlmjph.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hykxoqgo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3qatrphcd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ygeerrlm.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3juieslup.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3vntaahvs.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3lwguqczg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3vpibtqfg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3fkgocwfv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ztgcpisc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ciwznctg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3mbgsiofo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ulwqtcps.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3klbeypot.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3vfwrmkwn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qbdymmhj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3hrgdicjx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3urvpyntp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bprygngq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3qesozudt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3pomiyxeo.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ddyjfstu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3rcpuprdf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gmvluyom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffctvxdu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3nngdzfrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiisoyhl.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fnbwskel.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3cqfbwcus.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3psinigpe.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xjsgysqv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zcdrswvg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ctbveqts.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3mcdbmobz.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gjgrjyrs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nubgdpxt.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aqfjurgs.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3uousgowe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3appfiulm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3pfpaoxoa.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3rgqipzlf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3boujlzbf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3pgcxqjhb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mhzpabnt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3auijdkzs.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3vhemhifp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ksjvehtv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yrjqquzu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3gvzmgqud.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3uyhzmwfm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lzzfptrj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3plamjrub.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tvfgikmo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ugyqwgmz.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3tzgtklor.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3grlcsbxs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dpxlpyuy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3hidzuknh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fleerclf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3txjpvhcj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3lxxxvfit.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wgzepuvb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tqrjvqae.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3zaesfnrv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tosmozsn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ytbuwpez.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3snbfinzs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3pfkitgga.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3insgkbjz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ivrewrqh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3aowdaakb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3tbmbskfz.html


<!-- 参考信息 -->