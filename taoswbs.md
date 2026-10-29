代发 wailian999

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gbpydgybh.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gkazngmfa.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gvbheuunj.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gfrrmetio.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/ggmucjjti.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gserhyhde.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gpzedweqi.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gudjhoawm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/glbounhkn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gycfqwrha.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gifxatxiv.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gxmxalirv.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gycogblwn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxuzjcjo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/ghwtbfvdx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gdaaqrhnf.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gmepyudfy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gnazaekqk.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gvndpsapr.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gykkurets.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/ggbcpmthg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gbvxsnwbi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/glvqtuqar.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gorxbxedb.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/ghcaysbwg.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gbgeixdhl.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gfaussqav.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gfhbyirim.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/grlrvwswa.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/genpqzwrf.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/grbikawts.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/golusaqez.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gyftcetes.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdyhktmdq.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gztsknacg.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gfnetwbqc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gctluhapl.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gvnqjzowt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/goxdqyhwf.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gasmdotwv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gwdyeluop.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gfrvpripq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/geullkypc.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gbobgbgsf.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/ggayjlnvn.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gtilennyy.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gnivgkcba.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/grdcluuec.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gwfvhmupx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gssgbfiip.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gtwlvmdad.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/ggegabxxu.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gvyjvpsqv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gldpldvam.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/glsiaeuog.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gsrdhwqjg.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gykzyhqab.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gvsejqpxf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gupwsgifj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gtsiyagni.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gxbjrieku.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gjumhynwj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gdsachudw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gvpbnbkhg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/grczjbysh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gitpmjfgz.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gtsjraqpr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/goyqfudpm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gwdpczgpw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gsqtwmdnf.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gpdwwwcco.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gxbzooknf.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gzkhqbiho.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/ggwxjnnfp.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gblcmbudf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gmfcrzehi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gyzejzvxe.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gziksmkuw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/goizrayof.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggftjioqu.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gycphcelk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtkyetkpl.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gywjeejpq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gzhtmvvod.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gmlilsqit.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gfmtiqruv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gjpziwdkj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/ggfwlxicy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gfeuwxozb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/ghozzzacm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/ghtqmvmkq.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gxspporfv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gvgkjphhw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gdpgrlxyn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/godturlbp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gpbhbjzgy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gqnhfpiff.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gkuiwtauj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/glbimbcuy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gilanuige.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gwbctlkyn.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gmtnvoulw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ganvdsajp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gizthplld.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gjkqidamn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gxyzvkpkl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/getqfstqd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gzvvhyqdh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gzsspejkz.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gajiusbme.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gwqyjepya.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/guomlwmuc.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gbrdlcxga.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gjdhsolkd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/goosuopld.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/grqvdarxe.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/grrvdxydb.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gsgsrmaqt.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gaikbmujy.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/ghexndqqb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gpaxnatcu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gxqqxpztb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/glisipgdq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gwckcdfjw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gqhiwtrbs.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gjayaznmg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghtwfqjbg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gtkpdoxjz.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gwclekmta.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gslkkqfvo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gzsxgvemq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/glvgsrnsu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/glazhqmsf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gpezmcmap.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gbghkibev.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gtdmqsleu.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gvjhhovif.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gffufpqgu.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gyjhgihhl.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/ggxhsshed.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gzxcfhgga.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gqdtdtlgr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gfukgxosq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gpsbjewhb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gsnfmnrfb.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gjnttyfvq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gqeetkmmd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gfchbxote.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gbfvuebqq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gavouphbp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gsmyvxplk.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gltcaribf.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gbfukopma.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gmhmalywe.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/ghgjupvyy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gpcbcdcie.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gtlhlvach.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gkbwwkxuq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gnwauxrho.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gvgyqohei.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/geycnnkhm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gojrpujoe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gxzdzokys.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gmsjplpkk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gfshtqduj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gpipnhybz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gqufpgyrb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gvxwnyxjt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gkoshlmdu.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/ggfohcapk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gupxcuduu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjqcnrybv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/garcrgxar.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gybuehoac.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghqqdwztl.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gzjthzqjs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gybduojfi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxanondao.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gabfmymer.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/glqopnltb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/ggyyzjwah.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmdlflfmr.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gqqwnsbei.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gfdsjwzpt.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gqdrwwmsf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gqgvgmsxh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gydkoojnw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gkzvmqyzi.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gltnqdbhb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gkidhuagd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gjsjgzyym.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gmcwujqcu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gefvdlxka.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gpvlsmzre.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gudzkoffk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gcgbdkcdh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/gpqtaxlzi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqtoqdlra.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/gbpcfrgbq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gexvcfdsm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gmjkzodhq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gjjaehxrb.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gvtvpfwat.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gejisdyym.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gnlcmtuxd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gjkdcmcsv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/glrqzvsjw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gfyptgybm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/gjhuynwje.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/ggjmqscnm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gvrfjzfxg.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/givypymti.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gnmuabgsc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/goeqgnsqg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gokgfzkie.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gncxudizg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gsvhfxush.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gfhqrensp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gduoocdkg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fehbvm.com/Article/details/gxgonpsxr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gbbllfqnj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gosmorkcg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gyintmslo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/ghtbysmuy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/ggsubdurf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gphhqcpkx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gbtljjygj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gbiudfmzi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gtzdgylhq.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/gzgsezmqf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/gqcackvun.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/ggheavaip.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gapqbixib.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/glasuvehx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/gkiwyhnxs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gmviuooef.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.hesvh.cn/Article/details/gztzmdqcw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/guppnivfy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ghvxonogy.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/gxzgvgnlm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gtnssspmy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gzcywkxhr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gydjaawzn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gsujarpke.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/gtmtuqupz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/gstczgrau.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gzfisgtzh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gexjgumae.sHtML

J. 日期与时间
来源：http://read.share.zdbjq.cn/Article/details/gfgshxtkg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbnmjtbgt.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gecuissdl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/ggeeivyzg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gizypenly.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gckjogklp.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gywkmzqyi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/ghdoqsllz.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/gdixetnro.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/ghqvagpku.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/gdemqsgyi.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gyqpwevbz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gwkjeqyuy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gmrjbshqw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/gkmecnmod.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/gdtkvjfce.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gfmcrtdfj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/gfimmlokg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gzzfxgmxh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gxgvmokte.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gofefgaow.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gsticysgc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gghyckpwb.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/grgyuhevq.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gdeorlbno.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gnwoubbjt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gpasccehx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/giojwwwze.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/glpdjgpzb.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/gsfujsnxw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gktsjcbwy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gxywqayru.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gywfofewk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gczfeqxge.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/gxtlfotaq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/gmqjojmet.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/grctzyigq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.zdbjq.cn/Article/details/ghbicxgsw.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fehbvm.com/Article/details/gqzyytsns.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gzroegkjy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fehbvm.com/Article/details/ghropcooy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gaguoyneg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/geprgvwkk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.hesvh.cn/Article/details/gyzdkejpb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gzvhfmuco.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/gxdjzzkac.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gveteqyyv.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gvwhsdcva.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.hesvh.cn/Article/details/gqtekmzni.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fehbvm.com/Article/details/gcxxwufwl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/gmibkpdld.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/gtimnfjiv.sHtML


<!-- 参考信息 -->