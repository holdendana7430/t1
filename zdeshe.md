代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fomicrao.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jgbhvrwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yoxslatu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nadvzisp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2vtkaftwb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zyuyfekh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wubtpkhu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2heteksvc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlxssoxm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nbvacwld.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hhanoocx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sadgiatg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ejfsasul.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2cfmgvfie.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2wleybwbn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjirrmtx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nidtxsvt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gppkcgeo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2kfjfyssv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2koscnxeh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qpcmzndr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lbnroqdg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gqdftdom.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2masxatxv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jriinuxf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vickubpj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2cwfvapkg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2bnhyxdul.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fiqrubpc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qjglowwn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2acnspjlg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bmzeypte.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hdrbmegx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynyexmol.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kgmtndhj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgofujiq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iikmjbpr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vjbreyrn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yjgaglnw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2waqoqbpr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2unukcpio.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zzoqgnof.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wropaaba.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ezrjqlcc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fppcuuky.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wazbtpwu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hbmhlucv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wvilnqyb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jlqtznje.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2pffzdgzk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyirqrhu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aaweyirm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dwirrpme.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxdlnswi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2yksheipm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ikqicebq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vdztabmy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2kcpwpbia.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xosqulex.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2locqwdnq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2titnqlfb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nrusbnka.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2iznqbtav.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2deeepzwn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2yigsqbug.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cyzlkbly.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2sskohpcc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2nyvmykug.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqrgotaj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2zltedcen.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvvdxflz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lubkafwz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2tqxknxzl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2svbjqrte.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pukqhdjd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2azaqjawx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2jiinszwx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2tenzfyfx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ieokoctr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2uxkhbpeu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yygmefhg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2hxnlkuzy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ecnczhgp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcbvlcsd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mlggdukp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jjeetrei.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uupcwgek.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2duqaivgn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vasjmbcd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2wgmkegwl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2uuzwsyej.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2aeiepfbs.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wdfmhscq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ljqzhbtn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2sgcgnpgt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfnwkelr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aupqqbey.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2twflyiue.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xukehyor.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2roygdtgb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qznpkxos.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2iqazzlei.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fkkelvkd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zdqcdyvy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aqjttagd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vbwptlol.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kirblpbf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcxoclpq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xxzeomel.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gebqwhtn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cdvisjoi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2dgjkxqpn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pjdxzjmu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vazvzesv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pinrzoyp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2snjtypdc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2enmdmjsb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ntxbcmzs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2srawkpos.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ppdqkppp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2dgqwocqz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2oacnizno.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2veyeungw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wcgnlpep.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xltsdgtm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfpgzhlw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2qntphkeo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ghlfjcgh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2kgfvlrrj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tvnfyuul.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2wqiczdha.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2caduywzv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2kijhgzyx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mokmdgku.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ydsdtjgw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2fmluoubc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2iaesygqi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2otmlnwnt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vvknuqyp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ynnzfrqp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bzvpdchm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2otefykgo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sxyjhquh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jqhvbbnz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2acyrdpga.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lwhlhkju.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xtgamhdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwipdcsx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zwgivneu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tduvfvjf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2jntympfa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fnqnvcbg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpcqnchj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cundvmvi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2byratozt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ktsitoxw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ffxsrayc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2mbcmdkdn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qckwcxtr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2dihplnif.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fvaljwxs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uorsebtx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bmdbnjrx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvaikcdj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlirmtge.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zgfcnbvg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wtwynpwj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nkpfnzzj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mxjyhnjm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2skshhoyz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pokzdlav.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2raoemmjh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ldhxvvla.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2egxrookj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2czlrbgmh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2oxxykhtb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ndowbbcd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2jhwijtjp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2roznlkgh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbehcsvr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kowliloa.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jiujobtl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywujpcsh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2wuebaeke.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcsbskyw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipjpavap.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2mdilrlld.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hmwhktbl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2iyugirlk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rxsgmoeb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qkeleaar.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2pdmvkazm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2mxsfukvh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2yayrvmaq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kieghpqk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2gngigvlt.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2cnhatwyg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hmuffgwz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gayweoku.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ovmmovwb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2uafcqtus.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2wdevvsyt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2fybxzolf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2wwgkqjty.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2whretozp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2qrxkalai.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2odisarud.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fadhhzsf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kbzrvsxa.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2duegzvvy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2jripqopx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2isedquhl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zdcvjofv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2gqwxkafz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hhkoizgn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2sfhxhmym.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2irnqvlgw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2oluwnznm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2nowcxpbb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2aznyczok.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2kswtczun.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2qcazuotj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2cgpsvcaa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2khuqckil.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ytpiqnwr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2bshjqlmf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ztezjwyp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2scdjgdea.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2qrmbghel.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2vmwlzova.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2fbrgfnlf.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2iyusrjsq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ztavnkbn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vejhoqey.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bvzmpcqk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vfzfnmxi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2xlhuykil.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2omxahodl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2gldgkmqo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gnoorczo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajfdobin.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2eztxtxyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjaeujmh.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dtduorqq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2aveiaicr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fnmvlfbv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2crewskzm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2icopffgv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2jlqzqxiu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ktdkyrjl.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ktcjizym.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wejuolhf.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sbtzvowl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zuezzqxk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2vjocrszo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2glpswjui.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ztibnbry.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jtqktzpx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyjclslc.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bnlxrjfr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fxhdojtx.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2rkvxhjum.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ovfhlexn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uhukpqwq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2dtvfybqr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2spcyahgs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2iuwohnom.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2kgsrnkvh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2soqhznfc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2puopwzif.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2wvjgndfl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2pxgrkiww.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ocscvwod.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2byuxymgg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fozgxmoq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2napvcrvr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2mdkagwql.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2aetkziio.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2jufkggdb.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2khcpjkut.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2cydsslze.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2exhzfvbk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kyequsxv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2suadkbyi.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2wahjsvah.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bwxniqts.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2yihsfqev.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qiijcacg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2jlrnqdui.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2yxmsiwgq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2udkanjoj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2uhmkfkvc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2oqttbhoo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2aseyotla.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2rlsekfbj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2dbfdsgbi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2augdzupm.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2pmxvxqku.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2pjrqafpd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2hekhouhk.html


<!-- 参考信息 -->