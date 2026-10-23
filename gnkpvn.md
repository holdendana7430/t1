代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3wlchtiwx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vterevrk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3alaopprp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3frxxytsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfdwvwwz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wsnrtwro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tnjmuabz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3sblumonj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3efqotdil.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jzninknn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnrbjevp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3yfhrhhim.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3huenaxpn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ydnlwmth.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ynmlprfe.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3llkmzasr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmmadcir.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kzsderqe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gbeokofs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ugtrhzji.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3udmujhvi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fiqlnjlc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3fyqoiflb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3uuwbtmll.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vwqqinzg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3nntbqtqi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ibqllxfc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3snirkgbj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gyhamuxz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3onmtyrvq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3gpklrudu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vmxltdlz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3csjvtvmi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3emaiebdq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wzekffly.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vtqydrlo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fvbuzign.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fosvmbxb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fypgtdrl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gaqhrxpx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rxniibja.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vgckyxwk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nbvctcyl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ybplbfgq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3geuystud.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hceaugiv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqsmfxvx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yxdvqdjy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rpxcgbew.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rocvbosp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3huoxhbwn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3vpynlayd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3lnrjfvsq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jzanhpah.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3evajajnh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiuaszfo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yrvhticp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fzxvlclg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3nourqhwc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qqdvdvlm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xoxcipxd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gxjhzpmh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3omcfwcnj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3fggbjfsq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tstdphkd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dquerwmk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jidhblja.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kuchjupm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3crcpebog.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3uszslhzq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3tjwuuebu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rdszuuig.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tttjiqhm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lktqnrhi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibpavbdt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lfnbdisu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3cihhxazt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qvpzujyp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3qdwyzvat.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jvokpkwx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3breuxgvc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bytfuuvq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3xoocsbtt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ohhpnegy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kouzmufr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3shlasfit.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rnoviazl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xqpnmpwi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3lokalrfu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3wnerytma.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cmwnscus.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ekhqdjir.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3axlbozio.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dbwtrxir.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ykjttksl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wduyqcec.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3gtcxnwul.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3kkthofph.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xsfovweg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3stxzeifq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3thrbbwmi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsirjquy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgvayqwo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tboopjbs.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3btlnkjyj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3edvrcwgb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3eieqqbhm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rcrgpoit.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3flelwivl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qkjiplpp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ledytmyy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brvvjjgs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vhydwetz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qnevfihz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bbtlarqu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3zittsfhw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3fbmrxqxd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cwmxiibp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fjjcgjdk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3llecuzti.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dcpohfdg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3typzllem.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3raanegfo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3cjennxbl.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3pxjnwndn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xcyqknsn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hrntbrsy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3nkdavdyv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xmwvnxwx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3estjujbl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3zuejgvfd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hlshvrbp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vimdmren.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3hahflgtp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lvgyfvgc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ybqmhdxn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ubfoqbhj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fnkrvbyh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vdfmylhr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mcryiagg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nprtvvjt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rxruqsip.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3xmyqtvpf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3nzwidvps.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ygeuzajg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3idqztnkb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nirnljaq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3gweddmsm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ibwalttx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3wviradof.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hjsvnkjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yimrnafg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3kvlofpye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dddsmvou.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3dpsfwekg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3sqftgacu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3deiefuku.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3octnvpgq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jwpfcgjt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gxijmbgi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3dfccqqbv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qvhkzyvr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vbgpvyvo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3lekytahq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3emrjdmwt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cjdbfvsy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3prnihaqz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3opmvlphw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iwqcgpjn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3dwtqraad.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3dnlktcxp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xsxwndzl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3locblcrs.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3fxjbtjrl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vqrptvid.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dbvtqmwe.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fshjkygz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3arowoqpl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3btidlxle.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3jzqqevbh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rngewduu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3hxirizop.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3usghlbvy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfpsccqh.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3rzbbqbfm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3msvzrqek.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qpcmylkw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3urohjbis.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3hpavjoic.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3srwbbczh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bksasdtu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ogwoyzlv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3aiturwqc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbpgyoyd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcojrrbf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmrwmshm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3jaxzlhjt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3eabfvove.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rkytyitr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3nrrfbshd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3meqofalr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kxvtbbxo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bqntpmfj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ftgxdexf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3tslijgcz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3afhvhbwh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3horzawjv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lbcswkce.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3kutyetzs.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ajuprtlm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ockbxdmd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hhlpsgee.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rqyqqwjf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3tddmadza.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3eamqdekc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3bxdwefdk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tjdqjuke.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3qnjygnrs.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3vwmxrnej.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3kdhxlcer.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ataieucl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3potnlbel.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3nmtpkofh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ahwuuelt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3azewgpiq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3yinrisws.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3riplgjnl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3zagmnfdv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3icieymfr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3dkwpyqge.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3jsiwahqm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dxfwjjkq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pbougeuh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3mfjvpmyt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3egevgyvr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3uwofkvgy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3abkvrlnu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3nampfkuq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hgdefkde.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ctczwxkt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3gvwsegkr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3gwrvptjj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3lvsoethz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vqirynhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irhumeyr.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jnkdcmbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkoshapy.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ertxfbxj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3bszjmxcj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rovrewlj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jdexezww.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tfevplqm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3getbgubq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3utkqedgo.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bsgcjifi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3qtviepir.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3nxboogcl.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dldvxeey.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3riaxkvql.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3qibnukzw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jhqwfbya.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jbkigmil.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwforjky.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qsdbylnv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3evbopqnl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3sruxcgcs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3phnmmeat.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3sfonotrx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ncggomxg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ikkwrqos.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3qujkwzbj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3csfxmmtx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zuehsqqt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3mjyxvumn.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3aucklowp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vdxpqtif.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zvvulitn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ibvhypnf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zsjkktdd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xdndekmx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mrtjmbmh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fhznvfak.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xdqrbovp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3alabaqed.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hlqfqfdq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hcmxhmge.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zuhxwasx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hkvedqrt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3bunorcpd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ubbeqrfc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3umwkanvi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3vvfgdukn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3odofipce.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kcgtbbcg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3vijncvcj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bxeijmbo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3pjyxqdun.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tabcdokn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3mjejzjxx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3gzveqnyy.html


<!-- 参考信息 -->