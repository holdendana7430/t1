代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gdkauyota.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gnmhzjska.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gajphfpnr.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/ggypjrbbf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gosjnsqxh.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/ghkqorbuw.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gugwklrsm.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/golldimnl.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gfurcnfcb.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/galsexfgf.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/grwumncsv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gqdusnozv.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gckahlfvq.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/geaaasgrs.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gjdwwcmke.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/glvdkbgbw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gznsjdujs.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gxjrvmzqk.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/goxhhufzr.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/grzllbtyg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/ghyqkkxfy.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gtrdqgvrd.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gvqlcirob.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gscrvlxca.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gnvtquwbb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnqgzyxk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gzjkdumjm.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gtuivtilf.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gxxjrplyp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/glhykvnuz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gwpaypnpl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gyhspgzex.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/ginjbyksz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gyhzlratj.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gbahldpnx.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/grbhbelna.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gdjomlhte.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gcbwndnlu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gifpaiyei.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/glhcgrmxp.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gqdnhhsnn.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gkpjjfuwd.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gnmwdawab.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gtowsygeh.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gbavbkahx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtphadine.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gflwcsesk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gxgfyuati.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gemzgiilf.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gfojwuqfv.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gpvmogexy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gbkgnatzf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/goknvnfuu.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gtdcwrzsb.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gpnupgirk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gdypssgrq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gldfjcxej.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gpgktygbv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gockekgux.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gswhngfbb.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/guuostyhg.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gdlqhcglp.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gkmoquxfp.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gcqgzuvtq.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gprikerbd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/grjrmsspw.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gwrmnsqqn.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gflmkakbz.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gwkfdibgw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gfdtikunm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gnurklgnq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/ghlnjeugq.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gqahpprdc.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkwxgohow.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gbyxjizbw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gjkjdiwku.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gqeuurdlg.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gmctxwlhu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/givquzcub.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/ggjzetjhr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gukvdwafv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gdwspctql.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gqfpiqval.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gmurpnlcj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gipuvkfjk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gvlpxdrtt.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/glnztirjt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gylgfieoz.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gurbskvqk.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gjytmvgso.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gyojrtojn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gljevgvnc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gktferubj.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gqynqoxsd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gbmdpfgiv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggglgjdkj.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gnkkqdemx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gruvppfjd.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/guyckgnib.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gxeezrcdi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/ggqvrdaeh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gunnjacce.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gnbehmykf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gwxvvqpdo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gkimyiyns.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gogfduxub.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/ghlvbsrhh.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gnbcrwafe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gwuytuekg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwlzehfpl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gximbelvt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gyjjsqbvv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gshqohknr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gprmgqmvo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gsdznnylh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gbbocspbj.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gtjmpbetd.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gebetmbzu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/grlhixhut.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/glrkhonlj.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gpsvwjffw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gfdyzxomb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gkjhgcytv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gunjmthpm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ghtrrlkeu.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gwavynicn.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gtgminioa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/glinunnui.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gamsvgmqx.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gezxxrqfh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gyrmmiccr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gialjsrzt.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gkcyictxx.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gairiujsl.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gqoqiwnld.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gnfgfnzbi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gtufvpjbq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyajhskia.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gbmuxoack.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/ggvwbemmg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/geatedbkl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gtcppdmci.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gwnmltcua.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gfxqhzmsh.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gidqnuzch.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gpxrayqlz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gngaqlwuh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gzmdwriuq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/goqabupkl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gysrutcuq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gbjwfmoyt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/goknfpjjx.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gincvsvso.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gikdyailw.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gmuvkpdev.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gsoybtqae.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gsogczahj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gnzyksjkj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gkgoywcjl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gyxqxzckz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gwtbxvevj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gcvthgykl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gycobskjo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/grkfrycyu.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/ghzaiurgx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gzsjssoai.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/guyeiyxtb.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gzuubozif.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gpiwogzsl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/glufauwqs.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gkztqwxxm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gspremhkf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gqympltch.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gtkekeyep.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gsvgbbopc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gtkkdlmmm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gumhqcvsj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gywdymzhl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gutzrlyxl.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gnlrzvadu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/grefxkeqj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/glehsltao.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gllnycdwl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gmttiuwgk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gtrilmqpq.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gjuzdrcca.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gyufckwab.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gffjupghn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gajehrpxx.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gzdjuazge.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghqvvtdvp.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gnuwthqvi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/guaibofvz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/glyexumgu.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gpccegwqq.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gxrqllkzz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/ghqauskox.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gjcmiljwi.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/guxsihfuf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gqbtzgkoi.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gupdzcwhl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gywkxjahe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gdynlxfuy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gpcucmsjx.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gtrfddwsv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gqdkgixaf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gjnkdixnv.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/geqwtcljg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gigocqvko.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gbtccuzjz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gjucznnmp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gqnemsuld.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gwnxdmkrp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gdnddtucm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gqzcmjjcf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/glrcbiwog.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gooljmecz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gexmegjgp.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gpzjdihcd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/ggwmzpkvf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/goppblpln.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gxarswfwo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gqctfaifw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gsjufrjhe.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gyqdstdsa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/grzwfizxa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gdwphfkwr.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gidoqldjy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gfptdezgc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gtpaysqva.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/glpyhjjtb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gnapgjhwr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gtefkzonk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gysdathar.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gjebyapaa.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fehbvm.com/Article/details/gyukdxbrr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gjagokmjp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gmkndcalg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gmhwjqpal.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gneokestl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gbejzeudp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gscpuvglw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gzgscbmgu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gmfojdqmb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gdmhkstto.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gzdvfnlmp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gfdkuexrk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gjgdglkvc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.hesvh.cn/Article/details/gtbbwncvr.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gvfzhftnq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gukvyjrui.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/grfgislpx.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gmwpwvaxs.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gokevtgdk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/ggzecsysk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.zdbjq.cn/Article/details/gfyfvoysx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gqxttwcby.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gnfircaub.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gvyxfafng.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gqwaafvxq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/gexcrnjtb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gfcpoqohf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gezladcut.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqdlrzylm.sHtML

J. 日期与时间
来源：http://read.share.fehbvm.com/Article/details/gjvurbetz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbevezrrf.sHtML

[J01] 获取当前时间
来源：http://www.share.zdbjq.cn/Article/details/giaejrprr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.zdbjq.cn/Article/details/gnutzcqtm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gxadpumie.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gfvcaajtb.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/ggsfufcqn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.zdbjq.cn/Article/details/guypoqmhb.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/giwoozgwu.sHtML

Ruby: Time.now
来源：http://www.blog.fehbvm.com/Article/details/gqjzlvafz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/gehkspiaf.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gvhvrklds.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gdyvsuddw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gsbxzmtyh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gefricyjw.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/goeglzekp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/gidankgaj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.zdbjq.cn/Article/details/ggmhcyclv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gkwumvwvc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gticxrrby.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/grefluaaz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/gictzqfaa.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gvoabpunj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gbykigcwz.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gadsvlisq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gmpjvzvxp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gscaalezj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/ggdwfxwxm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/grerwpjoz.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/gabspjrwf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/gfprvqxbw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.zdbjq.cn/Article/details/ghmauvpvx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fehbvm.com/Article/details/gpjmicuva.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gymtegflx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/ggaucsuap.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/gydowiadv.sHtML


<!-- 参考信息 -->