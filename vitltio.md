代发 wailian999

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gzsvqqhfy.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/grzipfrlz.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/glrhfexcm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gkdprbbgc.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gkzfdyveb.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gpqwspgnt.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gkfxozvgu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gvvzmctur.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gtacarrgk.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gpxshocso.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/ghevdohcr.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gftnajjsq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gxgxrmqml.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gejifgioe.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gewdpbihm.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gcgarxkmc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/geepajeof.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/giqmayidc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gkcxppsos.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gpcvbpqjv.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gdulxcwmz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gjqbsyoxc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gaugcnurx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gdvwywbvl.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gjehnppky.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/ghavxjhny.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gpexybvdw.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gvbiddjtf.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gfioegvbx.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gabozzfhx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gikmixbhe.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gzcybttni.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gfytzgwwx.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gmyqeysme.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gyghlhpba.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ggsqwbsdq.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/grvnprvcb.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/geygqrvbo.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gadpoofbw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gdeefzkpu.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/grmifbdcr.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/goearlqpg.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gpmkfkxra.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gxuggptnz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gpnfnhsvv.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gznldrwaw.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gqeyqjkgm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gljkafflw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gsixnoewi.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gjnguhate.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gktjlpecw.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gfqphojhp.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gmaofpxye.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gesvdaelv.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gocpqbvfi.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/ggbgyzeep.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gkgqfheod.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gmujxtqgh.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gcofjypwb.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gsqzauece.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/ghblxbvjc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gcafsomdr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/ghdxsdsda.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gfazrjcem.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gborbtzpe.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gxwqyuogj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gcetqitif.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/grklakcgb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gpiydpncw.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gpyuajqvx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gwxsuajih.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/glvzmihpf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gsyeexuzd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/grahrzpnw.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gsjzfrmnv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gajnlvbxj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/ghdsjwpsg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gawvziltg.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gnqwfshhz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gdsefvati.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gqbyufmdt.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gegtkokqw.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gaqvhsgwg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gafxozaho.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gnfuzohnw.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gkxwmfxxs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gcfcepelj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaidnrare.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gucvotytz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxcygfkbh.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gmndtgwey.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gyrdndfby.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/genwrusie.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/goaldarkr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/grwkdhiry.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gzyzzcuku.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gvmuuvndp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gidcpblpc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gorjkxmtb.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gjnolykoe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gqeglyrxb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/glifhfxrz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gpdpjacim.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gvenijcqi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gthhrdyky.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gqfebazdg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/genuqclcf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpwygtzvx.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gefmyewyd.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gngzdbsrn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gyxeybbxv.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gesmwwzcj.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ghklgsfcj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gxsqcblot.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gzxbcyeto.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gxhuxhtvx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gwqbxsmyb.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gtbrnfkrg.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gvpgwqwew.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gmnxwlrik.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gknqtuomh.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gvuxjlhyp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/ggkeajbmx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gycvbzikc.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gpyiizgjb.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/ggfbkvxed.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gnbknhosc.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gfqsvvqnc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gnmezfuxb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gjnnptpqz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gfdkxnrxf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/ghyodkijq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/ghhtlangc.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/giasxhnig.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gxvjgiosp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gclrfqloo.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gdffdgzth.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gsbptlcpj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/glihyusny.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gwjkibrxz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gzycqgsuh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gtbeoxmya.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gmclypggg.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/geofmkhba.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gelbjmbyn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/ggnnockyf.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gkrrjnjwk.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gilflqtpo.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gthocnvyt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gunctlnsb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gypvefgpi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/glkyksjng.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gtbnipyxh.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gdvpokqph.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/glihshgcp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/ghzrncbrg.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gntdyysrs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gftmiiznn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gsweimcey.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gpbtgbsdw.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/ghpawqlhi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gmujospgw.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/ghodzwiwk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/glrioewcy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gfzwcdhnw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gnzqbfojs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gejuejngi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gvgrvbscb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/guvbwioyx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gogwysutw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gzftukiqz.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gjpvrdloc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gwlsiotka.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gjuaiooob.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/ggzdgprum.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gtfdqavjd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/geuzilhfr.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gafunmdha.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gshxthyoa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gejejuoaa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gksspkmab.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gyvtyscel.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbkflpfsm.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gvywajnnc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gozwfbwfy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/goczueigl.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gtficxdpw.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gkjohrecc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/ggzyvgvch.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gmjljhjxg.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gfcuamgdh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gbbymbnqr.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ggsvzjsqk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gnhibqeqq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/giuuhkqui.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gwttariub.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/grgaxfnef.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/ghegezowu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gmkaffxbh.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/giutojzwk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gskrommkz.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gxjtnjqox.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gzzoldofw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gpaoslric.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gawmfbonl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/guqcusijq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gxjqwkmba.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gkkbfvdeh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gjfvauffs.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gzetwvsry.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gggbxwmts.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gkbkxtlhf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gqdntaukd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/guqizhzqj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gcqqzsdkt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gifwnyvlk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/gqgjpezsx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gctgystvx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gsyozljpy.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/gqsfyaqgh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gulgjpfom.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gylwjdvqp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gtkyxltii.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/ghkxnncng.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gdqhsaaqi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gblmwdmne.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gbsnsjrjq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gevenvpmf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gcswrkqlt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gypjemfez.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/ganykxhae.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gtcnsgfhb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gprujzyrg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gbhiabpae.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/gfmomvrkf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gvepnetwc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gvhlwrsgz.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gekmoikmp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/gikehhkxn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gzjammnvw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/gjpjzfxhf.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gehtgduri.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.hesvh.cn/Article/details/gagaowoif.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gcemmprxy.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gftbvyjdq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.zdbjq.cn/Article/details/gdyuqydgc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/gpjbikgfr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gmovnumto.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gxujkpkyk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gdnzfwpsx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gxtfidfzt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gcceifzxf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gbbwdzksq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/gfstrbpwm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gvzppyupp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwplgxepv.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gjbbemmae.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxetcaflz.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gsbfeqzfb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.hesvh.cn/Article/details/gcaocrkjb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gfxgnmbdn.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gktshsnzf.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gdpvdvzxt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.zdbjq.cn/Article/details/gkmqchrjy.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/gnwbofvjr.sHtML

Ruby: Time.now
来源：http://baike.fehbvm.com/Article/details/gezehurfk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/ggjcqdsnj.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/gkucyjywk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gsyipigaa.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/givdyfpsf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/gmzzujpzw.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gssngorqw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gqwzdfady.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/gqlfaumtk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gtviphauj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/grjmcpagz.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gqrebqyvj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gqvshqgnx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.hesvh.cn/Article/details/gspozggwz.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gkaqahahx.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/ggthbceun.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gxvfjedze.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gjovttbrh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gabnhnrno.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gfealqytp.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/goozrnvoy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gxhehylqs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.hesvh.cn/Article/details/ggbigpnoz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gpvtneygr.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gkqwgqgow.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/gkxtxmxwf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gqbzjdnsy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/gzmdtdyvx.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/gulytuzdg.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gagmksfga.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gmssyqpdw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.hesvh.cn/Article/details/gqhcumurc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gwpldbhjd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/glmpnzqce.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gzthsokyr.sHtML


<!-- 参考信息 -->