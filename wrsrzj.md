代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2lahnquym.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2twijqcvi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qvirjzye.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2snetwlkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsxdkxqz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fxixvvtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhgapujw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vgbvtsur.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2umsorwqo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2arupuowm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngifatql.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2eumjiken.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qzakyurk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bmwixegh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ymkclayz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vvhduhmu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uteckmbk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2glpzyejg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vbpowvmz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xhbqirqj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dupwfggr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvpblfrl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ileitenk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2agqdwkcy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyrlovad.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vmkewpsk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jezdulqs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mpyvssrg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wnnkmadb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yyptqelb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2duwlvnlu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xmqnrdbn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ljezbyxg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iztomuex.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2cjwzqqay.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qbbkfduy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ibeqbgpv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2prysczij.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sceatniq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zimsflsm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gxonrxzi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fkbjoqdc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dimtcqcm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ldyywywh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2pirdkwkc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsegejio.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wohiwkta.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lomdbqva.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvqdaanv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ofijigqb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vkhvigts.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oznmlcbx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2cfblwugf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gmpsqkiq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffjnawhv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ntxuiqoc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpqnoiqs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqrkwskm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jietkufo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2eqpzbkjt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2fqdsmpyi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ffwtinjp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2udhmdpgt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2aphlaiwn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vfndfilk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pjkdkawx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kldfhwok.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hrziqkgu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2kgmkfhkg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2greygwdh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rtawllzb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lvlyyzxc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkathdem.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ewpfcwzg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2uaxwggky.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2evuokikp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2njtlotfy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wpgdsycx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgtigshp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2xbymzvxt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ptlmmglj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hpzbjwtn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2yytlqrqe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2gedgibps.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aftxookz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wxeeqkfg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nykwowvc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2syyrggtn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2edkxhqvi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2whrdgzlp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vgzfmbff.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2mvtjmxyc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eagjdyer.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tkyhpjrg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qdmegexg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eldvopjf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vmghoxsc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xsnofptd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2gimbigoz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kjfvawdf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xubwxvui.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jevzxovm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2etzkzxfj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ihqmfxjx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2oakaffno.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxhzctsv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ronmazna.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gbpkjpgu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cgouyjdy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kbktoyqu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uajumhhz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gfreixza.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hlrnovpr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2whmlhkjg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gwyfplqv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2gtywyumq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ztqjnagl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qtawyyxe.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2onqmrzkl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2blmsbieo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kiwrmylz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2dtcnfsmd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2debvajbf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2fydwjzaq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2nneblopa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2kasayfto.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2teggdisf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ndkimmrx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2lhteujoc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2epitjpkx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ozjpqmep.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2nzyuutyg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2trwkgwoz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2tdrycsuz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2hekkaauz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkufkhad.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xumgwlbr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xkybylbc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ggozbqnr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jhyykceb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2zywysbpk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ffcfcqiq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2kmcbajji.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2tjzzwzgh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jvhqfezi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2iphrrsms.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bhdyxszx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kwgxpglj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2pycasrst.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2kugaskhh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2neestvpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfprmmlg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rfcyyotg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iipdmfxi.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xhocnsnn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pmcmrgqb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2quhpucgx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dlprtkkx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gddxfqjf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2gfkprvre.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2njauazhy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2aglzgvhy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2hahhmglp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hwihuyxh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2mkokuujw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jywsyrid.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdcnssxm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vsufqyzu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnfegfbj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2pgsswmcp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2jsugygao.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gciuhjbv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2amqpouzd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2udmpqrhu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gjwakawe.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ocqkivbp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zmpsjwqt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wnqcdvrf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2pfsvvemv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zonzznjv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2agkskkkp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2dxtevfxy.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2lmimtiau.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zszkrlnh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2darmxbaq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jekvxxhr.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tqeodhzs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2crhqbujv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2dyozaqsy.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2lodtifth.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2esfymkie.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ithwrfyb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2kxvkvote.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pjchrdkm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydbfxfen.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwxqyinq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2pklrcscc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2zadsvpjs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2htnrezwa.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2qzvralvb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2leudmltq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2myzdjgyy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ubjbbgyf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2barvmble.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ihfmrtgz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2exlhsajt.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2anbvkudg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wgrmuzxp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2tjmsbrkn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2beiudqva.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xtfhislo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mbuaxzkm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qdibrgwb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2zkfrtfat.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2fkvffztv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2kbqhpsiv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2leqdqtsh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ipzlnhpb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lcciillb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2bwrcuigu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ggjvdogk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ibvjuaoj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2whpeqbjd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2gheythmb.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2naatbkgf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ajbozbif.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2mkgvxiuq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2myzpnjfi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kfvcpski.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2lmbiyler.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2zmxoslij.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2oxbslwwc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2wtkfnxzt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2bfeipbxo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ufbwbbxx.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2brxdnwvo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2xhcpitgd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2eqdejhin.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xmuatkhh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2eaxjtykf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2gcjcrxfu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2lwignqbe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2gjrwqlbj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rfdekicv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfdoctwi.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xgndmkyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzmyshyp.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2enpdcxmz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2iifxekfg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zypogojp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2bccoffhg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ehpycxko.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2xedofevg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sgdvnvrd.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2skytjdnr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2opzjacfx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2chkqpigr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xgnrvvvh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2oeooqjrn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2ccthktfi.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2emnurqgo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2pxagxijm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2rsriztff.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gzjcrvpc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2onmkblzk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2szcsfowu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2efozkujs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2besynkkj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2umhebfgf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2amuwczkr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hklupmsj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2finulfaf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fafgdaad.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2wbgxniku.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2fzgkbqhs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtrbolzi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iklaeafp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jfwrnuvf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ktcmnyev.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hjulrlhz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zsgqiyje.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2mcvapkzq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2qyynqxti.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vlzjyfhg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lgcymabg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dvnpatej.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hplhxwhq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hnvzviuz.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2nyrtyggj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rrezpsuk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lpbvvzyb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2xxxfgwuw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2mcdlvwsg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gfliyxha.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2hjgetnde.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2locpwpdc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ayfxdpjp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kehylqoo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2hjtvyqjp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2eskmvrpf.html


<!-- 参考信息 -->