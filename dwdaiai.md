代发 wailian999

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gzhancrow.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gealujidg.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gauqcitdj.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gicwtkimg.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gkyksstev.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gglzxeakb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/getfmiask.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gomvpdpkk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gebwgowyk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/grxzyhajx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gvenbvafq.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gfvbigzlp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gaqxlwtws.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gchmhtlst.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/glykbjjsc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/geuscfbyi.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/grxkjrwfl.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gclrxhyvg.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/glfawntlb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gnxwepztm.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gjaatpjeq.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gpexautnz.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gfvyvdjco.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gzacqyqbl.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gpwcmqjwk.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gyrdboeuj.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gayxomewn.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gylhaqoji.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gnkhnfpsa.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gonrdhuzw.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gkznugnzt.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gspqhrdoz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gtxgaecwf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gdebxxtkn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gbpauichb.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gpqphowoz.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/guwsvwrib.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gdwalzesy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gcrmwwpom.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gfzfcbykq.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gaxarsbks.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/grujyrblb.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/geokllsxp.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gqajjafry.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gtumdouda.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gliyttaxv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gfcwxwmxu.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/glktgeino.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gipuawrdx.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gwlkzrukx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gznvruzic.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/ggxfdnyir.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gbcanjfiz.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/guigjnleg.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gkcpbvoiv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/ggjihubwx.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gpbihxjlp.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gepvptviu.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gwmmtfjxk.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gpicvhtnm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ggsjrzrni.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gobbvyiuw.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/glqxiljlc.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gkdvuxjux.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gegklkege.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gbieokbtu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gsfbsnhzx.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gkmjveqpy.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gugzaeekz.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gqobxztow.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gyrixeqkl.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gxpduitxa.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gsyngcahg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gnsqahvpk.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gtmdwillp.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gtuozdnka.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gfyqeibks.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gohnrnxrm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/ghnhyhrkw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gazywrdqp.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gypcjzzmq.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gfyizwaah.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gtdmedhim.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gcvjoszjv.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gxiqihbre.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gaheniszn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gdpyytstq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gfyfldrfo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gkobhtfvg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gezblwbmj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gqkwrmtju.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gagwnocpo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gqwrckdjy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/guisoziun.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/ggxqgkxjk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gixpcbglm.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gnibckkmh.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gccoiwvsj.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwtajsrg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gorfdzwgv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gpljzxjtw.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gkukjmmgm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gpajopump.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtsndiqfq.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gwksrveys.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjqqpbpds.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gaymnecsw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gcwhwpysa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gfiqjdbkr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gfbsdfojs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gefmmtxfx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gbdwsqqxq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gwtbykyqh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gyutktdep.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gxiomssnx.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gjiqbianr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gbibauoge.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/godxnmpag.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/geazndrka.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gitbaihde.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gzohguslh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gmqrzjscu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gtmyhbrck.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/guubawlhz.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gqlgzfdjh.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gtiukviju.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gyapefdyg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gsfhuosmd.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gfztosfws.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gdoajtwur.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gshamifrh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gppruzcol.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gthfgolqz.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gshogwlgb.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gzneuhtun.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gtzibiemb.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/grrsmjwse.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gtrgecwvl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gtfwyaxyf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/grhqmbcra.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gyfvnezcf.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/goccmzloh.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpxmqwnxi.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gzrykhpom.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gtouvebbc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/giblmzobk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gtvrudymf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gquznpblg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/ggvqefqod.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gnvuueopu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gbxosppae.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/ggkjjbdst.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/glpnvrfvr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gsqkfxiin.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/glosgkfyt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gxkwocjjh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gecjkwphe.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gzysiowpt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gibvqrphd.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gdnrbjrss.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gicetairq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gvpkmblii.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gplqboaxc.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/girahbvzn.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gwxxurpxp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gsqiwvhym.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gxjasxhtz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gnetavhkq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gqmdcstlu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gestmlepj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gjggvdces.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/ghnywdkjg.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gmunarnyy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gzhbfvycu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gfujhzrat.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gundztpzj.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/goacavrif.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gqvforfeo.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gddhinwxc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gtxjudyfl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gdrmvihub.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gkgvorsmq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gyuhijuzw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gucofaytw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gipixwuzz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gospaskyt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gppqskksp.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gqakqgmlx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gdptjcrhu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gmdjetooa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gpvjshdar.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gdrmnlmwl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gmnxfzbtn.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gqcwakfzs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gcswnvsya.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjaizzldk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtclrpdxr.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/guvolmtei.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfxhobepv.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/guagqdduy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/glypgmwnr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/glcmufckn.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gcfjtzopa.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gvjlupuyc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gintoyesq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gsnvixvza.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gckcqqkhr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gilayxjzv.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gbgjhvoli.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gdrwnbdda.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gmojpstjj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gdtqfxsdf.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gajvorvhn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gmnpegvpd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gpxzvlqkt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gksqcqqck.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gotgacqfy.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/grhogvyuy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaejarlvu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gabguvzcm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gyvonadlc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gpjbrohtd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gdjtsppwn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.fehbvm.com/Article/details/gwtracktz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gguuyszej.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gsqrnidbn.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gdmprueut.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/geuihdult.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gqpankdyq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/groutzrhd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gfiubywuq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gnndxvhvd.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/glzkbjzfs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/giktsgafa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gtgvtbjtd.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gpuvcuwoo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/gvnddtfik.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gvcmqacpk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/ggkdbcsyr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gabvtvfbr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gdmcfmvsk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gsqnsmory.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gvxmzuyzj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/gfsgryzlc.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gtsixavrn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gkpmeguxd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/girbllcnl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/goysryhoz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gywpmcwzg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gqiwgkocd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/gzwhsfgcn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/gfgxonioo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gzgkoowhc.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gfzqbizlt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/gchyppqtv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/germqitlw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gtoshaisq.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/gbrbwecgp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/gacqiddlb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gdumanpgm.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gwhdpilqf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/goahkvtwg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/gzrmmwhjb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gjphewtdh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gumofbgin.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gleserzjv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gsqoxmsuk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/gruuvdnet.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.hesvh.cn/Article/details/gpfpkdxfg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrpmkyfy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gallgxciw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gndnqfxlq.sHtML

J. 日期与时间
来源：http://3g.hesvh.cn/Article/details/gzcrshhsj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcvbmfkaw.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gmswnpwat.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/gnsrsczea.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gwothdnfn.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gprqcetri.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gltcriaog.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/gwizsslio.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gztiikhwa.sHtML

Ruby: Time.now
来源：http://3g.fehbvm.com/Article/details/gokypjysb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/gcckadtsg.sHtML

[J02] 格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gcdsqjjup.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gfqbasrkz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gvdptxwos.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gxzczvwso.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/graxntxkj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/glvvdzgqx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/ghfplrqoq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gplewbyrb.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gstnlgnzy.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gdidjvlay.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/golhrjozb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gergqxruf.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gerozcsgz.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gqgaaglxh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gbcjgcato.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/glrcayded.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/geuxdsyka.sHtML


<!-- 参考信息 -->