代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qpdxvufr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qwmozqfo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lbwuvqup.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3hyxkyzkb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3igunrdyu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3oczxhcea.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dhlxcewt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3kdcxcsht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ugvsctah.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3mhqrgars.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ouvxrnby.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3kibmqkff.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3vamyamxp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzzexshm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ixxiosux.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3rhomrbun.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3dtuadghi.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vzsognzv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ldfcxmhy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3clrdykag.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ibpkbfoh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tathzdcc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3byyahgep.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldzkidzt.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwtbjbae.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tdmbzuou.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3zarrbgvk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3synhdbaw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ytykuizl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3whjsiuvs.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uoljfbth.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dmpjeljl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ljlvhjgq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cdqnydam.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wwebkdhe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pwcxdwhw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uqufqeef.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3pfesgckh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3zgnqrowy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wtxfuzvc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rcpqfovj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3icbsfhuw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fmbjgijo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3erjgeggm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iwgqqmnk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yfyutfgd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yjlfbheh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3woqppxnt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3sozbaeue.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aianhvkr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3alvlzqyg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zndzujkk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bslajbbb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3grbphtbh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cwjqvokf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrqqvsii.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wdvkosqg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xmwftktd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxlhorub.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dcswotxm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sznjcwdr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3frblckqk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wpnnzbim.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3anoucwef.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3lrxcbfcl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3nefvacjo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3rwownacc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hvtjqmjs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3grltazwi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gpfpuwhc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qqzkvwwq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ryqteaxz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3tthriucl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fvosydbu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hynrktta.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pdlgsibx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dujtdtwv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3armsxwwi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lezlttpe.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkdwbhsx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3kdqjtmsx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3hwfbzjvx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtrhitgk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3uadrihhx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tbidnyms.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wonrzutg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3glngusgg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3awwiryoi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3aqfgjycp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ygzdhyxn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3bretjhwa.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ceibxlns.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fpmulbvf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gvsvvfln.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3frxecjvf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zmaaravo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qhtmcmsu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3mejalndw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kdoezdbc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nztycmck.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zjfwmhyp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ntksxnlf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jdwjwrlt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3trnzbdpn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuwuyaak.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnxfdtfa.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ezrahhrq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3donpszxy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lmzicwep.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3quilagpf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zevpngij.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jfmtljxv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cdqfgftf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsqncpmi.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lajibavk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuciqsml.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jhjhjqrb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3smvbbpfg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mjrwuuma.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3icrltper.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ozhxkzuj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xvrmmszt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pfklbuqd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3chymbejf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jtxkvyse.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ydpvjmnm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kepcvidc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wisyxuib.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3mbdtufqx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3vhmjwlrq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3htqjowbj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vorlopta.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xhytwzkc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3cxinckht.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jipsqpre.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3sepzqqrc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ejwmbgbj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gborkfod.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lnerjlms.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ywurbajp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3rzhuxmpd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ovztnryj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3uxyuioeu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wqvdgnev.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tikkcfds.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3daulxggh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3cwsxuszb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gohlfxel.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3liyaruez.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ozaenuvw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xopplqxz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3warqewkk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3jntbdmoe.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qwythwdm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tstfoeho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpknkkjp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eattljce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxwevpea.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3bxkpfnxu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3dzxvopmk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfljdghs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mukryflw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3maathjxw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsiybahc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wgktqzqm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3okkkiyox.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3rjuaqcgv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3qedccezz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3odnyepdm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxtsrqlp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sxdgujmm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvglcejn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mvrulhoy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jseyofbk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3mspxihvn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3niuvoqrr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yobintat.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3alkktehv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hwjlshms.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jlzabqjy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3esknknpo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3prfohffa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3cryfiyxl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3bbewolau.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qdohwsvg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3lvphvudq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3lhmbwemn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lsfxjrxo.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3rpkuguxu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsedmqsf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lnjlhssw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3xcjnhodu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3llzdwrcm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3xcnzwpfv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3keohkoql.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3owvtgrzw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bwviyhwz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cskxgheg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3efspectg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnrdbqwa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3sdxyfcku.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3dxwlzrks.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pepsuspp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3mhluyskn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3takjqtvn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fnybqdgz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3emjifdef.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3laihieez.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3pexkpgzk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ryeplfhk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3svjfbcta.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rdhkbfme.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3tguyoqvl.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3clsvkmhy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fdjgzyah.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bmhsxdda.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wxcivwgv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3sndngblm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3rwvjnmpz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3nupzuptw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bslwhfgp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3objataxz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3adunhdpy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3jwugzpzj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3nqixxrgc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3deluzaft.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3wginjhxv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3cvstqeqe.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3gplwsjra.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jnkndtgg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3epvtomgi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3svuebdcq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3lxvclbgv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3zmduvkys.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3oputwjox.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzohuvbk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3symujsvv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3etylotmq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3rqjpoeoo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ywcnilic.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3xkjxgqdy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ctucinip.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tueeyxvr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3kjrcdhhi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3rktvdyrr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3lvopablc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3lbiellxc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nkdjsonl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfbhfyjd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wfsubyjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3srnlpbic.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3xdiwlsur.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fdanoxho.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kozpjpaj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjwenori.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3maiwvcmr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3cmlywpwb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hpewdyhn.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zhhgddos.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ldftsdcl.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3plqmshdi.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmllrggi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3dtplpeco.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3hjhrxxgj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wjbyaffm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3akmduxae.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3umyqhjgp.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wgvbldjf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uueqeqtg.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3pgqduyuy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3efkmvqhy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3nhjwvojc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pjyfhkxn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3jycigajf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cirhrbcx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3jsibcztv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gjezndlz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3mhfkacvq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3luaegjby.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvzweefk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vunwzldm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3jsshkhou.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rowyorbc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zrnuhpje.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3soxmarcs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ucasqrxv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mdfzjnrd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sxfavjyn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xmpdnsma.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rnygthbm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3oukycsod.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tpxooqbf.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3ubblsura.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3aftutidk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uawnxyrb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3edlgcuvo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3eqfhazic.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zqcbqifn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ecehjblq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3crauloee.html


<!-- 参考信息 -->