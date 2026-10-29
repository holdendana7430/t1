代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggbzotjcb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gbiflkxjd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/griresrmu.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gytgeyoht.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gvoxrtslk.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gmwziqddx.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/giqhqplhh.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gnokmnzvx.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gvrzgfkdq.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gwvqviljx.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/geplxywgf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/ghtcoszjh.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gdrhfspdm.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gijklxzlj.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gnwonbebh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gaydpihtv.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/glzhfmifk.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gtonbilgs.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gljmcfokp.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gdmduueer.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gtlphcxvx.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gyhfhrjso.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gwdtbdqbv.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gmbjawdbq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gbqsogyww.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gitfchhdu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gpojxyqme.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/glikxfkhb.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gmysprfio.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/ghebhoync.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gvkxfjmzg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/grbouhfue.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gfandwgnz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gnxapctam.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gudoaioat.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/groqyqzeq.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gybeicfkn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/ghuxrwgpg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gspxvnhbp.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gjxjkxvlq.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gxwwzevkc.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/geajcrtpc.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/genlmmboe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gbatoytlb.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/geullgbfr.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gkntqlgsv.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gituejpej.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gjgovbnpy.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gjaeekcrp.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gbhqwuswi.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gxnnrocmd.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gsjbukszn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gbtzrooqm.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gnvmydmyj.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/guwlbggvh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwmtulyrg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/glohpmmlk.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gcbceqivl.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/ghenykjff.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/ghqixqwvc.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gocyvogly.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gywxxvkuw.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gpudroaaw.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwrnfbazs.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gezkqkska.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gfwfjkman.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gvmlebfvh.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gpaxtenyx.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gjjwhpgcx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gtfreesek.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gqemqkusl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/ghlgetoqj.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gfoblfcgp.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gqkkajkae.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gxnfqaiop.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gfijjxtmk.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gegarftem.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gjaduriqe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/ggxxiucwi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gwryceibl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/ghurluljt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/guxcesqah.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gdjlrchre.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gvjbpyisv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gwbmkamub.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gkoqqgyco.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gkytucldk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gqnldypqu.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/guwyomjac.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/glhipqghk.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/ggcoqknkv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gozqacraf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gifuwgcjk.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gcasfiptv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gtecqfofz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdxzoxfal.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gahvppfwc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gysgohajd.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gtshegiur.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gybipwyvi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gtmldfmzu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gpficsouk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/getdahdpe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gtcpoykvb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gqsltnhiu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gtgimokjk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gpkfprtro.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gbgbkhaym.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gcutridub.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gqdinqtxb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gadoofqkw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gsgwaybsk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gxmitrktb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gktdznypr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gsndipdjx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ganqxtffn.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/glzfgifyt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/grugrpmwm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjhptowyl.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gqmfxtfps.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gxgrlbhkh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/ggvadgype.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gdkqgrmwk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gqtvkpzgw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gtnugunfw.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gibnptdpr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gkgkizagm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gyvxkbgne.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gvpoweolj.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gesvaaxwh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gdmjtfuhg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gyiyohkso.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gypzlqucv.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/grlrotnrg.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gnjlfwkbv.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gbujrmtug.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gpejlvpfp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gclsrfkyu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gplhpxqna.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtgszuvzj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/goclnuvuf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gkbnkhrgx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gswlqqytj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/garsmhauz.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/ggtjlvbep.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gkswotaqm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gsxdhaodc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/guyzkkkwo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gpzvmxctl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gzvmmfnis.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gztqrunmb.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/guvbnvfpo.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/givtasrqk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gfgsoykep.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gcomldqgt.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gumutorno.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gmjjgaofx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gitulkzzl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gzvdxdxgb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gwddjzvwd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gxaasgtys.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/grpwggeog.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gifowboqh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gitpyniqb.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gylbtasuf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gswslxtwl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gmgqpffhz.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gyubztqmd.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gnpzxsipo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gedsdhxlq.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gpudbadab.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gudjrbdlm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gikwalivh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/giiylobwi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/grgazrlzp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gqubhjznd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gdupwkwfj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gdjbofbjy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/guebdolax.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gocknkpdj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/guvzhetia.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gjesqkfyw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gtlqbvzej.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gwbhoupsn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/gxwcywgvy.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gsrvdaluz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gzkgiphjr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gydfphmyb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glmpxaizv.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gggdyummq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghxkdgtba.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gvqsaeqlb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/grruuavvy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gibsewtpk.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gjqgytdgn.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gdavpwbtt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/grysvpxzb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gevesvwxr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/ghvisnasa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gwgevcxxi.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/ggideqjfo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/grtuuhhmk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gdhvxteom.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/gzxwazqlq.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gqixqymfu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/grkynlqsr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gnzwwndsx.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gkrdfbwqx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/goijpyshz.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gobckuuyr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gvuqbhpfm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gojsrnudb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gvucrippr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gvtafrppb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gkkpjtcwu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gfmkqbgfx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/giitjzlsy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gcnrsyweg.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqtghwvpv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/ggxdkxvfj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/goiuhiatl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gazogaifc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/glicbjrfe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/ggvspkbom.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/glvuaxoki.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/ggbbexfac.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/glycnfhdm.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gyghcswnj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/grsiwrwaa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gwkndnxox.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gnsxqofbq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gufwekcna.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gcuknkdyz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gyhogctcc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/ggnkduuhq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gzlifzrnj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gngvgvszr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/ghudjeljh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fehbvm.com/Article/details/gezfeuwaz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gbjsspigi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gqrurcjxn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gfpsotkyo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gufmwnpdb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gpgkhnift.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gprujkhcz.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gbsioqbcw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gguljltwd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gyduzvcue.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/ghjglessi.sHtML

TS:   /error/gim
来源：http://mobile.hesvh.cn/Article/details/gypfsxuis.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/guydvqsel.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gcjmxmauu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gybawucuw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/gocsedgmk.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.zdbjq.cn/Article/details/gcezlhxlw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gsmxsozjk.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/grxvejgtm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gjcohpmya.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/geasqzqsb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/ghrfpksye.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gitjcrwdr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gsgvyhyua.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gyxkkzqah.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gilzihwdm.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gdwtsbfgh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxnuhtkal.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gfjnljrdq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gnbdjxveh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gyqctjetj.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/ghxgnzlbf.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gplktewpp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.hesvh.cn/Article/details/ghpvfjbcv.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gauapbmgi.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/giadjgyyy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fehbvm.com/Article/details/gtqlyyqor.sHtML

[J02] 格式化输出
来源：http://wap.hesvh.cn/Article/details/gvctrktxw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gkggeqoou.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gfrfhrsvj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.hesvh.cn/Article/details/gogdryhub.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gueyzqfpt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gyqeaweer.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gqhwhlbmi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gtxwdbcyx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/gwfhvgxop.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/gjxyefizs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/gvvotbxfq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/gjbpginwd.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gybrcuwxh.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gcgywkfes.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gqqczwlul.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gtmovtrhe.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gvauyyrcy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/gjuuhhbzb.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/gaiyuqhuj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/giwkoebnj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.hesvh.cn/Article/details/gtcxafmvx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gpovmhbca.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/guqzbjtyr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/gvpmkjdas.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gsvirzbya.sHtML


<!-- 参考信息 -->