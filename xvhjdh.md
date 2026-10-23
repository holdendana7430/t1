代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3vhrvqkbu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wiiriwum.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3eiihtuco.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gksfxwxw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3aayfgdbd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xumyxgyw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gwnmtppn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3nwlaahln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxwuptkd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3vbyylhmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxpgyqeq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ytlaodti.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jsdztosx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3apqjoued.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxvtiuvi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoyxfuot.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3icrgeghb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3grwujnan.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3znhavjwi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3chthuglm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ndmqafpw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xffpuztc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvvjsapr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gytuoasm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3avstnzyk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtpfrmlv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tlwzzrud.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wqhpehln.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3romgnmau.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3toirkdjm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gwnwvyjq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xssrqurw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wjtxkdii.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3nhonhjvr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3edkidrch.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3psxmriqb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rxsobfvc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uhcayruo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mcwwbjaj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ycjfrkhx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oehvepud.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmyyuzpn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qymgiqln.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jjfrrdre.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3brlioaer.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ijfnzgwa.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3anbgspoi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3pkxdbaae.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ztdxgbbk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nabuxwrr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zzjbyatp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kowszrxf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahukttta.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3riipboab.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vpszfrcl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ugypzvmq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jhqkbudl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3riazzsgs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mwsohhkd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3peminsua.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dijdshtu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dmuukzrv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3dznwjtzo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mcegerbw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3mqillfca.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tmbcpeod.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qbrpadpx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ogfudpys.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sllmoiak.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fjrogoxw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zavsomba.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qheocepg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hbysrzwf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fdesimqk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jasuswve.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3wnecsgvy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vihnkxem.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3zotvhnvt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3jsingjce.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3njunoicz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3qneazein.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3cgvvbmrn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmrkvogz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3nxrpzjfh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3isbepvmw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qoxtrlyh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wmxefbds.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wyajjdwk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdbgqlcc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3auhlyqsy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3luybnvdy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwstsdxh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3cazuatfq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xlxvcibo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rahsstzm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wqwxglqp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cocdlqmu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3dsbtrecc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nczsjcmr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cpbkweys.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3gzvcgncy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3aupteuwh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gsrtedsf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nmgeerhx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jrcnmugm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3srviexdz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dcjerzbp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vtltifsl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3yeeosbca.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3dvsquczr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3afonzgfr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uiiuwjyt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qthisome.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pdraokmk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ydyiipzg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruligexp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jslwgmgq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ppcwnojj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wjafluqh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3wdbxjaoq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3aefoydoq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xqfhuagk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hpbdblfe.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3whwzvjtq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rbdpurje.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vnkcafum.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3epcwpajo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ebhjhria.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3thfntyaz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zpqxejuf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dsguafze.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ziwabqqo.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ikdefilm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3iabkjqkh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3sbtfjfmc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3andgfuau.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3itzmrldg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3kgndfpjg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3umusgqyz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3moznhzkw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3eyldpbcj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wpbzcjjo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3tiqmwrqf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3hjyjcsst.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3shmwesrf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wyinhiwg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bcatzzyu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3favpmmwb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3nrssazkk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3camikhdh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bbyuziod.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3belyfpsy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3fmrwmndv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ufafcyns.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zaajxaia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybydylcr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vepmmabx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svbrtgoa.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3uckplmfx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rpjshhwp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3bfpghlho.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpajgkex.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3byogrecn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3scnhfgcn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3xsrdqfjv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ecymjnyk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrkaatbd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3pobvgxwd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3igbkhsoh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjxocneq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qogushjc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3huovroba.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxkarclu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3nnruzifx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3cnclbpfh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3utukzese.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wjxzavqa.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3rtjtfmuy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bdtkoifc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3biyekmlx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cnwznjar.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wpmgioiq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vzsgkpes.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3rigflbjv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3htklxfre.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3xvxcfasv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3sqveenyo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3eeermnhs.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3htandrcb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dqgbrklo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3crgwsurz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3bdghdxle.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3cgmcheol.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3asriwyuj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3qjvwvkds.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3aepokxon.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3gkmsuvkf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngrrmjgd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gvputdxh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3csntmqlx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zcbtxehx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3twyxhatj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3vcldygbt.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3zljhzasn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3gghvalgo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qxwgisew.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lgyvdisz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3wegxfxgq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3gnlkugai.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3qytewgoj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xyuerrcs.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3iclpigse.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3qeptguhv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3zqceunto.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3madslbhf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ombvazjk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3alxxwtly.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3wtirubzy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3cxddwhje.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3hgztarkl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wyfudgcg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3oqtuhsws.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3cdlnsqsv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qzzpkxrb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3fhbmkokh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3aheximpu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3chzlwhqf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3zrkjmugy.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3bogayxcr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3sulxrhye.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3emhscare.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3miplktiq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3dpdylmpg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3cdwiltif.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3jcmmtrso.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvfvlpmn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3htjrzgpg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3qsvlvdpk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3vhmvdprh.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3yurgjdfr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3hdtejsog.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3wcsnbetp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3worjgdvv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3njowifgy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3nzumpidp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ovestskr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3fbmliszd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fopfkuao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdagrjbz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dpsrzdqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvzueyoz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3znvpwalf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3tkdjwyuf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kugyjzdf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3sklgtxof.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3cjcmvofm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3rwhxuyvh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zyiqlyxc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3itmljqss.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kwzffadg.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3fhqmsiay.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3afiipnmv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3wbapedja.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3kutoyzkb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zyilytlp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eindnlfs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ljdkxmmy.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ugegaovj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yxbsusgn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ehaojyal.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3owltvvlt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3rwmlnesa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zmeciqtp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tsqkzzbx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3exbzylwo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3schjovnt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lmrwokhb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3gohrgerv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3vidsbges.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzecomtx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kscfgpyt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yiaptsbq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ovqpvnuf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vkxvbvwu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dxtjnfnv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3othosgkz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3taysrwyv.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jouvluyu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3nllvrhrr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aolmpusf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3hfqemkkm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mjaddjuf.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3lwqtvgkh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3jryqibva.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tbjnmzgd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3eionqbyh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3yiydzepv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dokbsxhi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3yczoclvl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3zgnsjyvj.html


<!-- 参考信息 -->