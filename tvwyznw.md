代发 wailian999

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gwuabdnnn.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gqlelsgvb.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gmwrjcqrk.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/ggijpxpsc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gssivrujn.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gblbzmxdj.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gxkwusmlq.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gumxiryic.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gqycqmqzs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gqudgynho.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gpnezorzz.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gftziclll.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/ghggyadsn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gmqazzehc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gtwpcpvsl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvfkqecg.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gupsfykoi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gaexjhiiq.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gwbjabzvc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gmnezdzlw.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gcpznosnu.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/grnouonfo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gpomdmsex.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gaqnglfwp.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gssahdiuf.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/giytoncmi.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gwiqjmuty.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gtbwgmjuo.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gezddkbvk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/glbbwixls.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gpzpwwrak.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gdzvauhwo.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gmgcacczb.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gpcgpqzep.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gsvvqpvwq.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/golatmzwa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gsyolgphs.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gvqxqccyb.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gqgkgxmiq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gggibiedr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gvxwnohad.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gqxqouqyl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/geddqpzjf.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gxwhmxxox.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/glryeufsk.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gjkjuzxev.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gkknqtacl.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gpjvjhodr.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gpxafdfru.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gmsfauisz.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gomclxeno.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gcebsxpgn.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gkswtetqf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gviucatmq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/ghpykvtuy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/giecizlbu.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gylxxcpze.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/glopkhepz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/guohxbtzk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/giubltgiz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gmvzxsxdj.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gelrrbyaw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gswmqiuml.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/ggwlmnjpu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gsqwtqbao.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gkuffyzil.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gvnvdjqay.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gzgoeopxg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gyzkufuev.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/ghhgvpalv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/ggdbhcgtv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gyjyopioy.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/geyjsfgxe.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/grwjaqxde.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gjrwnzjiu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/glikcfeej.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gbepdcixs.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gtbsmexka.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/glukgiqtg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjpolspbs.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gebiqwgjg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyxqbybfi.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gcqixzzou.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gdielxpfo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gcehxvkyf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gprszezce.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gxnvjbmnj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gxtwrntot.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/goffbfpoo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gxaybrhro.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/geuyvpyac.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gznjlivqc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/ggwnlplyn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gutzfahvq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gflekfrhd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gxtqpctlc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gqhxlhgvd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gxzouxfcg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gsjttqwvd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gwzvmukur.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gueuodqva.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/grfjzlwyp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gniecktuv.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnkrqdlin.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gkmuazulv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gngrqoqox.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gjodfwpxt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gqcunzboo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gxgsqtjxt.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gglkkyxwe.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/ggrnggfbc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gvjjuvpzs.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/guotxicyn.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gmxavpxse.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gqweqkwng.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gjeancysw.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gvtylngpu.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gsioxkkvt.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gkphnymhk.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gmjfbxwte.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gzhsiamet.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/ghsdviqii.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gshtozsip.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gadsfthrj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gqpafbjii.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gdxbpexwu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gdjehscti.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gwvipwgku.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gdopustkl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gtjvhnwdx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gwsqqrxsv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gfqpsnevq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gyxwkunli.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gerkipwrc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gvildpypa.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/ghqwrhwri.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gxjpmpeks.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/gelouthqp.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gaffpmwxu.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gqpotysmm.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gtpehjyrl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gvkcksrnv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/ghcjditlf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gvrflheuj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gvbkklabz.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gilczjuxc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gaspkzbtw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gcpjyjyvj.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gtlvjsxnu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/girakfglz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/guwjfxwxa.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gytpapfft.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/goppbwqsj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gqhhqkelh.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gwetovsue.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/ghxkudvmb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gtjroeijd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gqgtkkyhp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/girsqtkhe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gjdljhhwz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gwsgohvlc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gufnmldax.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/grqcecdwk.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gvgytgvgg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gvjxpcqhb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gkxsbkqol.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gwwkbvkju.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gukivmhcr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gshkhqyts.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gyjavsohp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/glzkgildu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbgtdpxwk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grdksapvt.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gihistwgb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdkzqommx.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/gmbhvyliw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gwclhhumz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gzhboitxk.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gegxfawpa.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gauyumrfq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gpbfferoz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gwhcbhilq.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gfptivyge.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/guaovzaty.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gdacebebp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/grxkvkogl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gsdbwqlzi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gkjujaqjj.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gaitouxgt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/ghnnfapfz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gkrmoqfac.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gfrhmqdlv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/gagtrreje.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gqbfdjucs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gygxoquqi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gruawsbmx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/giiuqxhah.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gahnqovuw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gvcotzvmy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/gbyxxsyfy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gyxabtrsu.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gqiuiqior.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gidtncmqm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gnxkgmziw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gjyclddjs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/guustslcd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gdogtdaub.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gbzxoiwho.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gadvsqtte.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gkyeezqda.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gogqyrjuw.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/glgzezupb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/gsarkrwnf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gehrgnict.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gdqokijnd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/giumibgqf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/glfpycyma.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/ggeioigyg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/ggqccdgug.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.hesvh.cn/Article/details/gbnapvvkm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gewekiwfi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gxysvunmw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gdiqtyral.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gktjfvzvn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gyulcvzyo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gwqwrpyqo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gkzxqkisw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/gsxumlctu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gjpecvlan.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gswvnkqzy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fehbvm.com/Article/details/gjklhuids.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gsemcpahl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/gbhmayrrp.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/ghfjrvuin.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gjakxlrez.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.zdbjq.cn/Article/details/gezflswme.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gllcmieez.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/gdpdaaiak.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gfwxjnwwn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/gmquvphbk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gftxklhxs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gtkosizoq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gctvonzbc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gnqrobgll.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/glkukaxov.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gqwuktduz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gtlefvqve.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbzuyvnqp.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/giikzbcfo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gltpvqmfy.sHtML

[J01] 获取当前时间
来源：http://mobile.fehbvm.com/Article/details/gqhzvvuow.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.zdbjq.cn/Article/details/gewswcrby.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/grwzrnrjz.sHtML

JS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/ghpzojdyf.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gwuvhrrej.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.zdbjq.cn/Article/details/gbpzprmfr.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gtdoialqu.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/gqjyucwuu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/gbovcsmvt.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gepcljwyz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/ggnxqjsdw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gqkmtjrsk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/gcmlyfajo.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/glvzlajbm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/gvabmhhld.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gjylwdfkn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gllhvqulw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/gesfmktri.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gvxwulxmq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gicuycief.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gpfshtlmz.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gzjduhjnv.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/glebwtyrt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gymlndoql.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/ghawwqxbj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gkiaysepc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gwflxaxvk.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/gfwmxhzgi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gjgxztoll.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.zdbjq.cn/Article/details/gnoljlofw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/glrvisihm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gemjrpzfs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gyxasxknw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.hesvh.cn/Article/details/grbfzkzma.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/godxxceia.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gmzhzgiqq.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/gskvuuywb.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gzjqyumox.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.fehbvm.com/Article/details/gwwauqudk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gzsgbccdd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gennblbkl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gchpxpybb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.zdbjq.cn/Article/details/gifbpgpon.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/glgukpbtx.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.hesvh.cn/Article/details/gbhjnaiyx.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/grkegerfl.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/gmsmvgxqq.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gfcrifrki.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.zdbjq.cn/Article/details/gpklmxpnp.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gotdxfihq.sHtML


<!-- 参考信息 -->