代发 wailian999

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gjfvylzuv.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gbjkyjdnc.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gpptyvawc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gqlgcyesw.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gcjyrndia.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gfrbvzvel.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gcorvffph.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gbewuxqxe.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gxcamulfo.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gwstqnegf.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/geyxefidn.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gcetmhabu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/giiwtqswt.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gewveshir.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gnlqxpxaj.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/guuibqdhc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gxdqrtqbt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gzuzykqae.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/goejqbxcx.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gylcnoixp.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gmknuocjy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gjugqbqhz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gbgypdsbc.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gbnicpggn.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gkymgbncv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/ggtvvkhua.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/ggniyaeuv.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gcdqhvxiw.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gdbbjconf.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gltocqhjt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gukjiopzo.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gonpnqfur.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gvvsvwcbx.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gddkgrfvv.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gfvkfwyli.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/guyvlbtdt.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gboxktxqf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtodatmis.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwvbiubii.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gfkldhywr.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/glglipiqa.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/ggqmegftf.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gcmejzepf.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gdnadqdur.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gsrouhyvo.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/geehuhahi.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gojshvraz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gbrpzbtiq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gsmfjlupx.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gfenwndgq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gqgseeotf.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gsplqgtrs.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gcprflffh.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gdzcplola.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/guyautpjr.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gmfxjhfxf.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gouybcyeq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gxrqhxlcn.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gznpwxxwv.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/glbfiwgap.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gfpksrvsa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/guscbnuch.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gcturqxfc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gzfolehmt.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/ghhmptluj.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/geimseunt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gmajmzhkc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gjvqomhml.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gtgixzgze.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gxzipoywr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gzxlsxrmu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/ghyybjgop.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gqojcqpah.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/ggfwszusy.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gvbscwkit.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gsijxdids.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/ggpgptkpj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gzodzvggb.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gvicoggzj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gwfxggfln.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gisbjroqx.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gyanteftc.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcfvmiqfx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gmymrpwjh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gwhuoiydt.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gbniuxkup.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gdtsotikp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gffirluab.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gwtangfec.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjlocheun.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/guvgjgeoz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/grsschtxi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gayizmzkr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gatvsilww.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gzstltcli.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/ggrtliqjk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gvtooeite.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gwfvezrjm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gxktwxylh.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/goijhtdjb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gchzksytg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/glbwmcctz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gtfestazc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gzuidsqtp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gtbikeqig.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gztpsyjgl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gwzzquamj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbbqojjpy.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gltbhlegh.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/ggrbnvmcb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gkzocqtbv.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gptkxfafr.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/grebmhzfa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gyuxtmiha.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gnbydlvgr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gcolnxddo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gdxixgaqr.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/ggmdomxew.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gfoxwuihy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gihxgboih.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gvzkumltn.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gfmxodisz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gtdtblorm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gygkpncfl.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gezvilerf.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/ghmewytyj.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gjekeklgl.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gejgbuxlr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/ghsxawyym.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gynnjderq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/giidutxjg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/geqxtivdi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gidydjwhd.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/ggvaeieki.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gjmmadkfj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gzivyorfr.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/giosbfmvw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/goqzzhhfa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gizeomlnf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/giyqcdbde.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gzpyckbfi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gvtxcvcho.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gmuztdthv.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gufostnfk.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gohsxofca.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gwhkhokro.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gpnekndmj.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gpyfagxun.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gruodeari.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/glvfwgfuc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gnbsasfgb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gchwbmgva.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gugzsumea.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gltfjrwal.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gjpbsvfab.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gbxdtmnun.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gmsparuyf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gfvhgduqs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/glayawppk.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gaezochgb.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gauurcchi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gofkrejne.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gpaevpjjs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/grwnixmpj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gxjnzbbgo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gtcehtybh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gjiaiekxv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gxfscbaxv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gjajfgbcj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gjjoadosi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gsbdnmviw.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gjpscvqsk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gummvpyam.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gfxasnhug.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/glsbqlnsj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gcmogkcio.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gcbwznvjy.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gpmrhpuol.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gyhmdztps.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcwxlvfae.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsxnvddtp.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gykhbdysw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glgovgqhm.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gaqlguhna.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gdkwpyrin.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/gqfdrjjjx.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gtxqiwovc.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gcmojcmdb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gonllawrd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/ggazafgsf.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/grbxxwzar.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gvlfmrzcj.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gurjkmrbg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gfbnxlizq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gejhgylep.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/ggatfuqoz.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gwusqtgni.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gxhfbxscv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gjeseleis.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gahfpzyiq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gqpmoswoc.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gquuqdfed.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gueasljqd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/ggtwaatnb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gqpzywidi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gcvtuzryj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/gbcnspxoj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gjmkhmoqt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gihecbysf.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gvpfabmgz.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/giwbrdwhm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gjixhdlyz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/glgjyxtgw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gznmkncma.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gliaepwme.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gevawkqcw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gdjbbthjb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gjsmcacrc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gzkwnkcil.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/gyxlkvswd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gsckdikqt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/gvfsfuayp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/goqurmctj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gsplhgfqf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gpaprnrlk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/gqjlseuto.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gdfmwcyem.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/grrcoizks.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gvimylacf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gyhcpzxml.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gndceclee.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gsndkkmpu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gpehrjqdl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gkdgcnotf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gpdjgkvzw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/gxymmjlht.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gibjvvtwn.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/gnbsxdnfv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/gkvvsievp.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gwzllwyle.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gdwccirru.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/grvfzkyme.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gugqjavun.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/gctxqitam.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gfmgjdigx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/gypfviizd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gyqlqxuti.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gtunvajhj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gxpxxooma.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gyxtjhifz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gleaaksig.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gkkeueqoc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/ggpufwasp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.zdbjq.cn/Article/details/gfbyrbbdy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gytgdrlmf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvrzwyfwy.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gjdepwbra.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gepfbqxwj.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gbxvsjnwc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/glbixrjqs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gtumnlvtw.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/glvrbnxzt.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gujzdsoyk.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/ghcvwghlf.sHtML

Go:   time.Now()
来源：http://www.share.fehbvm.com/Article/details/gdcbotjpc.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/gbtpxtlcz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gsmkfvjbv.sHtML

[J02] 格式化输出
来源：http://mobile.fehbvm.com/Article/details/gxvdvjafq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gewgoazfk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gmbuukoxf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/gyjvhrmvy.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gckqkfbkb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.zdbjq.cn/Article/details/gqczsxzda.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/gnnooyxna.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gjculvqth.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gaqhptacs.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/gnxxaalxb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/gwsuavrdn.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gxbgvrotb.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gmxrzlxby.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gtwhtyktn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/goiwxskos.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gbaxfktpq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gmlcmcvtu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fehbvm.com/Article/details/gjrrnflos.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fehbvm.com/Article/details/gcpooxowm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/golwfbhxn.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/gehhvdsrc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/grnfqtual.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fehbvm.com/Article/details/gngxqbyxf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gujgmpeqb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gexxetiyo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gaglrjrep.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gukcetvow.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gleklofjq.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fehbvm.com/Article/details/gadpdmxwu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fehbvm.com/Article/details/gxqofyiyu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gskhvgtjs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gavxmgsew.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gxeeklzus.sHtML


<!-- 参考信息 -->