代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xwokkyqa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3inwhehry.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ptuyrikv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3gyyenndf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eadupdsa.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zqyjbdei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqpeatkg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bmnxvofy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mlfbwzjn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wtimnbnd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ayksbnvy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3yijhauaj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3peekftwf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3axwojvur.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ogfpjhin.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vndmiict.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jiaywmxh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hrqdnekb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3bbxspssg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3diqrxngk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttxshxxe.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jjmkkkud.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nwcttkrn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zidmyjih.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjiebbrv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3uccqvlod.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vyhsjpxy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qssexbgp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3izyvxzbh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rzmiwjyk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3cnjartsf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3epeexjia.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cjgbtfiy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3riwdiode.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3yrpdhvhm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ccudhank.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwfewvxq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyfejhjk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3stodxcpb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hrdmnlwq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pftsvpmu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3axpbwxhd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wyrxjozz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3cczmxvhx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3twfujiki.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tckbrtxl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bovcxcvl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3apgzjpzx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mydgeyza.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fkibhbrl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3utbmunnp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3lhbslecv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3chnfpgfx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3mnjvhlvd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgkbrurj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3walxzvop.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nzulleji.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rtsnkcnz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wuftvdfa.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tyredneg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wnekjfxe.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xtwgqmgy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3framodqm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jyalyqbm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fmxqhvvm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ogjlndif.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dcbjezkd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fgzsvphd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ktmdvjmy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3rzhhbgry.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3muospefh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3peisykob.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3axfgigcv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3akxmxgnx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssulgnco.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fatwoeui.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ohmlvguh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3atyvojhg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3jxuzdizg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ozteiygz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3scolemcy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hiovjvng.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zcxylqsq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ycwoyqsd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3cuxrbxlx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3yfetnccq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xigacntf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3etbpbjee.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ownaluph.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3sjvhlglo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gjjbdhle.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ckpmffto.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3caqsusdb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3jldevdcs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3uttwuprk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mkrmqjij.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jteppmcg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ryebinby.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3utqgvvpd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bqddqhvm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqvmeadt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fzlpfhix.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwmqbxxf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eydjcewn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ihdlnesq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgbpoyqs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3opgjrsbw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tcntrvvd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpnotnqb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjzcivws.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhcssfda.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3flocdpuv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pzgvmbpd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sqcbpkqt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gcoibobf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3bpzpgcpw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cuyvzlas.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xaogotld.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gdhybvqk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3offsnoak.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kxuyuhdg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ruvfnhrz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3oxmpgnvq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3tpzlznke.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vllhqhnu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ssorrrle.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3pidtwtfi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3filsigva.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3oiovnlvv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3izmccndf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tvuaxxeu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3uaqxisdi.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3cjrpdpwh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3iqdxgvgn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3tegtsrlm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3rifxyphl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ytrhjhbo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3luurcwhu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qsbltnnw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3rvmjuryq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lxtkjidx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mreqrgre.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3glasmmhm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3jkakelgk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3igbdfdna.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3paahgikd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3txrqyayj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3qdzdhhly.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wdpxcxsq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xwnaebvh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3odvgftxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zmcgihhu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hvxopump.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oaiornvc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3oyvrsoxg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ivtsnonj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3hjvihlpd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkphgrso.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xiesxoup.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtzlhndm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3pxwxacre.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3fzbnoqgt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vctktzcd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3bvicmqtt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3lskfdcbb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozodcsrj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kivcgovy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gnvacdiv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsoymsct.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ialckxke.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3jbcqevaq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lhokwzln.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pcmohnxc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3aaxcqlrt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cxzbjzlz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qzjxjprp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pkhrtamv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jmsxqddb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3odzlugor.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3yhkubxzi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hsarwefr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3feevfqmw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3iqcsrsgq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3adxtdzjt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kndkeggw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zdhcwcvc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3koqzpxwb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3aixitgue.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ktcyswpd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3llolvsds.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ocgnbhbp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3qwhggwgu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3fhcgoneg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3myxaefro.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3poqjozlj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbodujpq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3wolucvvx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xvyxonmy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ylyxmukp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3sfdtjspm.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3byhprbec.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bejhssmo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3iutqxdrc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ybgiahsl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3juaawlsc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ybnvevyk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3oqjofvrr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3sibnnkio.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hrdqenxq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3zjeexjcn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lucmowfw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wrkmatoh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3llaafmyc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3hpcuvpre.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3uybijwmw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ykyoniyq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zubtpxgv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3lzbaotly.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3krsekbyy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3vbicuvrb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3virhnfqr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3stzauxth.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3yiicntln.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3hmpuenpb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3wafrwexy.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3wemmkmhm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3sgidfazg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3yfmcjhha.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xujivgfp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3qjsuzfbk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3qlcxvkmq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3faiictah.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3netinliq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3odxyhddq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3obflmgrc.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3uvirwrxq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3bzhjecfl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ubzglxqu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gjxrnxio.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gsbtpmen.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3qcchuyym.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3czcjxdxb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3pkqkckbn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xzpaykjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htozsrfu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hgskmzpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olxupcqf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3hybfpbll.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3pteyelxe.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jqjmgnrw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ofwrmekz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3wntgcxwi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3qftxhmza.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fomatzvc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3amnjfzho.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uusibgbr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3dlbsifjf.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijylidvf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ntbwbxgi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3rvugkmkj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rpuxmerr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kaxqpuqx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3pzbrmbwy.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zpbvejyy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zyrzqwyi.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3jopghobi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mfhgvnae.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qrjgoien.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nibaxfcr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3srdqpceh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ovjgvcmw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3rdqfnwbg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ieoglvwz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3gjivqvtm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3hyexempz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3osucbyzk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3etottufc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cvfpfnrz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xfelvgvx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3kthvarzd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vhpucmue.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3hvuecmed.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lqlapexk.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tidxgppf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3zqqvsqiy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vexutozc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nldnftnh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jgglziol.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3splrqbeu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ndnzdzeb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ovifsuwx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3xlmuubag.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3mxfitzph.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3pfyykemj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ptsqpooe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ddahnaef.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ktdmcziy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ikfhsems.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3csvzbyna.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3btfcnpgi.html


<!-- 参考信息 -->