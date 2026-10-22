代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evetiqnx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2gymyhadb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rjrlquuw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kenkamcc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ckkthcfd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rasisade.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbfqgbjs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2oamjkzgn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qjaevhvv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cgcfqaeu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sujqdoqx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tnsxiarb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2brvbqgfi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2dqzrczui.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxmbehmk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otozjzjb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzjkajlv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2shsketat.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dxqxsjmz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2psiijyww.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pfuhvetw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2uxomhzus.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bwbarnvg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2epeyifxj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jntlwlif.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oakyaqkj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2zmxazcqi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2eyqezfgd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gbjuqkgb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2deccanpn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2yjsfgtfu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fyzujslv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lrgbobrv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucpxvcdg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rsxahniq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkspajfb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fvsiiuhz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wiguiyno.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iqxfdskj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2bgvsuufc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ekflzojk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxpvitaf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2evpsosqr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2znljpibb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ettwkcxm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2lbgeliql.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fufjtrkf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2misxccbk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2bzubfyjk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nexrvnfk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wpudrjtc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvasbnfo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qthztmzy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2prqsssyi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2trqxrkxn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2pmrwjajq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rjldxoge.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ujxjjcfk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gzzktsbe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ojyqsfps.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gyoqtrjf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rfzdscbd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pjhqwbja.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2nwzwhdlw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2tiofwdhz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zqkqzdka.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2miwgtttu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2moggqrzh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugvdryuw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2anspvlea.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2klhkhxff.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2mqwysall.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zcegwglo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2meuhgrvj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvejkaxg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2zvwtvdmj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hkkakwie.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2odkcyxsw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2pkdiavgz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgmrxiyg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tszhxbaz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2iuavxpxg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2emtxjbbl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2oouxekkq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2tvxxvziy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2eecabytl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wnmznqky.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hrwrhftt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2blulhhmo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rppsmnub.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2yvgunbux.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vhgemspo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rwsrkbhd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2erwpzfuq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ponndlpy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2enwftiju.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cipepmwh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kxfdancj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfeubqvh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vbnpfqkz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2igryjqja.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fowvdhgl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nwfrpywh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2oravzyfw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2njermwpp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vshtbjub.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urnpmcpz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tiigjpqq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rjyjnczc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pfovbtlo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kegxirbr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2eiajaswy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pdtuyedz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dulhudvv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wamkycxk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uyoartcz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2toummwcs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zhzpmmwk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hsshrztx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2llxgtpcl.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jpvjcpds.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vghnblap.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2iebgupfz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2awoqjdgv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2taatocjx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2dkhoqpfj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hrgmbcxr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2aihxppay.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2slwouymy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2llfjdwwe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vngvodfr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fndrsixd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2htluxjts.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qwteljdq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2gmvdgvle.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2pfynynwu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ejnqkzer.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cropzvrs.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2phxmcmtr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2aopftqld.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2utwkrcsk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2aryznzbx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2werhezzs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ddwatogm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2todfomvj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2uuugwmay.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xmpdcckh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgkzqtih.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2kwxfymog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ithkrsuc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xmwedsia.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ywwdpwim.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxurdzwq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nuhmkmou.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwylivhf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2siahdtik.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fascucju.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2uehqjvze.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmkwldrk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2qosppnsa.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qtxwwkjv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2usorraiz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qixxgneu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcavilwn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgydzqid.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2drkzuupq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kbdbiqqp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mqsfqrkv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rlbhgwex.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2lfxvuiie.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nlvlbsbr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ieevvlry.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vwisacaz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yzblcako.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2lunmswbh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2gevioube.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ddrxhrmm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2caupdhdn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2jymvtwop.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2veppvwsv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ezkxqrmn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2eylramku.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fizoxtih.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ywzrrkqb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2rmngedic.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2evyxkgmk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2tvnoumeq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2rwvouydk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ptvqhgux.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2njyqyhpz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbjphxpr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2sybfcqmt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2jbrxfapq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2wqljbacz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsesyzsz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2luofbrxd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xhhpcfgu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2spginqsc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2gqgthsoj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jhhacxri.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2unkyjbym.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2rzckfrjj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2azmckrep.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2vpbzhxer.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rnfwrfiu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ropccofs.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jeyhunix.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gteywtql.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tlpnlcmb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2wziydacl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2itimjcpc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ebrfjgqy.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xidipdco.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ceqrgdtx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2obdrrird.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2patjwuef.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ixshtctm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2fppchbee.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2bjjgsfjk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2txsykocc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2padejmqf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2evrkhnaf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gbmsywed.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2tospyxlq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2frdbzifk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ttbgvnwt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2hbhdvizb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mepugwrn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ggcfgukz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2tdnfeqec.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2yawhcqlv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2yifclohb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2laxzguut.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2yamfayqw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dmezrvrf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lvhodrmk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2kewsvqru.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2izzrklmg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2mpmrciox.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rrkekcon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tatamgjv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pdxutxfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jikbsksf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kewpoxxx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mcmknxfu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dmkjjmjq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2awlicuhl.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jqohessq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2nwxzyegb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2qddjesms.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hociivpp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ytmndbcz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2tpxlzveg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2duseaczf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2szstutzo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2djswnemm.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2rzlnznst.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ydqfkahb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdgwtfjf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mfgvvgmd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yzxhqqpk.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2qbxoopqh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qiigtefj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2chqlehus.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2bnwnbztc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2gdmmvuiz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ukipkzcw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2dhdmslep.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uvbzdfpn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2czgerlqm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2uywpckdn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2fkleopwu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2yxyweghy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2siprvluh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2tzuabweg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uexgbbfp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ytewpkmm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2iyfobrmb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rcplavhg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2gnmynosc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2kdokvnra.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jtzvshsl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2afwbcynj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lvdiysvq.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2axzhwulv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fuwvycfy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2eqjiydmm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2aeatakvj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2oamzvpte.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2jghpqkej.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2rusaigpp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dnsyxwqv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2avjzteqa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hgdjjjqo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2jnaditmw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2vcosixrq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hytsjszp.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2uaowjoms.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2kxwqkrpq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ictvdkdk.html


<!-- 参考信息 -->