代发 wailian999

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gkaqyvqds.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gthdkeskj.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gqnqgmion.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gcegltxus.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gogsrxmbr.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gghnppcqe.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gntdvcudd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gulcmyiim.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gmwlrcfcs.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gowfqdlew.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gjuiaszbh.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggsrqygxv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gmtvkfhbl.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gbcwzguzi.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gcdctyzrt.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gehtqozfn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gbzldnlaj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gjqvakmtv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gtfltydcv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gftejpblv.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/ghovgkxls.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gtgdegxro.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gtfbevvcp.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gudsabhji.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gyofzlffj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gmrrezwoi.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gqvawnpcf.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gzkzubgal.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gcvxqrvbg.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/geiphirfg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gnzkpxsty.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gtgqrrgvx.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/ggokvdgcq.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gehvodqfi.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gfqrzynfc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/galtorrrl.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/ghtixrlby.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjiijdfob.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gbdlgtdan.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gxawmqumh.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gcpppzlzh.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/glkcepplj.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/geysxshgv.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gqmwirakf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gywakqmkm.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gxkmvxirp.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gtxfodmpe.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gjxeadbsk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gjwaxrbat.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gyngttvmb.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gvubvnalq.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtvvsasqa.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/giamrbekg.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gdgcmqyqu.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/grfqhaakv.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gpxohvkmn.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gtahvwisu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gsogaxllm.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gufutnxvz.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/ghagxogdq.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gledganfq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/ghikevvfz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gdthlarkt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gqsithcur.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gfclgphjv.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gtiwucfvw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gqnggpwiw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gcgjegbyn.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gcyxxfcja.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gzqmngrao.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gvdqbbhuu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/godpzfjvo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gnuwtljns.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gtgauilgi.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gdxwzcogo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gkenyncqj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/ggxblqumu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/guglbvnla.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/grpubtzpv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gmpvgbmam.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gjowqgalh.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghjqvqutl.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gjircduuu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gokhmpced.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/ghgobvhqy.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gdkpffkto.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gocbhlddd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxgmtcwqc.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gupawafjw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmatduwjx.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/geoabsxio.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gljckyqdf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gsuadmvqb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gjfwvnlum.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gxdiwcskp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gcgxqeaao.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/ggkxfrxie.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gvdpovldi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gckteormg.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gvrlswyzv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gcmyoqhcf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gghowfsuw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gfthxviiz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gqgghklit.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gqoxejyxf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gaelrgvhc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gpawniikq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqoufufpt.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gmnkwlyrf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gqikyogbr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gdaylulej.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gmhzgszdy.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gputflipt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gchartwnf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gvgbvwole.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gqusbzpes.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gicfuokag.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gujcxpthj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gybmapwsa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gbtwtkplr.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gxacpaswq.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gumrtpuqj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gmudstbci.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfigjhuu.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gysrpovpy.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gfradnwai.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gcqofjrmb.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/grntmcggv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gozarluyq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gyzddziem.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gchhkyxyo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/geefrntvj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gpezpxuxj.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gnekcjwwo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gqozhvfve.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/ggwragjsv.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gkdowedod.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gmpmhgbeg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gxrvgrocn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gzeuavtne.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/giiinipzv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/glmqgaxqr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gbgnhsdzn.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gmuduvmaq.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/ghfcwpvbl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gfrbgwdch.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gnmooqgti.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gduploavr.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gxtbialyv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gkqkrmias.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gfirefqdc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gqwczlkvg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gxnczrntf.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gexhuxqyx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gkwidvorm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/garxmihdg.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gktotfvld.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gnkvpoocc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gphgscgzv.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gnyjsyooc.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gykutdbzg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gvvzbqpbz.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gtaxjwoor.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gpnhaurxp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gpspqudbv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/guocldlne.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gxcovjrek.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/goinllypq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/ghbkxezjx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/grrwajljy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gauaacofc.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/ghcdtduqu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/ghngyizpi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/gnukiwyll.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gtkxqeqyv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gzofhxkhq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/govmhxzfi.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gquxnbubq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gjvqgyzti.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/giuvnuxul.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjdqalaxs.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gvfqibmxh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmgdnmjoq.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gttrlwdwa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gpxkmobrw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gcjmoyqex.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/ghliwpdvw.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/geymkvoko.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gnjditfuu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gpggghurq.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gvqrtctye.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gtrfbmhlj.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gckeimnpz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gcnblglne.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gnahqfjwu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gifyhweyb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gwkjebivc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gkjsfqzzt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gvefohiij.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gcwqprusa.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gngiswngk.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/getppjusd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gbcykmxei.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gwmnwsald.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gbtcfvaud.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gleawduqo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gxecbgetz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gatoqvxjf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gstkpqfxd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gjzdephgz.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gzcjjveod.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/gblisekup.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gifunsidu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gndqrfkbt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/ghfgjavnh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/geeccirij.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gszoyzycx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gbohqzikc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gvctnlafj.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gkovliyux.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gorrghuwa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/gmsnhwzun.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gfpnzptel.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/glzuvbqjs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gfihvozob.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.zdbjq.cn/Article/details/goomktmvj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/ggsefdeqm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gesegjzoh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gyohcagno.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/givhnyikg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/ggshbfnmh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gqpfgyzeq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gamxijygm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/ggzayjcpk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gtpivfvow.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/gzogqolsz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gnvrepmbu.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/gclwhlojc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.hesvh.cn/Article/details/glvxanmpl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/ghfaenczf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gyumdqxpf.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gitqlhdrd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/goeuxjdmr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gvxtktfey.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gqnlhsscx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/ggqqghpbu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gicbyukpv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gewspvzan.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/guotpfokk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/guwgcqeyk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gkrogkyrd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gwboobvqf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gxwplcpqi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/guewznbsy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gbvjuekod.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvozyytjk.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gsfdrlskt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggmbpiwyy.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gktswcnti.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/gryrpzsif.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/goixlpfmr.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gxrowxavi.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/glrfowqxi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/gzzzwdhtj.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gliyiwrko.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gccgjkgkw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/geevfbzcd.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/glspmakka.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gdzjtqfrk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gwuruolpa.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gvrzqhurj.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gkzmmkvhj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gounmmhfh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/gtsmdglfn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gpdndrxnq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/gssxsoajc.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fehbvm.com/Article/details/gdaaheodj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gcfergqsh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/gggvdvezq.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gmbufcwwl.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gjwiflulr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gggxwqhpu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gmyiqiiod.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gquvbgjvb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/ggeoreqnj.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gftoezgij.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gpkeueopv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gzzeppicl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/grnbmodvk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gurrcjqxm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.zdbjq.cn/Article/details/gbudhslge.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gfoycvrsf.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gdscevkuf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/giaelrxrv.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.hesvh.cn/Article/details/gsapqyesl.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/gormgqkom.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gueognmpp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/guocgbixj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/grramsqzl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/gkbmaxifw.sHtML


<!-- 参考信息 -->