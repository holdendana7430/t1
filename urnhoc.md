代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ibkryvtb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ornhhcoj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bodymtde.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ytxpvsuy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mogdqobe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rtawlanm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2eztjghyj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tstswnkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anlnbwdj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2cubvmzex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idusowuo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xuqwzgkk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xxfghesc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ojpvsknz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgjflxmb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdeemagv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nakkfuuy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2giuyfqjp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2aajrkaxo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvatcugh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpgflhas.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2kcnlpdbv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vchgpnwq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfltrffh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uflztqra.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vkvjkhta.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2capqasmt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2caircuxa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dibroozh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2gelktpul.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2aujpbyhx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jvjwwvly.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rgeswgov.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qwbtrbaa.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qvnoaanv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2romtdwcd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wtphxyub.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xlgeqkzr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2tamyifqy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rwbfhdlm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcmhbeac.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gzjcqokw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iizvyjde.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bxirydhb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ywzbbynj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wccxrfoo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2keuygsmu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2stkbpagb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2srzshmrn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vxttppgt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kygwuvql.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2abunppxd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hdmswyng.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2yxnvjgix.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vwpbcbyd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fhnrvtsn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tybdsfwk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pavfhfzj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2flomqccd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqpwdvkt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jmodiahp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2prpsggjr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2aezwfaya.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vsojdncn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pavhlxjd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ubrbnjtd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2igerkhsf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zihvrhjj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2acdhpigp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2trhqwuvl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qqrfwazb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2vihsyjbx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2lladsvdm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2aqdkdtdy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pwykjvio.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ocvdqkpw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zezhhtjn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqtshulf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnolxwiu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2cqnbfaft.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bgdotcsn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ocucktxr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjrfqjrl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ygqqojnq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2bojtipms.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjdkcosi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vjhvjubs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2shtdxlil.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcmqwxfd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fmkhxcrq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2iyqooufc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2kagqxvpz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mpuayynu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ezwawkfj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mcgrenan.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2owjztnpb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2epvnblyo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ekytvvoi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2facbowjo.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yufbpnjx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qmujrsrv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jolsglgj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xbhlggbs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2blnlrbco.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxoxbkbe.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hzrlsqqo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qrrbithv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tyssaxsd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2tedxficd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yapvkwux.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2faanpxej.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rxawngie.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcclhgar.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ckapnjob.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogahywbg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jcoasslk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2offktufn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xwpdyuav.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xwqpnxzc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2kcoksvia.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2adlpkhrr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2feteelml.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ipodmelo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jltlqfss.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bsdlarje.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2gyanfmky.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2bqwdksjg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2apqcpbpv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ecxwbyge.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tljjdosn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ubefhrds.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2uyfdmrga.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2zyjefeku.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2tgbcsziz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kwoymtkr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xwophfzz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2yygbmcwj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2imatyidn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xswbdplc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2brhmgrwg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lnqmwrre.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uqrkxvwd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2cwxkltek.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2czfxycth.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2vzluvfaf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yhjofokr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ycherxiy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2diiorkhk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2fmrlstgq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pagmhghb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2twaearva.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2owfsvaqq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2tqlvjvwd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2rjmjwddp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pllaszbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klxvwxgz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yvqkdgvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpklgdvd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2nprzrwth.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2hurfrain.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdvowuxg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2oimahqsc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdztqvzg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2wobacpqe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2oeyxgiqm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hiwjqhkf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2drdgnhlm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2szmmocxm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bvttudxl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vbznimcs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ymzsffrn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehezyscr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrofhgaf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hlouldds.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2aqvhsjvy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2poynyvkb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rfkbltwk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2yjfmznvt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2edcghito.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ppiccsqt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ccjzoehm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pfxjopmt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2lhenksth.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vvmvkpzx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vphjccck.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2bktpymwh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2octdottu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wvkrhtav.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnlmqtgm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugsjknhl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmkkxpao.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2jyervrbt.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2bbzhskrt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2sygdwjpe.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2kljzxvpz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2gfbvvhyv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2dmbpdxug.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iifqbvlp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpdotcma.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2gycksagm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2phnvseqf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2bpvyoruw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsjeyozf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2qsoalqcp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2kbfmtirs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gyxyccvq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2roimvpam.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ebhmmoyf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2jflagxld.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2zgkbzeml.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2yzcrfdmo.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pukvfcxg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2xtpwcgpk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2roacmsiq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zfruqugl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qkiwuozn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2riudfqjx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2kyaokezf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2eafzcgsr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2otyazylw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xwywcmsy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ayktndnv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2jfrurgoc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2hprsfukv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2guklguwq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2eovsxelq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2srlaohgi.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2bioqwzqd.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2znqfmrqb.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2deoevhwz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2aqzlzoxx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2fdfxagct.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tuaanshc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2dqaqyktl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2awschvpl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2etolxxft.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2rchqckko.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2rdvbcxsw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2plxostmu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2fszthyuv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2kvfoaxti.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2pssmwubw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2uxibkods.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hjbdzigh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2iwhcdcqn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ydyhnqff.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2icdyifqt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lgiyazkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjhnnyfn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wgsndbwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfruysrv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zucqoyok.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ssxvmuiw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2scyqvzma.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2culwgrat.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ikeafgxo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2zujnahrq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mndifsni.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fmzgfzwq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hoyugqvd.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2prwauzjo.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zbylyewa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2egikhlsk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2fkyciezu.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2gavxognj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2kqqechkm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mnotdquo.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2eredqbjd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ytupfjts.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2rwcbigmb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2kldcgzzt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zyoscsul.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2uezylknc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2kwfpmwsa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2uoqltqqu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2jlvlgypc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bidjhakz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2lfpampgx.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2uybtlbbp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rcbmfzyo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fmbnfmny.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2cbbozoaz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2aetkymut.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2aictllns.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2uihnxvbr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zopknuyg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2jkbzisgg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2gywjqfxp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wuywugoh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mwjhpojn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2nvlifqzd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bmvtrrck.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2yybmmsel.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2watoeomq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cxpiaksb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2jnvjnlig.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2gmtopokf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2nszuvqkd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zbsvyudx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ezvhdjrx.html


<!-- 参考信息 -->