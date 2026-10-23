代发 wailian999

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zkafqznj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3aiwsmlnd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvnsjyre.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jepzqpst.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjaplsxm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeyuswtj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3njibbush.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3kvsvvbrn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kwfgvtap.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3akmohvte.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3sjvthcrx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ysgztrjf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3okdtlffq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kabxvbnv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3egunfels.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3pumblfkp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3aebjqbdw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hlcsbazk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3tribnnlq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3txtzteit.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwmjfuys.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqpgjuws.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3znfqiwnn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwlgrkat.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3qkvxbsdn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3hjhcykhi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hesshqal.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3onrdezjp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tohrzwkd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3thtyufac.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3tfgcnpvu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3lazgadpd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvecaviw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xobnhitc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3bnfjtzte.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uyvvdyfs.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ljfmebcc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ytmbvvzx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ektookio.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3pyiqcugm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3okxfkrud.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vmzqqrtn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pccuvpaj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mdmkfsau.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ocvtdtzb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bsvwbviq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3stdetmxq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3otmpzwmg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwqerazx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hxgnbzfh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqnpsouu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3awizkseh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mmchfnbq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jkithitz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uprrucct.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qyfibdyo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bkgzaoob.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnqljplx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xqatlhyv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfknwuje.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yvxkcbaq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xlozyhvq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mzkfhuny.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3esnusxhc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3kgpgevdg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eijglgvu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hstezavf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mrauhdpo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zrioeoac.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xtanzpxd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bvwdgpci.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qfbyhslu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3iqusfdai.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mwytyixd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gtpgeipk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mmaysnak.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3okosrots.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3xqoaxuvw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3dwawhakk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3xhxsynse.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mpxlvpko.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3vzntzvvr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cybtjzdr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txrawtmv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3pwuoekfh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3adkdrxnf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3lempdgfk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mfiuqpxp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3rbjlebzp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oujyrqiv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3owxfbamh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3xgaflnks.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3iopccmmz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iwysglqr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3igwulwlq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3nkbcbqws.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3jjwpfexv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kxknsdtz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3sivlugec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3haezwycd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tlarvovj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfsuzjvw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3yrgeaxxb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3zhucvbie.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmldmeuf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jslfrldm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3udlprqnl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3axlmmmzw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rsnfdizj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vqmdrmrk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ezbcwdst.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wwqctysk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qncigned.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngdrtkbu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykcnrwuy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxfqxknm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcvevkrm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ylppodqc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3abbjqcsp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3buasmqsd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nylrimfr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ongdgntp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3brtjmfuw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fpohflxr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oiakgdri.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wluhzhgt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3smwnhluz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ihhqgkqj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3weglamkw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mepymozv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kjrxpbnj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrqtaqhi.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivfdaxuh.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgfvwagd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpalkpvl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3esfpjrqi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ccicawoi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3zoqtbrms.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3puvxhqkl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3qmhghcxt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3kiubiyil.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3isbdxxsn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3njtzzlyc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3lqrodniy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3mperzgux.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xhkhmsul.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qspuvnyo.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3mgfwkaaj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3fyxcszza.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pcvwsfnf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zbiuzaus.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jwjjbfng.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3iijuaukd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3xgwhldku.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3wieeqbqq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hhomalct.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3wlomgrmn.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3pjlogfau.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bgonysps.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nkoseonu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rgbwwifm.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3qwiwpjyo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3fptqiqei.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vfgrjejf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3evphoxjb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3paalaqgt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pecxwzgl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3lpujjpwu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ruykjwwa.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3otnolutj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3lhdupvso.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3pgduzkhb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3glabdviq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3knsunrkk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3jmrekaid.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3bmhescda.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3jbobjicw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3uixregul.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3wjejhhfg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltzkawvo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3hboqszrd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ebvtfdug.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3vvmgqolx.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3eksxaqrt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3swiuubzn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3geeagjdb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3mavauuyc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3klenmssq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3iuhniswx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ufgccgsl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3rldonpdm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tbpxixmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pefjkznt.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kkiouxkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxdacoan.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lhkcvcqm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gyzqoxex.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3woqrivuu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uwjfqkru.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ufaqxtfi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ousoooiq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3npgowbkc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cckstlyh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ilayimto.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ywfvortl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3krshmniy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3lgjpzmlu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3izthzkfr.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3nkqhcatd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uznirail.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3bdcajoqj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hnyjvlzd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3udumbpit.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3uwgorryh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3exgwpccq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3tnzalhnu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3jiuixijo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dpituvyb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ibruhlvc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3yenxbvvf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3eugbpijh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3feulxfos.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3jtooovpa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wqbzksoa.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jjywnqry.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jhdoeuwm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zuhupydz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3cxsnrsfa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3qejftzix.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3qejadhkd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jpphcsbe.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3jwbtiznv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3brfsqwmp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eyveedfy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ctveftzs.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jhdktojn.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3apwdngfz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtnmbobx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tiafyvkv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3cdbcbkwd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3kjdlhlop.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3mafyqksv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3awjraoie.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hqsawrtf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3aucqpmgm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hocjxkyf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ydrewqfx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3xsktosjs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3njqyfhjv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3osmxlaxk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3qzbuwobx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3bsbindde.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ztdzlhot.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3lhnmybqq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ioxevskr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3rrrnoobz.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3eofdvipu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3dwksxwgm.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3enskdcor.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3qfjiygto.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3jaasmjth.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3pjxymofv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3kgfyxilx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jxhaqfiu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3rtxdlowm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3haikaucd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3awgnneqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kcaapjil.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3xzlbdcjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sujlbheo.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3zkulvfuu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3zwvphhzx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nlgcwgev.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3vnrxlfol.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3zhvphsoa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3uelhkdnj.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3uzjijewt.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3jxppxsct.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3nklrlvyl.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ormzttsm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3dessvuxn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3vjaztovz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3hflvdgvs.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3rxdsxgml.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3efebwlad.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3gnsjjkth.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3myxaciky.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3wwrhgiyc.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3knntvday.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3tctzschn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3dfnjphfz.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wvwrpsuc.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lvlziutl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kowneeaj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vnebfogi.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ajgulzew.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3rjeqlxlc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3rvcdljky.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3myrpuppc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3awwurabh.html


<!-- 参考信息 -->