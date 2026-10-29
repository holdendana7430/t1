代发 wailian999

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gotmfskhi.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gfuzqrkph.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/genefvpuc.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gvlbzqesy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gyugjnmdl.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gurejrzpo.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gxtuxfdfe.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gmcuikpow.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gpewympvm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/grlvkiqhd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gpgvobgsg.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gajbrugbh.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gsicywgmv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gytijmykq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gsluytnir.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gkjnytynw.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gfvunnotb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gkplkpqdn.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gujydhsvj.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/grmhwnvsk.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/ghqladrlw.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gpddlrnbx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gmvtfyvje.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gqdcpdhcx.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/ghyahjvdc.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gnxewdegg.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gxojfaoaa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gtouazwii.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gzqjuertr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gjxmmumld.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gtnncotsn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gpedcdfff.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gjgjlhsge.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gnygclmss.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gimehnmbh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gadufcazc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gxqcorbzr.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/ggfvirhea.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gdljiwnas.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/goggszmdk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gsorrjuyt.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/ghvphfzko.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gviplnvmn.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gaqglpvwq.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gdcgkodov.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gyjwnioja.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/goxkjiiwx.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gmtpxyaqx.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gdxwpptdx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/ghphzepki.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/ghaxifwiw.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gtezohdca.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gxxdpyxqc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/ghsmnaeow.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gmslwgnkb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gigkqatve.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gehintkcj.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmhtqvwxv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gswmgzmms.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gofbwkmcx.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gqyrbfnmg.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gpbsihaia.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gsfvvcgkm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/geiuaadmo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gqfbtzqvh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/ggbenncsx.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gruuqfvgy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gdosrlvfa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gomobemgd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gwcggaojh.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/glcxdeupz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gzxohybgy.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/ggfizwbyz.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gaxmqkqvj.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gknakqaxa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gicdconln.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gjvbrwfrc.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gtzliodhz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gipbsulrc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdsgbsrka.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gifibjlkr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmqushkbg.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gidoegxfd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/grvgdahhf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/ghwyrldym.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gunsjmbpe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gqdwjelnh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gsorulgfi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gnedotkrs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gdlcovxmh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gfevthhbd.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/ggmpntigv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/ggcsllces.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gaovoaojd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glanrssuz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdocuvpon.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gvjgvgttd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/goohrjqbg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gesegkxaf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjabtwzjd.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gcfxgspip.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/grwwqilqf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gzddbpvbb.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gbuqextvl.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gsyqiafjj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gngctflfh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gwnyokeyq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/ggchbxpnp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gfomxaouf.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gvtjrlfuz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gmjkwlnwt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gvzjgsyup.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/geeqndydk.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gzscayybm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gvgfqsifb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gmysrnrms.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gbjcaalgw.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gmkxscwnj.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gjxltpdsy.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gofuhddqw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gvubkhvvq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/ghxhnphzc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gemwlhsyz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gbbsimpge.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gjezvdlbi.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gxknbelol.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gamexxmvx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gzgaffszv.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gxinxgidq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/grrnaqtpu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gswddhavh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gbihterzl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/garuutuww.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gsrbrhevd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/geqojcyic.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gumzefsoi.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gwjxhlcco.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gsyeyqxro.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gpcvcthro.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/grecndkce.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gxlvkwntj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gnililmen.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gglmnrpmk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gnjvztqli.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gzsdjpjmn.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gnfonmqym.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gfyhtrchw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gggoezzwp.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gzyzhszol.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gnbfiijlx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/glrxvzucy.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/glypzxnzt.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gmlklonhf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gnhxfymtc.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gjeobawph.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gunrbtgmn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gsangzsfy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/ggazgobkj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gkutoprtx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gynoekqfi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gjxgpznhf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gidtkohcf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/grcxcequx.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gacuxylra.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gfvgzmvwq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gmnfhntym.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/goetqrpad.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gnptsqxiw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/godhzcsci.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/ggyphclnm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gwmeojltk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gcqcmtiut.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gohgeebjs.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gmcriauwi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnzsxdzic.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/grunjfmdl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gwqcttgtu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/gbqqocbyx.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gijouiynd.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gjqmcoqke.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/ghvqnzhpu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/ghxdxkucm.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gdinweiss.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gedttzusc.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gmwzzgcau.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/grqitwchx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gtempclpi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gxxjfrkss.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gwhmvursp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gneoyxwsa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gcakldiyn.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/geckfzlnq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gfahmvcpg.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gptiogeiy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/ganswzpvq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gndowyvwn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gzojfdgka.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gidrxhvkk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gicwnmolq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gygotvwhl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gkfdbaxyw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gmlxzazdx.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gcftveqky.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/guistndfr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/guygrcepa.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gvohjvbtl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gfzdmeczr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gcakmknpb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gmcrwkzpk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gxvtmgexc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gvxapwmvs.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gvknpkkjg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/grzixmwas.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gozgwiblw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gsbgbatqg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/ggghtesrw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gjuxdxvga.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gyytrlope.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gpzfgmmcb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gymuybbrs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gevwjnohp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gokdsfxyn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/ggzvlasxa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gsocoauwe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gzcpsooae.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gqqtnndvu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/gwbsrlrwl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/gwwirnzfr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gxdamehge.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gdtykmrbd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/ghdsifrwv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gbjwktqdm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/gskyesugf.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/guaonbcwv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/gekwthgbb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gnieivpun.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.zdbjq.cn/Article/details/gydvzxywl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.zdbjq.cn/Article/details/gqjixkuyn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gkigjmvzw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/genmejffr.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/ggeksgysm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gazmtatnw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gngvzdnxg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gpmspkwjq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/gzworrken.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fehbvm.com/Article/details/gnnrgrava.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gbvlijxrv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtrptnfxe.sHtML

J. 日期与时间
来源：http://mobile.fehbvm.com/Article/details/gutmmqteb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkxokitqi.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gfxzyrkhl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gyrqeuuas.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gzcprxnrq.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gowhhuwvh.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gmrsjcxiy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/gciwyluxm.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/gbhvhimst.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gfalenvrx.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gyzlspjzx.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gyeybysor.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gzcyxwrmd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/groxkbqhx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/goihwfaqz.sHtML

TS:   d.toISOString()
来源：http://wap.fehbvm.com/Article/details/gcbutjpsj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gosczwyrn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gqosyqvjh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gyqvupvyp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/gqhrmiryk.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/goxbiajpy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gnqyeqkoq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gljnzyrru.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gwaebykuh.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gifxdjiko.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gemvoiblh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gnpfoboom.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gashpsvaf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gygdxnuol.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gmtvrkvmg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.hesvh.cn/Article/details/gejcotevh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gvzdmqztp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/grboduuri.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gkpandslk.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gqqjnttty.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.hesvh.cn/Article/details/gopfmmhbz.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.hesvh.cn/Article/details/gxhrjinxg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/ghwpvscdr.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.zdbjq.cn/Article/details/gkyvhjeiq.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/ggqkwicff.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/gkgwacnzi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gdkjyptqw.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gbtjemylu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gvbarubuj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/ghwdsncol.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gwnwmigth.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gkhawdgew.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/gqywckwlo.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/ggkypjkkz.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gabhidcru.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.hesvh.cn/Article/details/gzefevkwr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.hesvh.cn/Article/details/gelawzauq.sHtML


<!-- 参考信息 -->