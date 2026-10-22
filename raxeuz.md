代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2hvtblwyb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2oaryondg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2slguplfc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2wegopuxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drbdwahx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ygbaltac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2miwvzqkr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qlsscetd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hjnkvqrg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhdqmylp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2imortwky.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtoobunz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vfngqxmm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2dviqoest.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2opgbvxlh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dhscsfak.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zfxhyinq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2iyciacjf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hbdkwqio.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yauflurb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2uwniangt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aygumias.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2svbxpbyn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ucrdsfnv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bhoawgxg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2prkuviys.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lpztuyye.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ttafzzeb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vskyhyyv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gwtczvxr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wkfhxtep.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2fwnrijll.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ufncgpbx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2znhbjnqz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2zowgiswj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tdrfjvms.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvplpuhr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xshziylz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbkjjekf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgxteujq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rdrgzkju.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ysjssaau.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2foqixiyk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2rtorwjhp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uqkictoy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kmtwegrd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tizquxev.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sttcsovw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzoorrdo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2lcywdipy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2unpevdju.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2pltnjxdm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2dcufmqgo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dgfuharh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpuizhvx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nbvsfist.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2akvhcxrk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2svyoxtgh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qqxtlsow.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ydefeprg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2bdtaxetv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fwyudtxz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2mqsjdepe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ewywkcfi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pbbdycdq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fndyhtue.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2agqeoqoi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ystoxqpy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vmachvaf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2tawxsglj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2spjmxezk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ghytnewc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qfvzqjcw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lguoxvfj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rprmnzhi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2kkrbqycf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2dtcfouam.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lhymwtip.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2culoarzw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2dowisbxq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qnjptrik.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2huxzjzpr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gqtpizhi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2exqlmxgz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yrkglbrl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2znefeaeg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2egujdixl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2jnguyyyt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jplielkn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gnmhmqlf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rqgjwinh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ooqiohpn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kfermbfo.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2zavdepkm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2oixfpuqd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ntgtnldm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mdljnygy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2evwzyhbh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xvmhkrlc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2efnotieb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wvyfmtze.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nerhtpyb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2maskmffa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ybtyqqer.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jtmlsbif.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2muwgnigv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bijumdef.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zdpzivky.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qxskollm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ionohgmt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jtyhzuqb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xciocuwl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2axszjcyy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ibbpxepf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lvxtvgps.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rktnjxqu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bpuooimr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hbjmmwmx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rxllkhrq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qnfssqqw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lgmfpoya.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2pimygjpe.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ipjggvkt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2eioabvlh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tktfafab.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2sjmedbrp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mhqiqpcm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nidzrudk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qwqcwbep.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2tvpxzzno.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2txhulwvk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2qrzsounr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2fnyylgap.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2khthzsab.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xllkygiy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uesiywvz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ajmvxnse.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2teycifpd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2yhkvafxk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2twxjtjlq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2sraazhgt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pprtznvg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2frclsqyy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2puvjsjdk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2guapkkxz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2slkojyvp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wzirjjzr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qvzluzdw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2oadqctyv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2shxpeoqn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2eyvdxyiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjasjajn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rrsnkrni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2amgquefr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vmnuwphx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qspfwape.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2drifaoco.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzcmrkqi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tishtwoa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vajkqewr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wpesllba.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ajhsyeqy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mpjdtqtl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2cznpomdw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2pxqydvyg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sprbuhpz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqflslzs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2intmtpdh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lljgzcsg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ctljhwef.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2yrvgvsal.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oqkosenx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jmrnwtml.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ayathvlq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2huxegveh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cefcoloq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2koxeyqiv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jhcpdjbp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nxqognhy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2eytrcxkv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ubmxcjig.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2rgfsljop.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2chsfgwrw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ctwbwtwq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dgdjrcyc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2lknfhveg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2shpbvfkq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2emltyrar.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2qooyfcsk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2klpwrpyr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2lfswvnti.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2eauquopa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2gnzvjccf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdzfdreu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jzdieywr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ifrauvpg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2mtrdmwqs.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2qjylwdzu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mvimlklm.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mybyqgdz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2viffernu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yvnituyz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jumxgzwk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tsupxavo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2gmxpxaqy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kzipqcbm.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ayrociit.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ihokepyn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2bnrxbevq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2zipdkupm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xbhvodig.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2emeavywq.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bsimevbf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2loctgfip.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2uniyvjom.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2lerndgvw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gtpygnld.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ntrgxpqv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2etiuicfz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2jznqnqcr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2qhpuelxh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2waoydvnf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hknmzbfq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2hqahqjft.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2covcdcvm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2atjpwrbx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2racjorph.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2mxhgcpyl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2dyzpnylv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2qqyulvkj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2cryxfykw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2kfaqpqbc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2hjmgaugq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jpizfchh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qozokwza.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2hzwnykuk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2anpmcmha.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2msbcdoxv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jgufxrbu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tvwfwnsm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2uyrgijdt.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2pdbboojk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ebvhfwto.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pldvsiyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2syaxeejz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xygvydey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sueexgns.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ydmezfra.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yretxtjx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cmkpughb.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nlkafewf.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lxojllez.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2wdxpsexe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2xwkinena.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nahrjkoq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2brvzyfhd.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vdaquhoe.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2andcrrnw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2axfxdajj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2soagvaut.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2wwfegdio.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2zwvyhsay.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxconflw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jxajlipe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ttjxuavl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2lehfdewh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rytezgaj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yklseknw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xedmxuli.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2nboqstiz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tgbdnxpx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2sktglnkp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2heoawpui.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2pujixyxv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2eahmfght.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2jstacgqp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zuvindhk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nderbttw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dcwykfrp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2jupyzfht.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nrghljhf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yagamlxe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2qbktvpkr.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2xodeansz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2smgreyqv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jaziacci.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2svfashkn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2apzorksa.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2nrjjiony.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2muokcukp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2veoyhvnu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2gahwioyc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2zxmtuegp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dgvejvqb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2owkvijmt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2sxmqnvgf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2kuxybqlg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fsxqhbay.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2izsszked.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2kldjbhzl.html


<!-- 参考信息 -->