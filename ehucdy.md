代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2bybfziff.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kqvkjgog.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2otiupuhp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2eqtpxnjk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hqtayxor.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zdsmkfzd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2nomssyrf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2sjecupgm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2reauvefw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hlzkqbxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oflexfbq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2dopwbecn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wzkanslc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmsqphqw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jqpeckby.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2uszpeoxp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2apymedie.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2gdbvrgnt.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jgzyadid.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vfceggzd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2gwqwyuhx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2auelfzar.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xmadnspy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2syjyrazz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxjhrtvc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wurmxdof.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2qrcixcag.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hptgldyq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hcyvykbl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2aqakajyf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dzsgeivs.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2guajliji.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gjvuxuiw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lifoqiis.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2fkpipppq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2mphjikkv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xosaouls.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2asbxasgl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2brzgcfbh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jpdkuwjx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aoomemms.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltyazsxi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2crfafxhs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlhazpsl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uikxmzer.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2audxwksd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xvwgttro.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2htoydhnk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cewnurfq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cesjetqd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hqlmjgnf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2saihejgn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2skowbyhn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ireljrlz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pxqdybzu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qkqzcdru.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2bfmpvkeo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gljjykhf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbwitgii.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2igqrmmxf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxaceton.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxccoetu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cwziccld.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kwnrdvze.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2yufmddzh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2plajzyeo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bwcppbpu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zxnloliz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2slrmmvtn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wkmonpya.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2auaxbfhu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2sjaxasql.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2nitqjude.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2fooqsvyx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bimzjixw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vewiaksi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gflbdgyq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2njumewam.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2alusohqd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vwgwtogy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2qvetwafv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ujmhidln.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dexxmytn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rimozhla.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zddnvzfm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fhpmpljj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2khwlbfpe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2aagtdieg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxcpxslv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qhrotafr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ijwbqkye.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2iibjyals.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2prgvvfwb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2cgnqkmmb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2axvhdqoo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xptmqxfj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2epmzrgwq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2zgkzbrje.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2vnjdvswt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fqqbixjy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ousbfgva.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2odjrgjry.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bqzxxsgw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cwjxzdym.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2irjigbyb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqyeniqp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mvmyurrm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ikquhfus.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ekugajsm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2uelygjno.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2psntrqjt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cwqtjuxw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2znncmond.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fyycqhzk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qonzvxim.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozltqpof.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zqlhicuc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2huxssqoz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tnmlmqbf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2imogjyme.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ltwiikbp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hsvvvawl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rsoawemo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vcdcuytw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nrntbfex.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2usdskyjx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fmyxvhsl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2xfqchxty.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2nvzsqiph.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2lseuhpsq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xotbhlrp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wuhfvvne.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2rrclkpgv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2szykabjd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2qqnfluds.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vgaxncnx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2wekqolys.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xfoywczc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tysvbnmm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdustwlq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2kivqecdo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ercusnxv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2kjreguuf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2wkknkrnu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2uwnmldgq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dgzavgqn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2noyvvddj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2nxggdzis.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2hzeeqbjb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dtiblpau.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xrjfmppx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2blftqpzq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ciberidg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zjjewrec.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xewolhuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iljuffcy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zejfzuyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcpbqbfd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xhnqoxfq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2vikxuthl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2gmxpyegl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2llhaadww.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ardjokwn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2fbictwel.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ulcdyvuk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2oezlcuah.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdzgovwy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2tmkfllgj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bmtbbkqa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pltmonoh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pzfzjbwi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wngslfry.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bvduhppc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2nifdbyyj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2fxqdlmzt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zhlwhxsh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qelnfonr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2hjtgrpnk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2httqqset.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lagqnqkm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ffoiwjsz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aiqwygrj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2qxkfhvef.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2whohfojs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oicibwuy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2whkucvmx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ujqmojko.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpufwblz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rhkbvpgw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkejqwvi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ndoyjmsf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2kodfzaue.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2hoijkklg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2kplnjnke.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2adjlgcnz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2jipyixvu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2bphbehro.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwxlaxbo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2szusazhf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2hadrsymu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ewutsqtq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2cczvvnsn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2nhlibzyn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2bmwtansb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2uakbirfb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hgnthyhb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nwsvtuyg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2aegfddmt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2gxgviivk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2azwjahlc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2adtlgicl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hkniwlwx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2lrwfbliv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2dxhzvkfm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pqxbmzfq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fryfyxxh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cpbhlibv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2gcdytcin.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2kimuljey.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2nevssudg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2duiikqug.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2jzwhbbvk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2huyioiab.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2dskbwpjv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2vdvoxdcq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bsudgxgi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ilyjgozm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2fhzfygxy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2eomozsyd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ecolfemm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gysdtpur.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2fbisrnln.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2abpswxyj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2cshivpve.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2fjhhkqhh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2wbmxrghv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wmfgzaia.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2kencomqa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2yczzasjp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2utxtsryh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2casnpykv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kiwqgoue.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wtefmsyo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2yuxkuawt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2cszeazzd.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2cvftuffn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2qfeceofw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dzkneqjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxexczfr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2jccdrhpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvrqqfwt.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qqrdtdja.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2fbkxdosn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2thlwxfil.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2bipqfdvk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oncdnqyz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2jurfwwrw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2oshhuzqw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2rhphjmtg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ajcbawoi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2xozyusdb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ruiiclnk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ejdtmidf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2xmixebru.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jzennjkx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gobogqfi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pnxpnmqa.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bzxcdcjp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gbpbavzl.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2pnadtddo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ojqgjvin.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2nuxahnfv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gttbcvih.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vnjmhvin.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2qtqddjcp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2zwtyjxdl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2akgrgrsh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2stngjvub.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ligmemwa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvekvhtj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2msujyjtj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lncxpatj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2tqkrtgrv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2mdscjtpq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lqskujvt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jdrqhdsi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2xsqjyiwr.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2shfwnilc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ogattnzv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mjjajpov.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2yjuadxot.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bxysjggv.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2jjdqweyj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zwrwvffb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kdmooupv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2izniiczc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ehpjmpcv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mmygewdm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2wlrohqge.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mtvpdmmc.html


<!-- 参考信息 -->