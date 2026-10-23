代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atajibnz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tfqiyzje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvaykrcj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rlwojntf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3pukefdhb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oldbaqel.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nemupwtw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ommxxssf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3suftsxkg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3oqevxgzc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ysqvpedc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhcqugzh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3gpvqopqi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3rmsdqbeq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3zkcynbra.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbiyiqsc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fmcnjosx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mfpqzjmy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lgpaecac.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3woaxldyo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtiwvulo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3wkmmqmzj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3eamdaplh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qmswhovj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wjokpney.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jrdlawtj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3hvgfyxob.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3iczkdmsd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lbpwwvxn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yincrddh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ogwtivco.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3puqhdmjc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hjzjrqtd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwndxqth.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nvtjhuhg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwduqtkp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3udcadtnj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3aldqujmz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vslzzbty.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3efzkqsei.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ydaqweqr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyssgifm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mczqcpda.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dyajkrzh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfkvwsvw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3cknxvatj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zmnuympt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sclyibta.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3fnpezysr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3tigtxgoi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ykmoltrf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bzvlbewx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pkdlljzd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eicyaiqj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3keyatnrz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ncikeorj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3bgeqfoxz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3lgbpntlv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3plpojrcy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zkdihmxp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tfgxtujr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bspmmbjh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wujutvak.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3pegrpbts.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vqfwfwit.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xhwqwsvt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3azauoezf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wetfnjlv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3auvhikzw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mawsfxbv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ehmoolpm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjndotnf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3edwemeui.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3kedmfgol.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wypmrjnx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3abigpozk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3oeucikaf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vblasxjp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rbsetktp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3uyfcndrs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zdsltjsz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3njdntawp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3cbotdtoa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oygbldzj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zrqtfwst.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3yekvnxbx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3csmcrouo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gtyxqsah.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tcibrqhz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qqzgihtw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vaazcxst.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rfgzkggt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ikruvphz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zihjztzv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pslwwsbd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvpcmsli.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oglmqcqd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kyiwjijb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdwrlvid.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3omljkcmi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3onociwxs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcobhwga.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3glxkmazg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3thnkyqxp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yychemdx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqfbmvqj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zuuzqnnq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmxbtaqu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hdsoiymt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cxiawhxx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hjzjpfdo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3pwgumimz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uvvkvdje.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rpffzbti.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pfwqwfwq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iquokkun.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ogbwygxw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3btdpqett.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hnffxsua.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3syyswqnc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3wylozmbb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xczdgzmb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xaemabui.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ocimxfzj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3rxbezgbx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3vnauekqp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3fkhggjab.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3yzrcdopk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3jzqgvdcx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jzbbquse.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3djlzlfft.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yamaznuj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xpqkbiwd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cahthnhy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ytmswusb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3xbdaibwc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ruhjghbu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3inxdnrtk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3dumzmcri.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3osamhehs.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3yxpjublv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3clohjopd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fvujkrca.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qhwdledi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3baagnmec.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zlpihdzt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bgbreeca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kldhgxae.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3reoezxgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ueklzcqj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qrshlntf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3znxeoqaq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3olrzwneu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wlisyzql.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pswutwis.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3fyghjzsj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3epxuzpev.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3mqqvzgsq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofwdbzby.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3olpktnnf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3mjmxwmtw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3psnbvqeq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsmdpozv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqnwsvjp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yjoftjyn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3pjnduzmm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3kmmrpmmv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qguguujv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3crjjkabu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3towqsakj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qyiswtzo.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ybvabejx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nubmfpfz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lovqkgth.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3wvvtilvp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3pdcmwfbe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wvbrcgne.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3mhxyhnop.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yrorpnrt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3odgkmlkr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jilbhict.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3cfsabmzf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hyrkrzqo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3cvxtptgi.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3byonxlgt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdixpywo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vkkoeyzq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3gordikuk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ymxdrwol.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yygynjre.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqmpfuqr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phtxhnwp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3awwzrumn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ojlztrvp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwquvljq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3udiclsxg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3cuazroxz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yfmrzdrh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3wxzhqvkd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tkfibpxq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qqiknqyv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3oulxfwnc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3wfmkrscc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iqlonrcb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3uhyjaxeu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ngrefrgc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xrzgwkcg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3drmwrmhc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pweibfcg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3yrrmsdhv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3fqsqcbmu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3juooyncx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cckiqgst.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3rgytqufx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3gswlwjwq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3bfdpjcet.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3straogbf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3scvrvbxw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3usnrpbyc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3awpmqbml.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ubmxfsmj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3eomtoiuf.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3pfeczkbq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3itmqhsgi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3wkxsiwxi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3isfxfcli.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3cgmnqoec.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3nwisbtpt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xgmpouta.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3qimccohk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3opxdkdop.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qmhjojfa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3prczukke.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3qfkdnxwj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3suamqnuh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3diawpzqh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ibaocuon.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3tnenwnvz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3mdxfxeaq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vpyulsvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epkobhud.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3zvndufcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltdzglkt.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ikvedzur.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3whvkpmsc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ozfbmqoo.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dddagwim.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdhesxzx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3pqvjwfxq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dyujaybr.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kpbsoqll.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pavzdeyj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3iufsfcas.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kxbylaco.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3pddqrxmn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3qytptwen.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3jmchiwld.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3jujdhsdh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3cniyqaok.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3eiijahqr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wikzbhbo.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3bjdnacqn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ycvfspef.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ngbtlggm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xetipecc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iwlymabd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lfsfecnk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3emqlxiev.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wuruchgd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3dbjgvbhz.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ozxyudcd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3luxacxfn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gmcrokvd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vvdmqlsk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3avxgtptf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dpcqyphv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3otjrodww.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3nhuoktku.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zonczddw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xggdhkvb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ngzviojr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jxwaoddg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lcanzcqn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3yfzdmhuf.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3kvzabbsm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3uxlanmoh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qahjqite.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ocvplprf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3pfmudjmx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ddvnzsch.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3mevbprib.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3dbdcrjxl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3vgjdygan.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3blqbogyv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3elnssbrb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3gsyinpkl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3aqvuavyl.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3bsyhtgqk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3cjmwvxsp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3oscxiiih.html


<!-- 参考信息 -->