代发 wailian999

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xtkbxjpm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rivydlxr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ngjsnnoa.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wtzyqpkx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ziiwfhiz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kaomonao.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3eevzprln.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzvbsylm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jccqlhbh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3phoxpmro.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhgilrqz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wcezqama.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3faaazzup.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3njpjjtnu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lovalpow.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jrahmwke.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3czkmqwuc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3hibbnrqy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gythlzar.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sbbvzpbj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qasatkxm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wfdgncwx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nvrnzowl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jxmizmkv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3juvfcrhp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fcjcwjnw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ltxvdbwl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jhauzmei.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbrbyuyj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzhxlmae.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fjqobrez.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3prqiwkzp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qkwtsvvg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3lilejtzl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3avepdzqw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3onhjurbl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3bgmkfyde.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnyeuxac.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3pslyqhjb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dfjfrunu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vfatxvdi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kwinjkfs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3njxnqegh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzqtnxrh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gltgofyz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3aarhrngu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rkdcjpys.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3orryehpc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tqekrhwa.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wrhhblua.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hzpwfvzq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3phthxuze.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3sivsxpkz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mdjcrafj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3odlpoxfh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rtyspldg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3aflbibsm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uyqcmxan.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bicjazay.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lzhwmjso.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3iephthja.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wnoruybv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ccfhcvdz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3niyavgzd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtqxxpji.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jxbjehwn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcxdlwpe.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3njxuloqm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3osuikuiz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3iufdcunt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xankxkoj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3fgcyjpoq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3fqewwnfa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lappujvo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xyasviyj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pgfeexsh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dcvtzfwb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vnaspxde.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vhfvnkks.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3tkziqaml.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3axrxaphy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qyafhiqk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3zctswmfs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3zxzcxyhv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3drvlpcky.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmhxaixx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3htooxmkv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3bdxomgdd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3rhpatvbu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vahznkie.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ducjpyal.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlonhymu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3aeplniym.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bykbhkll.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3phkcsncp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qtykzftw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wufxvowg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zubatyud.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3dhfjwdgw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3bjxyrxco.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3yhwakxvp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gzuspwxy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xzxlfxsx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3sjslxgnj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3mjkcbzww.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ujhddqxs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zzdonarn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uoccclvm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lotggtbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwzarlof.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3rmtpktkd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pqgozkkz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqmsneof.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukyxkqxr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwvwbvuc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hejvhebo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tukjybbo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3phruggpf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3wuvvllqc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3imcbcpmj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3vuschmdd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijrygovg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wienstsc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eijjmryq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hzwiwgnj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3rqcoswtz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3lhqeaqin.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oifboemv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3quhhmkao.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wldnflcd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yxcqdlrl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ajmralzm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mifxzxkd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gomlylxb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3lwjujfmx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3bzlwsmjv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mkezkoih.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3kgshjumh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ulblgvcl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3chdmpgwe.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3asestmsb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ivirosul.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbtegjsi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wmeoxpuz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3nsubjxyl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzjsktnn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3atyvrvys.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3aaphpvrq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3zfxtmncv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3innktyuu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jtchucfy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fakoqqwy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3sevzxpgp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3rcvppvnc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3dkvvhvyx.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qivatadm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3egwiezek.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3bphhebwx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xncpthgh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qveuktnl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3nxidwvop.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3aqeswhii.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3wuysxgzp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jordqnuf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3fdlcjhkz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3jomgissl.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oezsocoo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gloqiahl.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3iuvrwwxf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3luebkttl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3pzcfvbrn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pokqmlfw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kjalejvc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3bupxkejo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3rxmflfsq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zqeulyai.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3uftgddxj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3njkflajf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3iocqfosf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ugtrcynf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ssrejhdp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3fxhjxooj.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3zyubrpiq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3jjsruisy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ibacattv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3bkcfkcnt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3cauumeud.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3snlcdjvf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3unrroica.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3qpvbjnnv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3sqdkgkrx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3uckyxqfn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3khufqamx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3pglgijsq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tlgcfoxq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xiskmffz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3vzzfbqgj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3suqjkaia.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3vrlzwvkh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wfyjcnqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgvbxqoh.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dwdhhrki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3giicbxvi.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ogogfojo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3celafigo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zlkejpbj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvxvdgca.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfbcapnl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ibrihkws.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3epzlespd.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zavrsgdd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ytbcvgtq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3usnukljm.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3uyxhtqhc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3wyetwbyu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ntwyhvai.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3rygtipce.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3txnzwfjh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xcamxdqv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rcrhfhnd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ekjlefhz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3kuxlytmx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3mvkngosk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3aofdkmza.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3pwrknxsb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3rgnrbmip.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3wxewiwpg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3xwshyyfp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ptofinjv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3dwkwpnef.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3csrozbjx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iorygpnt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ujgcvnlh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mkrfmxlq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3jruxbxdv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jjrzclso.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ljiqgdzj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vylotmep.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nexowzne.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wktgrkeh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ysuowiuc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jfszhwwt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3eqgixpph.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3vnrtrggp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3llxzcouu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kaaavycy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ejjfdrrj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3pghhdkdm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3siktfzof.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3iztrkxtq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3qlytlabt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3xxngwlbi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3cebmbrla.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3uwcnbegp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3zsahkrjh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3jhjhuefk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ikvrbxlu.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3lvsqylqm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3jgbqrafn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ltbqeyxe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3lhehzebm.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3jepcmqze.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3rfevryvv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3fdkqtrcv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3dyxhrztp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3nbbwkdiq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cnynddrs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3bzrohksl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3pqvrgolv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gconrdfr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3lsxgzcjl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ilbyklgs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3fdjmtkqe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3xbltrrqy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3gnatxorj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mglswasm.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3syuztscn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drwntmkq.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wvkfqxbl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3jadpkqzw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3gcjzlphe.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tbsefaxu.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ccpkmcqk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3qgottwvb.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3pltinrrq.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3basusuvj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3azisqmni.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3chowchaf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3inbkoqxc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3fllujopj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3dtylmhbd.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ookpsbwa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3pfnmdvcs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3jxdxabfn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3tneymsrm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3rxydkgdc.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3spdbvwxp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3cbznwslz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3bqfezgmb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vwcifsex.html


<!-- 参考信息 -->