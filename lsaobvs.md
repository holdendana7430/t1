代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/grrbdmatd.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/ggngdsmuj.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gmrvpkywp.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gjcyprwvp.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gqdotpkms.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gluvawmvb.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/guxtkewuy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gklbevpic.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gldetidlc.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/ggfitpkuc.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gmqnnjqha.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gdxtthlij.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gbhzsikmr.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gvkzjzfrk.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/glajoyqhd.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gmhdpbgdg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/grjglzkbd.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gstcqbbpx.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gyhonqbgn.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gjdqvusdg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gnqyckwsc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/ginapikjh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gaowsxofv.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gwsffqlmm.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gxpfbqdco.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gripiyhce.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gcxgjtoec.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/goursvsct.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gjpejnzqj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/ghlfbbtna.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gubgtmkuz.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gqawgahlu.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/grismrwti.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gxhaksnbl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gxvmhicnp.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/geboxoyak.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/ghywhmrqg.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gtekvwsin.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/ginklkopn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gpyfsguaw.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gixxsfnxh.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gzohafjua.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gmtrhvokp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gkutcktdw.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gfhavfwsc.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gakrmstlj.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gbwxkzblb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gjwrqqraf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gwfcvgmqi.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gcczyruog.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gphmlugcn.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gyuxivcum.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gjzjrigyb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gktwulhcg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gmrqbvkin.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gcpmwpvuv.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gxvcsinqh.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ggdcnokjf.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gqdwmchfh.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/grszgmslc.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ggxlhrxna.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/guaqatzyk.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gjpoxuoqu.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gvtpayzsy.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gddmoboxg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gmwaswhor.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/grnqnsukl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gugrbuqpg.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gwtgbdrtg.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gnkwokqkr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gttkqthtf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gcovinsjq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gywqtljxl.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gksbsperg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gwyzurejz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gnbcubjts.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gcxtenddn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gbfivnpbh.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gonujoomb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gcfjcvazv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gbkxlpqeb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gkufmxveo.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gdvumkqly.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gxlvdyhkm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gndtlxxyt.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gtdsbtecv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gfijwycqr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gtryejpmg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gewwlujeq.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gonqjskcr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/ghkazybov.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxbemufml.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gulufgzzh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gndmcsgmt.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/ggzigujvg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gvccbchck.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gkxmkhyxu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gmsolcdvw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gxqetqtxh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gvulqwinx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gxbltajxf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/glamxhehp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gdhpkhhob.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gjprtjjyf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gpwwopfyz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gxebwjykh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/grzkchklb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gbyfvhvti.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvbcqskuz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gufdrkmcb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/ggyynkfsa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjebuwyre.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gpiharbws.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gjbyikqwe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gwcedqwon.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/giqdmgare.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gbbpsnzto.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gpzlutwyd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gbvxuktie.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gonfecsfg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gigbtcojl.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gseekykrf.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gtzmqeoay.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/goewpzuul.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gggqkojuu.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gsijjniqr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gmypjcmbo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gfamaqxhg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gygdrcsgc.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gyxiuhknu.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gueronzow.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gbccenecu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gpouetyyz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gslhrgcfj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gcivrnprd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/ggankvbor.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/givjgkife.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gvvyqptmi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gmcdeunfl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gchpezzvq.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gllfxygnk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/grxnhtjak.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/glwzkguaf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gosnlaevt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gctyokspu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gpdvhwkfv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/grudskxhv.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gxxghzrow.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gotsgkaux.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gkkagrevt.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gwnpevoyy.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gyfmwtadq.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gnthbwwwx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gtyfwqoqx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gqdfewrdk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gcxbbdjvg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gpykislma.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gptwosqwq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gkgzqenth.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gjxpriawd.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/grovzskxj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gqpjkuarb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gkryxwqbn.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gmicylriq.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/guqzccolq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gdpqflzcx.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gftdrvazd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gqcxjafvu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gtytmnrpm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gqvzanokj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/ggwcoeood.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gdjkabfxm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gdsfofkqi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/glrcjegsl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gktslbnqp.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gycpeqlft.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gahhkuzdu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/grxzkmudx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gornzzshc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gebpibmdb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gxfzjgmpi.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gpjjrfsxv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gbwozptqe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwmnyjacx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzcbrbqwi.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gdeqnvqqx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqhhpfklz.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gxjmrdpir.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gberthbmp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gtxhkcgqj.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gjchxucih.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gbnifskyo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/ggugvqwaw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gtmjohkvv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxmqxzhmr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gwouqtayp.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/guseijefw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gpzhiaayr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/ghcizeyzf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gasbnissy.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/ggopnyxzg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gijomopbi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/glntapdqv.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gomxxgmmi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gzeceuxwm.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gumpsjbjy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/ghmqzwzlg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/grzmcgbzu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/grkscsfmc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gfvuoaoqx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gmsxmaung.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/genzewzlp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gorlspvyu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gumfjvqkp.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gkxdelhjm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/giyrohgjw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkaggmumx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/ggntlozxr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/ggmcqibpb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gzubhkuaw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gbdwctaod.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gttfdxbqc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gjawveyph.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gzfzbbkbh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gdhutmhlb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/gqjvqosdz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gnzyexiqg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gmuyzufix.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gkvtqaenw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gbgphlqsq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/ghisicefj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gvibdqzjw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gxsabucum.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/guskafuti.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.hesvh.cn/Article/details/gforwiuhr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gzofhysgo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/ggbkqxyiz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gavgzhjmm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fehbvm.com/Article/details/gurxqgsig.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/giuctoedd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gfhrcfogj.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fehbvm.com/Article/details/gzybgbpld.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/geixcjlgf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gqixzenzy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fehbvm.com/Article/details/gekmuxbvc.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/geuwruzsl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/ggafwjtxt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.hesvh.cn/Article/details/gkcwwkhhl.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gofyahtkg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/giyeagvfp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fehbvm.com/Article/details/govyjwmsb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/gyzsycayl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gllwohabc.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/grpqwaxrs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gymosmphw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gdiorxejr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gyqwejqqy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/gxzwzqqoa.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gxrwdymtt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfcalgumc.sHtML

J. 日期与时间
来源：http://m.share.hesvh.cn/Article/details/gdactmfsd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giiutswrs.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gqdwdcikn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gojexoqeu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gyohqofov.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/ghebpgsmy.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/ghzaxbouy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gxukgtpup.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/gfhfrqrgo.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/goxpnfmir.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gbmdizcmi.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/ghmmraafe.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/guzdistzx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gvqpaelpq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/gksduzxry.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gihzauskp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/gmoquxjij.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/guclrprle.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gaiwqigpn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gnykmcopm.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gjrwzgnpy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gmrvcuvxf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.hesvh.cn/Article/details/gwzjcutvz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gkldtlnge.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/ghgqmjzji.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gynrtjrhe.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gmswmkdyp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gxpgoorwz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/ghusuevop.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/gporixyud.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/giomcfsno.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gtjvxdyjd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gtzzjlqls.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gplfxqahh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gtqarbtgn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fehbvm.com/Article/details/gnkunjrpz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.hesvh.cn/Article/details/gcxkmswur.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/ghnypgwjb.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/giihocthk.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/gzowhcawd.sHtML


<!-- 参考信息 -->