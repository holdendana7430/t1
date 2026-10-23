代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xarybyyl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3pzjvwpfc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wsbdatlp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3kvgfgwde.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3bofkbjpl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zthekhfk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3brqpywrf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ctaaussk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttnvrfce.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3vzfvsdfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcazlrpw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3tecmextj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3olfvgvua.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkdvncaq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yqjvaizs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vmpkixtd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3duwfmema.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3thyvngza.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fvewfmso.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3icrpzlzn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3gjiccrfq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jrbldmep.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdtnviyf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbeqkilw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrtpeocb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qupnfupl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3rthzrojc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oxjeevfx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuxqmrlr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rnsuripn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rvvhepwt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tiwiiekb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pqrewqak.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3adhliwfn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xdgwwqic.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3phzabtrh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wirkaqak.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3auvuqyyd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mchcuikm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kknzmnal.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3duhhxzba.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rftikmqt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jpkvtysa.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3alpzoshw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eojscgjd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zbrdcotf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3azdyaovn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dnzvdnhs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kcrlxhef.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewfxdhrr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xheqbbln.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vbgxpaxc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmhowrrq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fwtmdecv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fxfuujxo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3xqazfggx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3kmrmiqoj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ldrfeapb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fjcesbds.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oooqapqe.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uunhnxec.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qufaiakz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3seqicpjz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3gpqztqab.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3urtbqzsp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3btzynyto.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3kzubnoud.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zfxtvxqe.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eimciyzh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yohfrvkk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fielpnro.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xxrkmpzv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3mqinzayq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3mdpxilnh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hgqtbjea.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3esmrcwgv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdontpyn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3febcjuzp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3irwtojmz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hyqkdtir.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3umtvctbh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3xsjtsnyd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxzlgvtt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3huyajcmw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gesinjrz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbeytuaq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ncwukgry.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wrjonmoj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3evmvtjht.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3uibpyvnl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zlxyypvp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rpdyudlu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ldvnvaaf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3wsgktgis.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lcvicsiv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3yaqbtynh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vehlapej.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cmapqhjq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3lilljgkz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3scyeqpqo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tydtoqzy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3uzdfizfi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3dfkaapow.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wtwpbabc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtsglfyh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dopdctgu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lsuhmzog.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ailctzsj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cdxvcdfn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtsjnjio.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3eninaoup.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dpxfewvh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dpxebeuo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3varpmgsq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hwrvbndc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zhorqluq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vmuvniob.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dcynwjgp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ppbjsjcr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3sxnitabq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ndsqhfar.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ikvixydx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cdjewmjk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bjwconfu.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3imoaqxnz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dygtlcpi.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xqwrrfhw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yrqsgggy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ukbxyulq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3iyqozypm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ksrbpsqp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vbvukzrm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3cdumncjl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwphfmwk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3rjgcuvjp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wjaidlzk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3vmjjtpqz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mcmcsckv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3aubmhtlg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3meiflaud.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lijszgir.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mtfkzeks.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qazfvmjm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3oewqekky.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3woswkltj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qvpknobs.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zwemgdrg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3luhogidv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3igzxpagq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3brszwfwh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3usmnzxtf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3wrhsgsvn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3erldvakw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ncwqstuk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ytuafipt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brebodor.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3uwzvtxhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejilpmru.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3yluizxzj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3cqnfbhdb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ptqoizjs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjuhcmqa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcsxwetz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3qptrykhx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3nzzsallq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xxzuqanf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3rysvhmxz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3fuauxrqo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3hodiiixx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwdmpfcl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dzwkdibq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rratpnub.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ayblziwu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ooqulnrg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3jbmtzbjg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3umyfdahy.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3begvfamg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3sgjpehje.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3efqpards.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gvsddeox.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bihtwyku.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ikcgmlre.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3gwsaxszt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3xgpefqlx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hctwkrzq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3szgpdvpz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zaaidrgx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vnrhcirx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsxwuvov.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bhgvchww.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wodqmmdk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3klqxzjnq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3peqonsgm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjwiamfg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3totkbedg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3gsfshnkm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bhatfwjm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3digfbtfg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zojhjlya.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnhicahr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zvrjfqye.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xubctplb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xykvthhu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3eyronqdm.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3asovqqrl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nqiioumz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uoehfamt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fnzluump.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3xwayntyt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ndypywpd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3skyovaxe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qeevozma.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3wgvlruyu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ikywsfsy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xzkxdxmq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gwitbxqp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tdbzmpsg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3pgfipujq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3yhjzndvb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3qmjnhhkq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cejhljrl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3isiiltzz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3odmjxikm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3kkuclrje.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ljpbzfma.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3yanvlyaf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3nhaccdiy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3yrtmthjl.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3vbkyhxrb.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3eilrxkek.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3tjkltsyb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3liknevkv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dcvrdboz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3neyvmzag.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3iiuquuui.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3jnrthmaf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3fvtzovxu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3xcnovigg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3qvztmejj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3nbxcrvfi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3fhpunnxq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3kgcjmzty.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3neixepmg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vjwxnxvv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3vqloxgvp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3nyxhcyic.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3vgsaioas.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3chvnpozv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvrhodvl.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iddoxxev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmtblzzt.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3afrlfdkb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmkipica.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uhvgcxco.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3akuuwevt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lzghhluc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3vfrwakjc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3xasqtdhl.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wjhmcaoc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jbnaivzo.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jivchjsp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3adcvsrap.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3pninoqqv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3kfwvqhun.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3csiwimut.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3lozhdiym.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wfcknusz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3mpaburyw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gjcnguys.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3kwwvlhaw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xgwumpcz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ycdoazid.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ntyuzbhe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3llqwmyiw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3dmfpzbcj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ovrdlnur.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3kvxraunk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3tcdxtdwb.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3tyyumtvw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3zxnbddch.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kthfjulx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3auryzcxo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vhkptvui.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gjzfzauv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3yhvewjcw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3olbzisly.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wkdzhqyi.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3eclxduzi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3jcsykbbl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3juugcieb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ctzqwclw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dwbhfitd.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3mblpfuwb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3kdcffxys.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3sxmmdrsb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hpabnrqt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3oujhjsmv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lcicufuf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3bclawpvh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3jybcmdcp.html


<!-- 参考信息 -->