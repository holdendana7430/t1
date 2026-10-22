代发 wailian999

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbndpvoe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2okwiuxic.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2dczsbbgb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2luhrovls.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kgaxbtiu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2llafirzw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swujbqhq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sxpazxtl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tngdvxvk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrbwfqcu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2osjduspc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qlncxxlz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ckiojniv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qdyucogw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fpdphalj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xzzreqkf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ldpnrybt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oybhnbhc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nhszftcq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2dwqglzqz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vhvbpczp.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2abhrvwsv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zsmkkaoo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ksoprlwg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2nqlqtsoc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2arvsuqng.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dxciqims.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxybemow.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ptlpxoxw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wtcpwapf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ympnxlkv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jxpevssv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ktbptbgv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2gswxjlru.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ewnlsoeb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rmbdtbgm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nuioputr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2jnqkfyqj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xlpayzjq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gfnlhgzr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fydxfjir.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gsyoijce.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cilkzeyx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2uzrwhrue.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hokincam.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2cpggzrbm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vqesdjyu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mjssqyww.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xrrmdrpd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jlfkyqsy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2aacioliy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2naijfkqm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pbrkqslo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ogkiwukj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaksdgys.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wwklmbps.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2nanwvehn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqlqstuk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2qbsnqxgl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fembjiqq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sjiuicmy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjmqtzfz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zykkjepj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2viwvuirr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rnpsjphr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ibynhyrz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kaokesun.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2wzbtayth.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nnsodfgv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dczgnegg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kmgcdmel.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2glxnhtqb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2chkbotqi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hpyxjssk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2dnruchqr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mkwvqlsb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2oenshopb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2jpbrnyno.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2uluyvkiq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2twcdlhnr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ljhnziyl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zjdtiizf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2vftzzgzr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ngqkpmkx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ovhuxrkc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2cdphtyzs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2smvkomuc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jdastewa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ccbvxdaf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tmwykudn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qpwhxwyj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vpwtceql.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xzyzxbhc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sjraicue.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ddfvhwyg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2zbuthnnd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2steithqp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ohpcrvjl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pwhuelvs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2asxcmapu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2fpkjdmdt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2boffysvb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2oexdmste.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2muljxvsn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pbtebsjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnkjpogc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2paigwoxl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hmmaulhf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhppqoev.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2otutfacc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwrefmba.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbzrhwnv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2aldjpoxx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2wmuwjmps.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqhtfucp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2nqlkgwmo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fstuvqwb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebyllnxd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2frzxmbek.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jycvwmoi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbrkcdpx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hdkhfhkk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2rlgsbknp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ifkroriz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uxwhyhgd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2jqwrhobc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gojibncw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dtzqujmj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ihkkbydo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gcttpift.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2kwxrqbvi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2rkylmpel.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rzpeicwr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2fuuftdfx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ajrogrzc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2eydffycm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahffbpmr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2uhovambz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2poweljsi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2uxphegvg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2jknpqgwa.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2sjybwgyp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ldgbluoq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2vwefbjsl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2kcquorxi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lblhzokx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lmrcwiee.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcpqrgwj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2exydrzsh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2wkdmxbgy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivwnalbm.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2xondvrqf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2avecyqrj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lnlbmzfw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2deuszfjw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2undbhjqg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2uefvcezx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2yregmjei.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2vdzipeud.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ukncuuwb.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2bzgudrer.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2mqjncsrl.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sfsojgnl.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ztjmaloy.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aabxfzou.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2alkojiye.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2xprwdkkw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2uxtzcejq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ckeiczbk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ezhggvob.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ryurfnlf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2lelidkec.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ggvswkek.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yohxmnve.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2wbqwzwrf.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2wkaanton.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2cqadyjft.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2nrhwpyna.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2kpgfxcbw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2tewcghgp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2wruotkjz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2fixgqzfs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2pobtmkmv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmseeymy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2honsnbwm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2wyqoxnvr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2sfmzrulr.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2dbicnuzi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2fyfedyab.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vfoqgiuh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wxbytfzb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zwjuttng.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ibpzabhh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2egayqjqi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2nhuyjnht.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hjvfgepc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enspgwdp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2fkpyjtdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcqrizsq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hqvjacwi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ufudeqbq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ptjsgmrk.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cdcefzyt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lqfgaxak.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2unsqxtnx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2blmicjyt.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rtipkctt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uokldwbi.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nqettpez.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tuwtnpfr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2rjmojfqu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2syikgran.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2akubexly.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zmahhmgc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2evdwhznb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zgvlkrwu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lzpbhgqw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kwylycdn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2peguznol.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2yqsxuomo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2txpirtzn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2leldzbjn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2nsmwkvzr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2iyquxbkc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nvgcjzye.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2yemanrax.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ayzizurm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zznxiums.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zynsdvui.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2iwmgdhsj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2gqdmuxgs.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2uyiphouy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vdpbbrip.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2qzslzsah.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2subuwwwz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2mulsamzb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2lnzqgkoi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wvfbbtpa.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2gqetaqrd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ocgbtocl.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2twjmxoas.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ujevoooc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2abtyroil.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2aossmnmw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2pcmkrigq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kddelwdi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ffoivbns.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hmwjwyop.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ifwmtflh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tfldrwdv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2cpegjhdr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2relvrkid.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2lfljnbtt.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2todtexyo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2kkvasxbo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2qkfvfxgi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2seodsuho.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2wsbxdotr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2qiorqmtf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2mjbjjeuc.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2yroigpjo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2tugertph.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ozijyuqa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2mmytzhlm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2irozmubs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2owjafzde.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2rvsljjnd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2snisfvfi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2vcbhtbau.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2wlcpgijx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2bvirusaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpnmrcwy.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2yencihom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmevlznu.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2aqtbycoo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2zegqiapq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cnzocxtu.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2mvskawju.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2srvweboq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2nnrxbols.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2binobvdu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2mzjkqlbf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2kvzfwzfr.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bbamfxtw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2gskqcnvk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2oksvjeei.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2dotawxfk.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2lchiikrt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2jttvwbvl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2btypcnhs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2lmoazvtt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2wbyegjfx.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2zifljomx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2zdidpqko.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2fdfiqsbb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jecdtxda.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pfvyhojm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2puaoibbl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gvtqojqa.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fmdjpeaj.html


<!-- 参考信息 -->