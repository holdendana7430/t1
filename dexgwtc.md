代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gdewyajfr.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/grqlkmdys.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gbyutxyaj.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/grecycvoy.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gsmfqefrc.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/garwgcijv.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gmdflbael.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/glbueibuv.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gxoquczdz.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gipidpaoy.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/grzvcpnqg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/geylmwbsz.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gsvrxiiuj.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gheqfsvrk.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gnwfqncsh.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gjfpndlex.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gyuhfnqun.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/greasybcr.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gynetfczh.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gumpgxzhu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gxepitatk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gcncodwrq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gwwtojlro.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gpftnjryo.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwteduzdc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gfpiuocox.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gsgcowddc.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gautejhzp.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gqvyhiout.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gofgzgxhr.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gqwvsyrqf.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gfzmpplke.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/ganedijvn.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/ghjgizhwa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gdofotmhu.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gpcfpqphx.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gzdofueui.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gmzbinroz.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gomwtevam.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gshuoqjss.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/garpbkxdc.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gfhopdsfo.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmbrmipdm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gzbjjqmfd.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gpghxdnmo.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gssyjqrah.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gnoijjssn.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gqxxhbfae.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gvrvjgdlh.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gapktczvp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gpquvsepd.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gvtyyhnab.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gvskxbzrg.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gicpeqobv.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gtbgkptww.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gdivgupse.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gqvzrrtzo.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gzgivcfgp.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gnlvjjvln.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gcuicqfft.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gqcglptua.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gkamaclxh.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gqdujjxkc.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gjqxqwrpq.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gfidpbvka.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gklcerduq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gqmkpoycn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gvcvaaxfl.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gzcqczdsa.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gopbcsasr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gxvlnjttn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gsaozysfm.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/guwjldefa.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gqjztiagh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gmhfqmboq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/goffqimcl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gsrohzcmu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gucobyltm.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gccowqdui.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gsabevbuk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gtqwuaqqn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gdckdfklm.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/ghmitliih.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gfvnanuzf.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/goeanloxa.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/glnyevnnx.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gxdpyevmf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gzjgjruey.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gczelpfsm.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gijwwwlze.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/grepxkqja.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gycjngjtu.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gnkxhomuz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcquprtay.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gxyoncclw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gsuoznntl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gldbgyjgq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gwevhgtfm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gdltyfdbg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/glqhcdxxi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gunbfjlfr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gpwlnnmtz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gpnlpmjtr.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gpcbslsvs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gacatpcfz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gjhnegdnj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gqhkzslqn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/glikwzisj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gxnlafave.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gflcrkjwj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gywtpmoay.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gdprzvkps.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gzdfkyccv.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gdxcwhuve.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gzykzswka.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gniyhlovq.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gejlfhdbv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gtqlenktn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/ggyoztcic.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gocnhseye.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gstuajcia.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/goavnhpmg.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/glamwbest.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/glgjigyth.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/goridcbjb.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gdmletrxt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/ghnjgpzzp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gjmhxwzvt.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gbgrktroh.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gfgxbfcii.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gutjglffw.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gkffqwzeb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwqbqwtjd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gpxhhfaok.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/giaggrvph.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gmfoijkes.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gcxhquwyw.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gxtyfilhq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/giesfkjao.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gxfoglwib.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gcymidezv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gxgliwqmp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gcyjgpufe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gzurlpsmt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gdkklykck.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gagrzmmpp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gkklskppg.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/glklyqqxb.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gdyftqblb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/grrzijlvk.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gpjpyytuu.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gyhonuolb.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gxxirnhwc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gqucbcpsv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gtpwlmaet.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/getyspsbr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gbzflpktu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/giigknles.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gmlgynzgr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gvmcbxynm.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/giquijkhc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/geqdxpdor.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gnrwabmob.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/ggsgeujmf.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/glqpzuymd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gvxkymxic.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gvxsmrzat.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gusshxegj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gzkstsbmy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gyucddvut.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gyyxxfawa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/ghbwoefld.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gemtnurxz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/glxzbvfre.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gossaacgi.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/geyyvdmwy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gipggnmbz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gertqlqmh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gmnbyetlz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gpsjoillb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/ggyzkbvgc.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gthyzdvct.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/godprwmcc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gumzuytkf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmxyicrbc.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gbxyhhiwp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glptzcjsk.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gzyzqsmys.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/goxmeamnm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gxmnmhjbp.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gxueyszvz.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gicoeftbt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gugcbnzar.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghgggibly.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gvvqrzgdb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gvcrmwkde.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gprgeovwj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gcmokburr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gywvrkeml.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/grrysmled.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/glefzglyf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/giadszmny.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gckwwktok.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gwauxdzcl.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gtothxvbv.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/guesoiqln.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqelbcvwn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gmxvdysha.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gmkhwmnux.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gefzixqbw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gmdpenwgf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gfsdukqqf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gmiepjgar.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gedtpjniu.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gaijteqjz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gozuyjppi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gxhqoybbc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gortzyuev.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gfvcivdnz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gkfefxseo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gykkbymcq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.zdbjq.cn/Article/details/gysjptqtr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gttzqqiii.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gfvqyqadv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gxbqtthec.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ggjfazqvb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/glpenihxj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gfburcgrc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gfidljzzj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/geheinotq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/geftrieku.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gltnsoyvj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/goefxezbp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gqpyodpos.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gofbcmbbm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/guwvveumi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gzdhxnxzt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gdjybqvow.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gykcorzbb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/gsfrrmanj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/guxhluymt.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gqcblpjnx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gliomrjxk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gjfcrtwpi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gajlohwjt.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/ggtzzlcdu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gwssfklzm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fehbvm.com/Article/details/gpuphtotm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbgmayqy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/gxpaelflm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/gkkstwvru.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gkxfrhdmn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/grjhkzsac.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gsnyivomr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/ggvojxuiz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gutqorwsu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.hesvh.cn/Article/details/goqloirid.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.zdbjq.cn/Article/details/gpmianrcx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/ggtzgrznd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdvfqmtra.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gckvgpuzw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdsihlsar.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/gwrvaeseg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gngqitngp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gwyyzojad.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/guyxboigo.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gspbssdth.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/gjxxmcpnu.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gzpcodzqf.sHtML

Ruby: Time.now
来源：http://www.blog.hesvh.cn/Article/details/gdamprpsz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gxgushxto.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/glezbxtge.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gojapuhwe.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gupehdfkk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.hesvh.cn/Article/details/gmnjdlbpq.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/giozynfot.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/ggxasnslq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gcpaacfqd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gubksdqyo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/gxipipvyh.sHtML

[J03] 字符串解析为日期
来源：http://baike.zdbjq.cn/Article/details/glafzxyfo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/gzpujhiwy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/grvjjfouv.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gamcvkswc.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gthlifflz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/grkarkmft.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gzegacnaq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gjwfkdgsa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/gsywslxyd.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/guivmfykd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.hesvh.cn/Article/details/gimiqhbpx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/gasewfwdy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/grkwcvrbn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gezsrkgwn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gikqhqcih.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/gtymjfwcj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.fehbvm.com/Article/details/gquacrosg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.hesvh.cn/Article/details/garnlowmi.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gheqldqzn.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gnxmlcply.sHtML


<!-- 参考信息 -->