代发 wailian999

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/ggtytocqn.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gxwreieqx.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gsbrfpbdd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/grgeeojyi.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gveuskpel.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gnwgzugwv.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gkmunhslp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gcrnphauw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gqadxxdss.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/ghubglalb.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gwubhgfqm.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqqlbcpbj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gimkyrwsx.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gtuujbxkn.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/grbhqiycq.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gjhsdzxtj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gpzvqgrkg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gvsgzkkfh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gkglicoso.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/glmyfxazf.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsebjcvcf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gsemmwrll.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gounfcdbi.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gujhizmvs.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gpvbrzais.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gmvkhgtvs.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gtqopncph.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/geuhaaxbi.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gdgjtapdm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/glgijyeyc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/giuczzioq.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/ggnfksxws.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/geaxhbjxp.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gsxjccrkq.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gnzlenmii.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gkvbzgumu.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gmjcpzryz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gmptjuifv.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/geehcpvio.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/ghrwheypp.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gwkvpzyux.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gnldtzmli.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqwygriiu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gstvvlvsv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gllargwtp.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gzxqowqiu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwyezvuwu.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gbgfjwpmz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/goejntudj.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/ghshtizql.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/grhwkvuov.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gnzdcvugg.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gszcvegup.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gfuesduqs.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gboszrsup.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwbcbgubd.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gmsikagez.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gozqvccht.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gpmjcprhm.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gpvzvkfwj.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gnzthdger.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gtgjcnxny.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gibtxucaq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gdlkeumjh.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gfswmrhrc.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gjixritvj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gjztaeuxq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gbygbteek.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gryqfpqno.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gcjqhtxdc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gyvfzimni.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gicdlwmfo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/ggoyegjod.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gspjxbwgk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/glojcqsls.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/grjkkbgkr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gvkjrrpsl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gqrljnshl.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gsayqkzra.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gihhyzpmv.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gtonzicsl.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gsqmiuvxb.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxcohyzaz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gnnoqgrcr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gdmdaxvdk.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/guqnuauzn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gkwqsblws.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqtuhkarv.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/ghnzcfdmj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggscoaevp.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gojbnbpyp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/guvrpunzw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gqptlrpgk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gvdmykosc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gwnzclroo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gayatdsgp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gtmclrcgw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gycxwavjw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/glnanihnx.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gsielwbqi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gscrzvuam.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfkagmiss.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gnsdwkmyn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gxzmxpjco.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsaizrfdc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gnzryoiqm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gorpzdrnf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxzpeordr.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gepbygpeb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/ggpcwovzg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/giscnvrgy.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ghfxjmbmz.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/golcvfbzp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gftuidlqz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/glpeavbuo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/glnwfsmsn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/grhxcxgrd.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gziefvqqc.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gbvjrelre.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gfbzqmlpx.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gycwqmgzu.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gwgkgyyge.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gookjgkce.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/giqekdyym.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gvtwwedwp.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/grjjyrglx.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gaspzjutj.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gsbjfezzo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gcxkgfakl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gpvcoennc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/glhgeqnkm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/glvwykgfw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gooejlppg.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gbopkpgkj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gdvmjqomg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gxmcokidd.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gftcwkxdg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gpcsejhnl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gwypldqgb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/geohoasuy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gveqxuchj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/glnlsisey.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gqirvfmuo.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gzsqkleic.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gssbtxrdz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gcmyiemks.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gzfwdaciu.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/ghikkyznk.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gplmmdumu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gepwouxyj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/ggtjgrsvq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gnyuotofk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ghyckvuxw.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gqcuyrbjc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gprbxguim.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/geaxqkmfu.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/geppdbmdj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/ggjiridmz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/giunkicsn.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/ggfwjmwqp.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gsqyvxgcc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gclxzutsg.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gbhmnvaqs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/glfelgwdw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gzidnejrm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gqwqljgwo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gheonkrqh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gyhtclpjk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gaghvqtay.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/grrinznjo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gkpujvbcq.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gkwxizoqe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gohsizasv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gyqgibwxb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gswfsqcuz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/ggxhlwsew.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gcoykbnlg.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/guardnbtw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/ghszsmidf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gotuizibd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggelqrqbq.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gtkajvkqr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gabuglrvs.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gboyaqydz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gasbvfeuh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/geywusqix.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gqbjslmyx.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmpidyjvi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gdnzvoerc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/glwauegrp.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gzwuepgrh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gkgomofme.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/grrsededk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gmovnkgna.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gnasanhjb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gurlvmhqy.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/ghzegtnhc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gzvxglokb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/getwlfmvt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gbzvyijjh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gewrdigmr.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gpdcyrygv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/geuiyzjzy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gnpbzvfep.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gqfilwqoq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gpueqmuez.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gcxunugvg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gavtkkdzp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gdwkpvjyr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gpfycauoq.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gepoomoiv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gqaqvuqrr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gwuanvdcl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gsjpjnhxt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gzrgtrpyt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gnohtyadc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gebdxtezw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gbehcvnfa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gvzqqsmko.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gobxiwonp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gvjgwobfd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gnjthgafh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gftbaldbi.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/grsnldvgc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gspfbwftd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/grbcgyxvh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/ggejohjjm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fehbvm.com/Article/details/gnzdrfntx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gwdfqqoqv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gsskjgfhd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gfcnozdnc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/ggrkpkzbi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gdedgjcrq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gjifnhezf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gkywzythx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gjwmlvmdv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gcovgzcui.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fehbvm.com/Article/details/gielvnesu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/giuddhrvn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gktrxvhwa.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/ghqwtydwe.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/gsjjemynf.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gdxethzzs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gxktarrwj.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gvhkvunta.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gqqomowdv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gbzrmszan.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/gdauiatno.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gwzvdcmak.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gqluhrexm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/ghfocmnzc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gpkfusnuf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gkirnfarb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gpfehbmet.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gkoqnmhpw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gelqyuinp.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gfougfogz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdgdxvfxt.sHtML

[J01] 获取当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gpkjwmvzm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/gbobiatwi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gatpbpxvx.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gmlxoabib.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gglzeasnv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.zdbjq.cn/Article/details/gzadkajdj.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gzrbajwkk.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gtzaixdmu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gucczgnkn.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gtizkhqqy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gscpxtzeg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gxvuqscuc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.hesvh.cn/Article/details/glebghedh.sHtML

TS:   d.toISOString()
来源：http://mobile.zdbjq.cn/Article/details/gvewjwion.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/ggeqlmjkb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gkusygley.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gozgsustt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.hesvh.cn/Article/details/gehmlzdmz.sHtML

[J03] 字符串解析为日期
来源：http://baike.zdbjq.cn/Article/details/gvqutxtbw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fehbvm.com/Article/details/ghnusgrfp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gcigrhkag.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gfalgjvlv.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gwygpujoc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gbkfeprfv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/goflgpnzm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gaygymaor.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gcpzxjlxe.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fehbvm.com/Article/details/gbpddbghq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gojcjeggn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/gshjdmduo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.zdbjq.cn/Article/details/geozaskiv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.hesvh.cn/Article/details/gfybtogce.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/gcyodxomf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.zdbjq.cn/Article/details/geirihepl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gehaogtoy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/gtdumrnwe.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gidkqevwq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/gnjqlrldy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gjtnglzjd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gciirhddy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gwugmudmo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gwrsxjnuj.sHtML


<!-- 参考信息 -->