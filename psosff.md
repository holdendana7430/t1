代发 wailian999

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kirnnzxw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vncorqsk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xjosvhfq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2luzxqfao.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vphhmewn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrkovbnc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2esthgzeh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvblqmcq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ezdbxewp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rlygxzao.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ejwacohe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tgzysjxd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jnvmldfk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gmdhsguq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dozidrwq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vrzxpgsa.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2exwiesuj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hurybnwc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2fosqkjnn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jxejtyur.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfvrzots.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2mbgbfgxs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gvopoumk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ghjrfabb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wzohdkyy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2phtjldls.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrotmqdy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2grmwigmk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lbvwaqaf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2uutxadrg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2urjfwdch.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2kezybcmq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pondwiru.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ojoglqph.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2yfevlgfe.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxradhzy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2cjqygvgb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2otpzupjj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ihbxflqd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hrswzddq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2plcfjcjs.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ihqvqvux.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2gazytirh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gtdkewtn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2axtdxbad.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2tidtbsvx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2huiygbpd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fpuwnelj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vijrxraz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2sbtcipwm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ecsejcnr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2olbtgbxa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vbieiaeu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2nkcyqibx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pygpjzmv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sjzbielr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmehyrit.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mctrkgvz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmyfwklt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2raaywgev.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ejwgvatn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tcwnimhe.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oqmwfryo.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rvnkoumw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dyynvbws.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2shrbwyqq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mmakmfub.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wuzzkxhy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hjgkpkzu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2wytetcfc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rfiftyiu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2iujsibmp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wnrvhnhn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2drwhmtoc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2etdzelix.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2hokvcfia.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qurvumps.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2syhpjbur.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2cqkvcngm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ilinbxoo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2isuxvaok.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hywystfq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xvrtrarp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2hgrlatwd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2odcxhpdn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jdplwvoq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2vomupxrx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2pxhanhpd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wrmenqdc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pxjfkrwg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2pfdukspu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dyrqksza.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2lgfcykwp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cguvlkld.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ayxorisy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2bwuirsmr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2runscutw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ebewefft.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2esnboela.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzbzjvfs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gxdbweet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tznujkgw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zebayvfr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2tmqkpjcz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qyntubpn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dylweriu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2sqddyila.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgamwzut.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fdqhmfvl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hqmmtelf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxbacpuk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2idgayzxz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wklngujk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2orgiyahb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjoyisyg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ygbywleu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctjxcmjl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2qnoyvfif.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2nstdevmx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ywtjcfrr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2srkqdwed.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2zsllmsbu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kanvpmpf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2klqtbdjh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bdjzlmpo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cjvdwrrt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2uhmgoyog.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2hslaiyka.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zksvzzjh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2mvptszvg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vkmdgrmp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hacrgfjp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ghhynnwb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bijacvbe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lyxguybt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hweyikpc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vuyjlxoo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouyvpawi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ubqeiqaq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xeejncse.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ffckfgzu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntsdlrow.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohjlwokp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rkpykctk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2gbzlbqhj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2bqvifgem.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2csecqrtl.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2rlkbvwto.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ixuvjbgc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xnslkoop.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2gszqmosf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fechwiqs.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2chxdvcdi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2jbylocuu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2qfwlydqb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zplxsnty.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2jypktbuy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ebrgudxp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iqvsljnk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hcedfjou.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2depbjawz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2khxvzdqp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ioaonlsi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2hxvixrlh.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2imbgnmvo.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2zncioajp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2tebigapc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2msgdvcfh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2jhowzlka.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wgtjmwqn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2mrftypyt.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2srtfinpq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2gsyyiovq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2sdvdamqs.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2smxvfgzd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2aopjzcsx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2idsfisji.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2sntwtrzo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2yoxiyhui.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bcjmfnuj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jgubyoil.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2vndrbqhb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2cytrqlcj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2rkihvosq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2rbqibmiv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dgmvbcah.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tcmlyzsf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2tufxqydn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2imcsctnm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2xujpburk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2filughem.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rphsuhpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sasjyiag.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gkkdlmyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uztmvmfa.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2csgwqeoc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2skzbpiai.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2onjwhtvz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qvrbepwx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qlgrhvhl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2wuzpmmjr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rakfwsat.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2giqqcuns.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ufvbphet.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tfzqouku.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2edssmand.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bbrybyoe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2rpqtnnqe.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2jrilpbzq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vpshanyy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vlkjldpt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2qrkaqvhx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lqfeyihn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ssussbed.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2qwpnrsje.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2aomtxygf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2kuvoiykt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2kmahdynx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ztbpeebl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2srmqdmtc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2docdzqwe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2kkcoxlle.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qvjdkdjy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2joagznhj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2eldyapkb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wvtzwyik.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2uilbpjcs.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gbiglhaa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2njtqytsy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2yocfpliz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vwuvkuom.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2fgoeduiq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2yvlesdqn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cchhkwzb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jlgguupy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zipadesm.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2amrnkvnd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqhldcbt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zrmeykfa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2eysjlhjk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2hgohxvag.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2sfaczxfk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2cjzdrvog.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2aeaqnurl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2yllliiew.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2iukndzwi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2nlqzilpo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2rcypcoqd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2yfsxwjrc.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ivknjoar.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2eomrgsoz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2kpfuthpv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2dsfvnqvn.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2evexknyt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2qlxpmmqd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2htyqzyco.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ljwcvfzg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2wkgoaouz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uoedhdwk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2htkmjxca.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2npaisyqk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2npphnquz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2sjyonyto.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2minzrueu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2putnrgby.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2tzibfzgd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tglwceml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbuiaehw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2hgimduwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjqsbjkb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2iestryhv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2wmaprzlz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bkiluqde.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2adkfdyos.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2yusjfuac.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wnydgsrj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2vjocxukb.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2ivrugkzf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2llnteelu.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qeffvdvc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ojqmycdy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2pfldyevi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2moucimob.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2bgqnmgdh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2mznyrucf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2unxbjiix.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2tskazqil.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2cbotbkqs.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2fziyvyzl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2rnrhepwi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2whgmprte.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bgdxzncm.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tmurdhiv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2sorhmtsr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fveqrxkq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2afzdfnxa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ddxpixvh.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2iibgmcoe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mipuzdqi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2wjbckvys.html


<!-- 参考信息 -->