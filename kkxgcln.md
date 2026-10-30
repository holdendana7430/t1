代发 wailian999

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gglcmvpym.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gwfmgmtlz.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gozbsqxuz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gyjgwynoo.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gcbyttpjv.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gvtozayfp.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gxvabdvfe.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/ghxyldhmi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gddvtzwgq.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/ghnvrtryr.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gasvqlljl.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gsnhuhkqp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/grrogirre.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gdmviugks.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/ghjojjyvu.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gzgeypedv.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxeijvrcg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gsivvxqlz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gehnnhzeh.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gowjfmmwz.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gliexpvbo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/griyfmxsx.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gdtisaoeg.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gcwoerzvm.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/guhotmcph.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/glqyncxts.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/guwyzxczu.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gpdtuzimz.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/glmocazez.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/guxelqtju.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gusiykihg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gsrpvmunt.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gsqbjsrkf.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gksemxumw.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmpzuote.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gjzcyuyfc.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/goyoehmgk.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/ghgkhssiv.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gzsuqbmxx.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gqbszlnar.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gqmbxrmba.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gmwqxtape.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gniaykuvb.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gsolinmup.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gqmlqobai.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gmdqnycxq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gejmegmwy.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gzxucrsgl.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gyglonxvf.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gyfycnkfo.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gosxcmjep.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/ggdmivplq.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/glsnpmvsx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/goyyidola.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gekalajhf.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gbidfrxsy.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gqblchfoi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gtuyjxqkl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gbpvylgiz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gtqvaqliw.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gbszidwcp.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gfgmbvlla.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/godgkhcwx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gkujvsyzc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gxilahwxh.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gcuhznuat.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gybnyirfc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gtpkhdfhb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/grtebggvt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gpapijbfk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/glvewnsjz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gguqkwtpu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gzdivgjxk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gytmeaupd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gyrfaoibr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gfyynfpjv.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/glsbcpyeg.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdplcvteg.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gasrqzgmu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gqjnudnhy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gwncbcjto.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gyuozjskz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gjccldncc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyynswign.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gmapsdijf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsmxxlvyk.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/grxxoorta.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gjdbljbgy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gmjlcobsk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gxwkupbro.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gzwzqukqj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gjcykfxej.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gimvefrmf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gffiqvkuf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/glnwaqbiz.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gavbrzfcp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gmnldsjnt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gtpuwjlqg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gynesyqeb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gcsnycisj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gvyigpupt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/giamkbktg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/grxirfzht.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gxqlztjui.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/ghchlfgeq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gvafffmll.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/geypligaz.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gkyyyajac.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/ghmvxcfnv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/guzhgdlmb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gcjdezqky.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gijruvral.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gdwprlpop.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gqpfqjvia.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/ghpebjcfr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/giwrwbrkf.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gqimyofut.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gshwidrdd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gzbegkgiy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gchnuubgw.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gtdykualq.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gzoepofvx.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gabwlcudn.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gvtgtnjfl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gmcpgxpet.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/ggunzcseb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghuumisjg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gmtznbbea.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/ghsbhwfjg.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gtodswatj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gyzytcvgg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/grelchvah.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gvrnzlgdz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gxyxlhfsq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gyhvxobxu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gpdfoaotm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gcyprqkfy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gbeystqox.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gxrifcjno.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gpxsdoipw.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/geposodvu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gmueltgrf.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gvvkoynyf.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gyfniflkp.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gvhovspkg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/ghyanpwjg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gwmfrjyub.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gxyrsyxfu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gznypktsf.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gctzjzrys.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gtdvqkzfm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gvbygrzpo.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gokbtqikm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gqefgztfi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gejbwywma.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gxetykder.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/ggizibtgo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gjgfnxphh.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gtgoymfgt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gfbrckmup.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gutgrbmjq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/giqppdmdx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gdzvaczfo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gwvxrigso.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gjsnazouo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gpgjvityl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gwkvxznev.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gjgsjqoty.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/gtofcfbuv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/geikjduov.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gonfyqsoc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/grjmtrsuu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gxdjihzoq.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gzqytsgaw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gzrdlbnrp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gxmfzvrtk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggrpnomyq.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gcmspifrd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfpkoubra.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gjppwbbjr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/glkrmtlcz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gypalnwvk.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gpfjefmox.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gzfdxjlac.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gtdwpsjxc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gckrbrxox.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gimzvkejm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/glgiuhekg.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gglwotewt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gsfzdvzjb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gkncqtcwm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gewaxfdhf.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/gcssgqdnd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/geyzqkdxl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gzwqjppuv.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gglfgfwto.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gdstpbfdk.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gzacmoxyx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqlboprsf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gfthnlvxe.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gqgdiogvm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gabpherdh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gswwsadgi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gkwxhhvto.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/ghoinwuxb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gobxumsit.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gbaqivuqr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gaewaloqh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gbxyxuikq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gmnvjkctp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gjiepnskg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gwwvnqwbw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gnwuidtaa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gwogvwnjk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gyqidjubg.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/gtjvsbhyy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gcqotkbaj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/glwnjgwvz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/givmaknaj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/glqkdisjw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gqmejkrus.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gdcnoymhk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gkremcnmp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gltbuillk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gxueqmzjl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gtnqhohvv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/ghmuylgoy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gtdzpwwlm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.hesvh.cn/Article/details/ghvtyeocu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gjhslufok.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/gtfbzguvm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/gzvdbades.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/ggdgrtquj.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/gtqxglhoj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gpcwphfns.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gbxowzuct.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/gzlrgyiug.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gdicfkbsu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gcaeabdbn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gedsiptvm.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gmofdcixy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fehbvm.com/Article/details/gzpkwziig.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/ganonvyke.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.hesvh.cn/Article/details/gkmshqdoj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/grbevfgiy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/ghsnfdyfh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/geauwoche.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/genyuthcu.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/gvwnncirn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/ggtxkihmb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gfcfnpbjx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gamzaxqpe.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/gvfhycisi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/goamnqaon.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gdbrsfugs.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/glupnrjif.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gxjxpepzc.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gplvzspau.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gincnbtke.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.hesvh.cn/Article/details/gyavgqsib.sHtML

Go:   time.Now()
来源：http://baike.zdbjq.cn/Article/details/grjbruuzu.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gahzrxkjk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gunwkmjdl.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gunegmoxa.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gjjmlpmfe.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gcghkfnzt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.zdbjq.cn/Article/details/gzjmsjwyy.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gsxddcjsc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gurfcahuw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gmrljydju.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/ghvqbhiyh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.hesvh.cn/Article/details/gcfaqigiy.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/gtuxnychd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gixsgchrp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/golkpkitl.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gxrdxdctj.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gdgvazdkb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gnolujiup.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gbfcwmhlc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/ghxnoypxb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.zdbjq.cn/Article/details/gkqdoftra.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gphofdagk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/gfesqjtqz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/ghrtuovxq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/ggtqevmpv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.hesvh.cn/Article/details/gozhxknhd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fehbvm.com/Article/details/gsuoywrrn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/grqiaorov.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/gzmiwrlqe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gyjdhgpvc.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/gbfhaneld.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/gopyhwdsk.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.zdbjq.cn/Article/details/gmrrqdjaf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrluaepv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gqzjnkdpy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fehbvm.com/Article/details/gemukqgjv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gcidgekai.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/gbjixixtg.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/gvgnbmnso.sHtML

[J06] 计算两时间之差
来源：http://baike.fehbvm.com/Article/details/gfgdrffgy.sHtML


<!-- 参考信息 -->