代发 wailian999

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3llbdrwte.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcqtwofg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qrepxzme.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkpwcity.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xhbtdvec.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wjtoaiii.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvabmaqo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cunxbmcb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wbffzjnh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jbcbxkxf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3envhubck.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sweioeth.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wdmyeipx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndddudfs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3yrzpkdax.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3sqjyzqkm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3rndcnsph.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tfglgrmw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3sxxhospr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3glsojerb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zckboiwa.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nqxvtryc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3spiiazby.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3akssyrzd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3smqmiopy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3wzpekqds.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3hpplyorx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bujobvmv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zecddnjg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3gvpunady.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3melkrpbf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvbredbd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jmrobtxn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ukltotjd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3guyrelpw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3zpurndir.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3utczusud.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3mojglemn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zdzwvzfs.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3szxcrkxr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zeqofjvd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3vvamtlid.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3dhusfouf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wrrkflrc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3tuejscje.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xpycbzup.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kfmeuofe.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3upuucinv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kzsmdnvo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vlpcepbw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3urkifyeg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zdxjlupw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3awxxvesz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3dllrtbpb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xcwnxphb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nqkeirnq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dqzfxvhm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbpurexz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cnyxqtsy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3efmazhwc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lsffwnon.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3khimlgzn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jzfheavs.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3inzshmfh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vpccdpew.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3snzktifv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sgffiegz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsfguttx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tzierftz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oxhsuyya.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zqxhgzhb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3riehxlnv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3dfpaktiu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kzgecsfk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cpkqsxry.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3epqilsuh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pdagaxfk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3asizyvau.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ljmnbjoe.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3jexkxflv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ygjyiwcb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3atxgcefr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3tojligwu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ufejnikr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3nrorooju.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3uldqnjwl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3oxemgemj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3cnbiepye.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kzmcyzsg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3czivbbgw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vfhqwbhj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3psryymgi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3dyiwptti.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ftvnbjim.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3miniimzh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3gzufmdst.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3aebfdhua.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ksefujto.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ccgpefci.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dvdhmwuy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3yoknhihn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wmkqhscw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mfwmuueh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jmtfttqi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rkuhrtlj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3fkgvoqfm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dkzxeeoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwkmuhvv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3tveafire.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aivoounh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3juheuitt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3rejcrlvh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqvavikd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmgtvumv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jkzgcllv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3uogihilh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qinzhrdv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3kebalgon.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3mgzdpwlm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3blrjcbhw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3chbkcwdq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxioalqm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sctpbpyd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3aebvjntg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fizypajt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3klcxyoux.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3yjnziggo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pjpfujia.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pjmkvquh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3mkoweopq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yjygivlf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uwbdytrf.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mowemzzu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3btwnfpkq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3xzxkiwbc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3rsclyfyc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3seyjjjml.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3vphkegrh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ojaikllr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmykcegl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3yohqwiuy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xburpcad.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qujkkzhe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3dqhazqpm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3gstkpjru.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3avtpnfmo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ktoqcimg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3xklpgmpi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3bkcmzjgb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljkxhhtj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pspwnxkg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3soobfebz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3zwrqhveb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3zzypsyes.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqzacjri.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3eyinxgev.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3zfbgncrw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sdicwzys.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bdcdccjq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rbufxqnb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3vaewxwsd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3anqmazfi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3bjrewgvy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3onppjdft.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3krjywnze.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3zopdqtod.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bfkbwiyc.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qzucieip.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3crrkzium.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3hixvhvsq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3lkjmcnei.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3qoavcmqw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cbxkalti.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3vifmejnk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3smnxopac.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3bljuwltb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3zwuoqwrh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dtquyrgh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3owxiumqr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3qnqwoqqp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3pprfdapz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3jpcpyejx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3nslebucv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3msgmmeur.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3aymofvwk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3goeazqcp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3wkukcbek.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3otsvtvsa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kribxgsr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3thqhazcc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3azgahvgh.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3hjpmshcr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3zdojtgmc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3btwemxcr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3oaariqbe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3kctsjads.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3tgcoqeqi.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3kswzayqv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3nwjqucvh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3obzbsbrr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpokxmsr.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qthfjpwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wogzvreo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3fteepyvr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jfrafnqg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mxrrdilx.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mffwjfyt.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tamyapal.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3dqbyeobx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kdbrmdsk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wrigkvjm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vnpgqgdm.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dahyeady.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3piefutwc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mqtfvzig.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3whihlfvk.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3yywqozjq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3xrnjfjas.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ptdfryyg.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3edfkswvh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mpsyclus.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3tchmsrtf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3fxebxezm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3iwehzuut.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3uvtbhsgh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vyudwjls.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3xgcanrgk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3zymnrcem.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3szqnjpez.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3iehuntjp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3yyrtyweq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3zluqhyzy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3muirwcxd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cihvhyxk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3mzsqjxzu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3seerswrc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ygneqkjg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ifkypzao.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jdkuvepb.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3xmodfxgu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zkxsbpvp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dgsnefkh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3czdkqawg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3sywzwsxt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3fwnadrwp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3awgfghfd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fzfsuztw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3lauozjco.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3vfcrfepp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xixxbqis.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ddkgvjmr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bocogmpl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3nhwmzrys.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3lvqukncd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3xvvrbfan.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3mfdxowff.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dyeohafk.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3huntprdm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3tzewkqfq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xbriryer.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ggafcmxl.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3upmmektv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3jqmyurib.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3culavqua.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3hqfqezsi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3sabaugil.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3jemvmttl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3cznoxima.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3frwxcles.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3fynpdjkj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3asqgqixw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3cwawzvwz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3eadfzzbo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3lgebmzfz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ijgmicsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmnexngw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ffvvshyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ueadbief.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3uufkqfub.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3tgqowvav.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3lnwyayff.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mulmygap.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3uzsihrxm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hsqvohrm.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3qsjofgwh.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ekfmowly.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3peajoywd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3gyvtpwvv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3rtyjuxnu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qwnzggfo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3uybelugo.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ipccfbzp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3rqgwvujn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3hfyxcyku.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rifnawmy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3azzffjrt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ommuarcn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3ovpqugtb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3glaseaua.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wbvtvbai.html


<!-- 参考信息 -->