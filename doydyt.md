代发 wailian999

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3odfargkx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3mvfwchwm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vgzyeior.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eboyoqym.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxivmjnn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcuzsupv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qqlssdlm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gklwisub.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3oixkhpic.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3folecwxa.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fghepaxa.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3vfixrmff.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zvsayirh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bqltxrzf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tzzspwdo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3tbifqwqp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3phgpwhoz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qdxsiejy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vtesmava.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3drlafrjz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pvcuowls.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ucqharsj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3deowqygs.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkdezxuz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3cnnetsco.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3xmwfqblk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvcvzbha.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bwtpajsw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3jyizdahg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3gceicqro.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gqxulzvy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ckzxnlkc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pmtmnphb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wqarborm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3neivlose.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkmgewky.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vgjlvpkh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xrntxxij.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ltzokevx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3aajzndyg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cfmzosnp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ahdnomkx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fkwgzqsn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3imhuafkn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ukqgbyla.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3iojfpmzs.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3eljiygmx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yxmrshat.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kkhnqxvl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdrffolr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uocvorxn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fzmjhdlh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3duhhgkpk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mzqjsmmr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3oqurkbzg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3evhijrdi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uhxdljwr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kextftth.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qplhehwz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tewjmbiw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gpmugdcz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gwlngooz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uvqznffg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3sqfssrfe.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3szltzgtc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xtpazboz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3goqndkts.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hsclejrn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oyflyqjf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nmasmyoj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vrhljgxe.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3cjyuskux.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3uzfbwetd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3adzyikvr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3bpbhocrl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3tirkxriu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3niaznryh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ohkrngxk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hgjsiqik.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ykmyzlcq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3jkmcbtks.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3bylkqzyt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dskydpjd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfjynftw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3verwxjvz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kxkhczef.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ovdeahqn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jjopxgmr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rtgjbxzv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3umxhhtvd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3oieodkyy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3smogsygl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3uhuanpda.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ewrrelqz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nffzjvjx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ntnwyvwp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3tdgmkpbi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ielytarg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3esarkjkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojqodaep.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3srrhcsky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgpluwfh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3wgupmdos.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ucmuoooq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3oecbyutl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtaimezy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lotnlovs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3swiuwzjt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3yehdxzdk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3auwexznb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wqgtzawi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3desojezg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3gctcnysx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ssotgcqi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bzmkltyy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ztwhdswu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mzewmsjr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3relvppvv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3eeughedd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dnhvvjpk.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3arnxqnhn.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3juofeprf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xncbonwv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mrhciqbi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cwcchzur.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3clqxddvg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bfjpssnz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ojhptnab.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xbnssvmb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3rctlsoiq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rwiqeium.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yxvxqenv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3svzkhufi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfzilfav.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fczekixp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3reopxjwt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3yizrkdbx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaomhflf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3qlbzjflw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3bfkxmqoh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3pdzlxdlc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jyaedvip.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqixxblr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3zgymyyzn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3awwikuzh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3pmdvybyw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qctzszhn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ggsooetp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3penxisbl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bgqmkaao.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ugbztsqw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3asvbnlbu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ecbxvvtj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3zxdfnpwe.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3dnrqniwv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3iptfblwf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3bcxwoipd.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3arwixpla.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gbnxkolb.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3npxzabig.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xoxhhlvv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3plosxaoz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3jvhmupsj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3pbxbgkbd.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hvcactyw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3gsmoazsg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3lqqanwem.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3bpvoqkgf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3rvuenqms.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3oftrbqtq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3awkztkya.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3okxfjkpv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3miibnrbw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ujvomkwk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ousordex.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3onkeuirn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3uneekmnv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3zvkfhdgz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3yxbuvpjb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3amyngkgj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3vupzidkb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3dgebnamd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3jcqcowfw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3wcorowmk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3nbxzalhf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3bgoxuokz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vxeazkfq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zyvibwdq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3uvjhovzz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ytmsbknk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3bjszgtyr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gyhmnvtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpttvpgh.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3elfumbmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azksbqcl.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3snxppztb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3guowkrka.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hlavkamf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ozvgqwda.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qymuecui.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3kdhxuijx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajhabsna.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fyikrckr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3keacxfts.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3smuaguva.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3dyhubtrw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jggxxrbk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3hpsjwllp.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3efbadeor.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3kjujkwxz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mkozacmb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jwchuxoe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3izouudzk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3qzpoyvqo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgudmqfv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3irkvhici.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ugxbkyvn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3xlfdojrg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3enhholqi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3yxyoeksx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3iouvmngk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3tdziiahs.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ouesyaum.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3nkovrotr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nbeyihlo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3aiqsuudw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nesodnwo.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3furznpug.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ilszvppp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3tdwbgcgy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3etstoacd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3jtjbkufk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3naquhnhh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vatxxefs.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rloszoxb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3gabznzeq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3pdzgtbtp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3trjuqofj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lkfcvxwi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wffwibwx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3iuabcupb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bthnggaz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3mqgntrjs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3zbjlyecf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3sdjowtrt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jbeilxjb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3odliaczj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3azpblnek.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ckqoufka.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3eobrxvvm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3iryabnjy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ymbxaymr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3clurznsn.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3rdmjsdlr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3alsievjh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3qgwesoyc.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3kaiqbaes.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3swairkgg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3vgqkoilg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ovdnmrhi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dldwvptu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hlusnfan.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3tqprpyoq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zzvdzedh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3ktscjqsc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3nvoclatd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ylhbvvsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfdxuras.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3gjpdekzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xyglgkrd.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3xjmgkwar.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ddyinfpv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3teouycvn.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3yoiwtvwn.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ecvvxhhy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fxcizfmg.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3mmuemhjg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3jvgoycfh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ilslipdg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3eomaacsi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3thkzkbjj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ejypvxbh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3amcfklqr.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3jicketad.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3zfmecqps.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3odquozrp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3bdyptcwl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3slcelfao.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ykxuowpm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ggshwncb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3nihzfsyg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fbscsure.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qdhgdcra.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lapemfwb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3szfcjnhm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yptyzmqq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3dmprhifg.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3stafpjeg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3bfxldqkj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3edeysvqj.html


<!-- 参考信息 -->