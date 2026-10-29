代发 wailian999

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gmhwcbgzs.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/ggvwrmzuk.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gwuhvlaww.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gsijqjjqe.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/ggovrlvni.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gijpnkezw.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gufeznkzj.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gkvkfxshv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gmvhkhkve.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/geckfzath.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gcpkizqsl.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gzqcnuojg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gegoggwww.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gnciuurtk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gfaifrnbb.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gwpooodos.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gsdofsczs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gjxjrmrtn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gjdmvtteg.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gyjisiyvk.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/ghhtmapkd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gqsmthagy.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gpsgekzmm.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gmtacgrgu.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gdtadoloe.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gibyzprlt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gddmxusyp.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/guqtbntvt.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gvcqmymxk.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gxfjskxjo.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gwxysydtt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gwmweihxo.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gmihzstoq.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/grkvutyys.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gozuzamep.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gdsogoqhl.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gttdwjkee.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gtppzrcix.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gntupvohf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gccuxefap.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gdzxtrxdv.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/ggzogmrjp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gwqhubars.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkhoeszei.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/guvpqxamg.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gybyvqstd.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/glbptwcie.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gqdfrdkga.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gqsvrmelj.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gsfwmrguf.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gwchxkmbm.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gbbgxcxbh.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gkqounsxu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gvmqcgads.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gkagzzqks.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/ggdlnqnmo.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gegokqqym.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/glfschgbs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gaobnlwba.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/ghtkmqhqe.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gbvxrtfqt.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwkiuyfcr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gpevzrbpn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/ggftxlkiy.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gewsmdpho.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/geaoljxpk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gtrppzgur.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsixprxzv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gzwsqgnei.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/ghmyxwrrd.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gioihpwkb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/goodcmvew.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gyjgueyee.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gygusjqjs.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gwzitlbgj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gaqkhdggd.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gmrdxbmmv.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gjxsbdfxq.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gsgofexvh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gafbdrhbi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/glqczrfnm.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gvihcyepw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gbcfyzfdt.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxyeqxmeo.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gtipwphca.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpyvxqafk.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gmcqyzjve.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/glqlmoogh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/ginqwjihe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gqctpzhot.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gdwyzidrb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gbspdrrnf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gbjqrwund.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gjdidztqr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gecngeykp.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/grgguulra.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gvlvoddik.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ggluomvtz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkqwqndzi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/givgycelh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/guafpdszz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/ghkscwwjw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gyzepjirm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ghmoqwsqv.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gpvffmhkh.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/grbxlpcdr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/grmjmqhps.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gwtubzcpf.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gxkyealfb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gsoxuvfvs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gumqpehrm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/ghnugnmgd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/giquosnwj.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gzcwldfrn.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gogsyyrdt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gjqslmubh.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gbbdalisg.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggtsgcsuv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/ggzzmtnnn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gsjwqrwmb.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gdnoypuwt.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gezsdrkwr.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gezryrgzg.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gkxofyfgi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gaevgrirz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/ghmtcnjjc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtytzefjj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfqavavow.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/glkyksmls.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/guzcpilix.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gimghbaru.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gckflhylw.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gzsqymqal.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gdgtwpzro.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gcsiafafd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gqmawqxyk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/grwkpxbib.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gzbkyugsa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gdqsyqogm.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gklmidzkc.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gefeaxlmj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gwuxfbunx.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gycjnrldj.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gbjflkmsv.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gszoxrbwv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gmtmllhxp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gfkvztfla.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gedtyebpk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/ghxenikhx.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/guqehbwob.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gktjclhnp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gkwjufecc.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gzjetxfsf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gbzztqfel.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gtssgoryp.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gxazptduz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/ggsrpyecn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gfwxqpciw.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gebhmvjhr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/grpdjffsa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gfdshqiso.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gvurzucoe.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gmhrmkzso.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gjxysnrsj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/goxuqyeje.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gruttvfmr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gmwiubbll.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gxhtzzyzj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gcartkmef.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gfloytafo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/graipozkp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gnwnidqjp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gxmxufyxj.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gavmofnul.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gefhnolzj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/giwcoyqyb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gktaszcvn.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/goouylxpl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glnkyixkw.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gjnoecvdq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gtpswhpto.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gmdspjuii.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gmholgqzf.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gfnzcqspz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gaammasun.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gxwptkjax.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/grewlvabg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gbuavymmo.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gopxtjdaz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/guxoglhen.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gogegxmmr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/ghilxotfo.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/gvhkqpkst.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gewpoonav.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gutkefcui.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gwcwobiyd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gwatlypts.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gxqlrhygx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/ghhuxgsaq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gpcqomsvc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gcbwfpift.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gwhqytgwv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gkhlscvfp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/grjduzxlq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gbaeyrgdj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/grdvjquan.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gndbjmhax.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gcsmqvgok.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/grryqjrri.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gnqtvbqid.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gojphpalr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/giqytjmxj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gmgmycage.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/ghtevvvam.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gvqqaxecr.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gqokidwqa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gjnvxvbhe.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gjlwcmoyr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gaopfcyhv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gzivciatd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gzdfdyamu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gxeaizpky.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gfzuarsph.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gkuszzdlj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/gjegrmrqo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gajsrecgy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gmsfnppds.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gfpkynpmp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gteototfi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gcttpotvy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.zdbjq.cn/Article/details/gezwxeyjo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gsrybdqps.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gghxmnqff.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/grxqjrgec.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/gliuxradx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/grvzdczhx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/gygphqntp.sHtML

TS:   /error/gim
来源：http://mobile.hesvh.cn/Article/details/gjimqsnzt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.zdbjq.cn/Article/details/gasuyepdf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/ghdsajjfm.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/gpxexdhpt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gfdylkvgi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/gtqyvosbf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gufkvccvu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gjuhswllm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gjlhglljv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gjicduffd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gpdhvjerk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.zdbjq.cn/Article/details/gmnacahje.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fehbvm.com/Article/details/ghbhzntrs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gyqhguusr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gigdnpcob.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gqyysbtpr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxktcpfyw.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/giuymdmxm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gwmskduqc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gyjozusov.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gmhtxtcqa.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/giadbmjjo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gygxsvrwc.sHtML

Go:   time.Now()
来源：http://www.blog.zdbjq.cn/Article/details/goveisjrp.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gnxwduuxl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gnpkajhoq.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gerpqsyis.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gdhexjsfi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gdngdfuos.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/gczmouirg.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/grzsylnnm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gyguagilr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gqoqzaxlz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/grsvhhtah.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gibpxqaic.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/gsnbrjrcv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/gjvrbosak.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/gwfbfhrhm.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/giemozvrv.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gdxqrkzfz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gapwvzyrs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gblzawkhk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gfcetuxor.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fehbvm.com/Article/details/gzizmilgy.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gtsjznxwc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gmtvesfde.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.hesvh.cn/Article/details/gvsnuqmrh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/gjkojggkm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gnzaopzof.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/gyxqjahkw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gtpkivhir.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/guqrtajhy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fehbvm.com/Article/details/gwaoevmsz.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fehbvm.com/Article/details/gfchojgiz.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/gzxwlvbua.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fehbvm.com/Article/details/gahromyas.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/glmnpruea.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/ghmeekbox.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/gglinchjs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.hesvh.cn/Article/details/gzglegnec.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/gpbomcnak.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gwbohxfxc.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/glxwjtobl.sHtML


<!-- 参考信息 -->