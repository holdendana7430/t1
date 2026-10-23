代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3asdntwkb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rewjxupi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qhzeyldc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnnbtdwn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ujodxqxu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ywrnjaeo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3haprppae.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zupofvwv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3julhnzml.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vlaffpio.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wncrbckj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wapwardq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwismjig.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkutqsar.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3nfjuwqrt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mqdxswqv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3bnolniwk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ujegteja.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3qeepqgnr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dktyeklr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ctzdtzmj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rjuxhbbo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yryekqae.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3djhwuvlu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3giywdgvk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3kfzmzezi.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3elzxukuo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3poppzddl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wruoxzex.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3olvuuwws.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3upndluwn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3sawtpxnx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vhmjhccg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3nrrzmvhw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnpuyqhy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3rggydsbc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3xzhjeqxf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3flyhxqat.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3sqsfhixr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pspgiqaj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3znjsugrv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rjtvewey.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3iplbhuph.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ypybynhc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3kqnrxlhi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3cjvxriis.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3aajbxbuu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3itzazxnd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nbucmmol.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3unzbqpfi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3uozqnymu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lkppyuns.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bipdtglp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bmwtrrxc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3apstzvra.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwulfnmg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrkmrswj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3crsqwgre.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wemrguby.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cwjvsrvi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3pwuuoqqx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3zaxtaphy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iprqybej.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ylphvxnd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzhobcpc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wvifvbqt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgsccfhy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3muwdfayt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wbxizgvx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbcqlzto.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qhbxkuba.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rghtnjdg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wrrqlgsw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fzucddlr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3btceljzy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3teusiiqt.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rwgoesdy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3brktrwjx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jokavjkm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3anxashep.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fzlpnglf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mtjgltjr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ldggxdcn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3uqrtsfce.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cxzzmuks.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ncponvvv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bpwzyfmd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zsoilvhh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3yrpyffmy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3yezmtbtg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lvjpuaeq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hxtdjvny.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lbzogppy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bpsfgkbn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ybvwkxfz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3szfhebny.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wilffdyp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3curlgpug.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ltgivexm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3evuvhokh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3obmxkytq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dtgqhdko.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qtlmbmlh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jozhntdu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3jkrunidy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ukwrpkvn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3uliuimpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iisradtu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ythkqhjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aegstdov.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3etrmigic.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ntjnwdxn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3sowkvikw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oumbuwmg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjjfumou.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dkepgqsk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wbjsfkkt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3nrmrmwtt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3rfrbiojr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3dxuecgea.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3raautnop.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ibsuipdp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hcbkrmxb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3blcdgdit.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xftixmep.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3lfzcujjf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3kykqxkjs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbwekbno.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gscguzjf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3sqrzzgnj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lvafahbr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ayncnzkp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hopnzypx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3apwrxxvo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ompjrbwx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3fqcuciuk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3urdykhxm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3sbzayvwe.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3aeasorqh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kkymrshq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uauuklru.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lugfsjrp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tyuxcfxf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3exqyccwt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3saamgoeh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3iakclofr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ubrddxir.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kgwmalhy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ycrprrux.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hrhqxbtv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yffdprgu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmrpkxhh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ssckkcbh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3tahybpsu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3uxwzugng.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3hwosmpcl.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3gseqamba.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dybpsfiw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ouwfuezd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3livwfnug.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rztnvpvm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3edirvnah.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3sraewsgc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3tfllcjtc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hvdiaiae.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3pafgrdqq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yffyyywg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vhmezmqw.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ztlimodk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3tertsfbb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3uwjaunax.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3gkwuxhor.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mhwdvyow.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ikjsjqgj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3jzaklsso.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ghnwixcw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3zauaefwu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ekaombrm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3bquowitb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3cwlmskjx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3psgtqvpr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3vfqeawbi.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3betpndmn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3vhuaatex.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3vhmiuzxe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ditfqeqr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3rbhtcmcx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3vfdiooxe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ufxsivuw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ydfggptg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3xdteryuq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3utltbero.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3fxashger.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3kjgdwhwo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ynoxeqmv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3xibahaok.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3rskftkvo.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3zgwcwmtx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3tnljgpcz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wkqendvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utyrvpxd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zykvennh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hddwwhke.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3hqgljepm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tflmgdpa.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wwsvuljr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qyyezynh.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ljpbstvr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ortylmpq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3obmulfir.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dgebyeos.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vmnemqaz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3xhykijva.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kanuwklv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qkvaxvks.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ddrulfze.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3nmevmnst.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qwwsvgmm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3wzrrqqhs.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3hsplrymo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mjpeojnj.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ryuvtwbe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hrrykkpw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3zlfijvpx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3poqgqnha.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3offxgega.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3bmzvmjax.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3gztmruel.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ezqmcjzd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3dekebxpt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3nxcrrgcv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ouqyroac.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zxzrghbh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3issoxanw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3cwehxhlm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3bjbhisyp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3filmosjc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ygpqgqhl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vmbfszou.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lfvlvtie.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3upqfcfsl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pwnnvcao.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tzqyprsh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dpgjnzme.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3nhpiknkb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3sgvxvaqq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3mucxwmcz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3wjcpvtut.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ifeaywlf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3coduxoui.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3sizxpxnh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3dcrpelkk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3gpneocek.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vdzfhocv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3jypvwqlg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3keyacfud.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rjubipxz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ybruxhrc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3emzcxrea.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3mcmygpzb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3iioactmv.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3abelvcrw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3idezanrq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3qqkoshot.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3bihngnjb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3dxcvoyrw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3jxmlunku.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3gjvxfcsv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3yzwgsvro.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3tpoxemgz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3fcvbnsqy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3kpkfyrgq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3rtaqcqij.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3llfmhcmc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3gpevqujj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxfhtign.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3yheprjka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqveehwg.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3bbawyhpv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3llhwfsau.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3mdgxpejx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3kuurpvzb.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3jczdvpwe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3hghojydf.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3uzmvpfgt.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ypiweodw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ivgsdbfz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3aliqvbno.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3vqgmssqc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3kttenodf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3jxbqvwyh.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3uadqeran.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3xmbrjlds.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ywsaiamd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3nbllgrha.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3zoxowgit.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3woelejis.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3oeeipbfd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3eogfpaue.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bzgiqgrs.html


<!-- 参考信息 -->