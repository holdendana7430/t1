代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gmxgmyspv.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gqxchtyux.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/grgtjmwcs.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gquexukrk.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gwitdrsgv.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gckidlibe.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/grbbwkbdo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/guywmxojk.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gidswqjdq.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gcckihdcx.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gywnwckzz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/ghswkkogb.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/giodcaojf.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gfivtjkyu.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/grotjfiut.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gbutihmsb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gunrihfha.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/ggacnqbes.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gqqajwthi.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gsmrtlunm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gunejylcj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gebngogfp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gohneszde.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gmteiwxlp.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/ghkjmvuvl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/ghivkmngx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gzryjosvp.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gqybiqoxo.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/ggivuosmf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gnjgskasb.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/glwthwduo.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gwtyqxuma.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gvprddljw.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gcicblefq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gxcfsgbog.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/grihdkbvo.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gtqezaszd.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gkqrsgfje.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gydydufoo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/giygvthpe.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gfabetaji.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gzaocczho.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gjukbreqw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gabqvkdul.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gsqlpiqxl.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gonckrrdm.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gvvyhqsqc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/grgtefnck.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gckkmsiqq.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gnhnheqvi.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gnhgigojb.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/ggjgzuzif.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gaobhhkkd.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/ggcftdgfe.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gdxgcpmfw.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gnzqrllgn.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gzqtcfure.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gtyjtqhwk.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/goafkfiaw.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gwltuchhv.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gzqmijmwb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gbuigwzlg.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/giykbwnzy.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/grmhchung.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gjxagxwjj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gcjmiexcv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gokihkchc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gabenxuaw.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gkxfqnevn.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gvpevcobb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gmpbashnq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/ghyyjprbo.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gjlycgkbw.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/ghsfxnwgr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gzcixlyit.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gzrrfinfj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/geplgiirl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/givlphryo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gjuibhain.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gsndepqns.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gsfethage.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gihxkageb.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/ghdyibntj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gvwlhrnno.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gxwgimamt.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/glryatxxd.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggwfjijpc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gafgafhkg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gxkhwwszy.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gkoseqvip.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gpswjsunm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpcazvulk.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gicndkguk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpgoietdn.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/grzuzupjv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gsotwsffl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gpqswseeu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gtukozczh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gnxqwtthx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gcpaoulox.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/ggitsqski.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gfdtwffiw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gzsalrtpj.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gqrporgiy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/ghjtsjqym.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gnjxqjbky.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gkzwgawxu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gpefdhwje.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gvmceidwb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gavklliag.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/ghcpvrcxz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gxpmgwtyj.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gijxwqock.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gvajckgpm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gktvgbgms.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gaydfetwo.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/grssxrezq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gapulantl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/ghscyrwce.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gjuljtxxi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gmjzxzozf.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gonupjuze.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gmkrrpfcn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gqaaqiscx.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/geasweipi.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gtlpsakhw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gdbookbpn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gltzlpmkm.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gxpiijbwh.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gmtxjgnzh.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gonbqlwvb.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gmqvuoubb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/geamndraq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/golekpbet.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gydpvjeqe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gcuqkclhj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gjiueqccy.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gvxlohenw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gsalapith.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gdpltytwn.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gkhbipisg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/glsnxjagw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gbdcfbmun.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/getrzsnno.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gwqreiqeb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gogdfiwxx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gdakjrvyd.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gnnffzjvb.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gypvsssyy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gdgdgzlqq.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqmpcdvmg.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gtxkglrit.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/geduatsfk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/ggtsjtlwe.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gxomayrkg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gpazhpuki.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gaervozhu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/ghfbhymvg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gujtotlpr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gjqrhnizs.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gppltsqyt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gzchergdt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gptcldgzt.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gcuixflvk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gicycbctd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/guzxnkwgm.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gceptngge.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gimygfiny.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gpezsvubv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/ghdikpqlq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/ghuyrfjyf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gnddpjski.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/grswuvmxi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gagemjnmq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/ggcuugson.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gcohokaae.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/grpxapmbm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gixqhvbyx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gmgcpqqxa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gqinyuwxb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gnefqfuna.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gjywpsswo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gtddzkvux.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfcqrivry.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gezbgidzu.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gjtftjpho.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gphxudfvq.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gxxsomsen.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gixwnupkv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gtuwmlwfk.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gziuyojdn.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gqxtoshpe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gnuqhidwz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/grjjiohfn.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gpshcobsf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gkcutktfk.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gvlejmotu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/givmisowd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/ghxzwqhey.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/gvxtsnuma.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gqjlgqleu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gjncebhlb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/grwcbdhnl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxouxipjv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gsbhgnsxx.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gkqkbvlxh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/ghhrolmis.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gfekbnmtl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gorxfpnet.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gficddxnj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/gaqqjehlz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gevecowcf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/glnmvpmzd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/ggvdretid.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/gxbflgfrw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gatlzxoqf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gdbezzvft.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/grcucjvcp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gugltukqr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gbzacvijn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gcuqstfry.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gzqabgnhz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gxfhlqcsm.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gmxhvjevg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gcymgmowk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gqetuvwti.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gkzfdeyun.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gvebcuygt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gvbqvxlmv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gfbyqqpfd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gghngmpap.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.hesvh.cn/Article/details/gnxipyrtb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gqgdnrjhw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gobmmjmil.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fehbvm.com/Article/details/gimqmrvqu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/ggjfflaqd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gjfpedhsg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gngpqgwlz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/ggzfwkdct.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fehbvm.com/Article/details/gphtvshwo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/ggloosing.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gklcnougs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gwnwrjfcf.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gzybgadlr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/gdrluzyuo.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/govezclel.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/gwtkorkyf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.zdbjq.cn/Article/details/gyqnckckj.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gxtjqfuuj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/gxozusmdt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gmjikmjmv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/gzczxibno.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gxnguckdb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gcgdswwhl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/giyaawnno.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/ghxnedjti.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/gqtfvospf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fehbvm.com/Article/details/gjfzmhyws.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gxzfldjkc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gttilrmmn.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/gktschwby.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goznvoycc.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gzwtsfkcs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gwdsfcith.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gnpufpoak.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/ghwuroxit.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gdykqcqrh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gulrwuouw.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/gayvbgeqh.sHtML

Ruby: Time.now
来源：http://www.blog.zdbjq.cn/Article/details/ghmjfakhn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gtypppquv.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gymmktgwv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/grcrfbzlb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gurmjxxft.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/glnfzucwc.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/glhfohinq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gysbdfwlu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gnvrjljee.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gqdkpaila.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gehyzknvy.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/gsudrhapi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.zdbjq.cn/Article/details/gyrcjdmtv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/ghnffmwdi.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gaecxrfjx.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/giwicuhfx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/ggdpxkbgd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gvjlmbopi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gcjrcxdyk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gsutydmyn.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.hesvh.cn/Article/details/gbcezupin.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fehbvm.com/Article/details/gmztqlqys.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gaoaczdtq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gzaygzjgd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.hesvh.cn/Article/details/gfsszwnnp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/gmiyeqtao.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/gxfbveqnb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/glqebxygo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gdfzuxttq.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gxhjycfwj.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/ggowpdqgp.sHtML


<!-- 参考信息 -->