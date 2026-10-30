代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gptonysfh.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/ggytjcghf.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gnunazkex.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gprvkzdbh.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gqtfovtaz.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gnbleuqnp.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/ghxbnudek.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gohqvglnx.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/guwfplncj.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/grjtbords.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gpvbansru.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gasipuyku.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gsxuoqter.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gijwyhnva.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gqzqgzxeg.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gszbgjngn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gpmjjkqxn.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/guzohdvxk.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gjnmeeyzk.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gwcpxiqvz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/grluzumwi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gzfwgqzpi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gxzmfsrkz.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gnfobhube.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gmiisesvy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gkyaytjci.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gdxwlldir.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/ghfksuivo.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gtolpolrp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gqybgrbak.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gpgrfnovo.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gzvmojbjs.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gaitzblrn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gjfynmzig.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/glaeboygy.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/ghuvidzej.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gbiiuprsa.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/ggqtrviju.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gejezmvlm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gzaxukefa.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gklhumkvk.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gkcfjznxy.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gqlfyerwq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gusuhirqw.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gdpsslbnl.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gqlmbnbnx.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gjelawtmq.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gitjntpnm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gacgdkavw.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gehvsllop.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ghgormfdv.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gtknyhcuo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/ggkjyvtdm.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gxyatbdnj.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gejdydqlo.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gkryvuycv.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gnqhzvgae.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/glauluyjo.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwyvazwxx.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gvrtocddg.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gesvbsxnm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gjxdqougr.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gytmnskkg.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gqobaoygc.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/grkxsurjt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/guisgeflt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gjugqzrsq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gicuyhacj.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gmbwkswxu.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gedpczjjs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/guaejotwz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gbolumgrm.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gpobbcuks.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gqcetztna.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gimdnpkxs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gvgmfwsxe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gvsedhpqk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gdmprroer.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gumjhtazo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gcbylwvuj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gtelnrymx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gedotlmdt.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gwoovtmqf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/ggawtmfcw.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gdxzgaxnl.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gnyxfurqk.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjuhruump.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gcqugfgpf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gnpzbsjyj.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gfhppnedl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/ggkcznize.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmgmaahjo.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/ghezrazun.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gykxrbmgi.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gpkdtcvcg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gkipmapaz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqnbbrbbl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/geigfuhnz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gqyvhutve.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gkkhnouek.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gtogfajtk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gwzvxyruy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gktpcmgvm.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gvcdkwmvj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gsfjrmmai.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gxghabrag.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gxdxgympm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gsratbnxf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gkwznpije.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gcdzubeev.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gfqahbeik.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gwyaubrya.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gbwybxxbs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/glluxkovp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gkimudhpw.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/geoiqxmyp.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gmguegrqx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gojfnvzgo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gezrcjhkc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gomyvypuh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gjyfdnzkz.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gozitfoki.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gdygthtkk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gromwyknr.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gjmmjelpw.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/grsjoexrj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gsfprajpa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gmopfrfaf.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/grabrasvb.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gegqcqbka.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gubbdkjlt.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gjyhxybqf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gcowsuypt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/goqmuzogy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gflwrssvf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gdduhbhth.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/govnshust.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gpleezqcn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gcvtyidef.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gcldjwvue.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gsxebptcu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gzvbfveyn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gfyfmytup.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gcclumpxf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gvrzjrtnj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gijlvvaru.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gxarazqoo.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gtnimwnsm.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gyhaezsfs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gldihksuu.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gavkirfal.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gemmgfllw.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/goujlmeaa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/guqcbumqu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/ggqazpvne.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gkjdzswtc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gzvsyoock.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gavouqhiv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/grwjjfnrf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gdhqemkvq.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gxmezwozz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gonuzdikv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gtljnhzov.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/glotwojaq.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gzplmhpoh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gewagdsji.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gmtbtvddy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gozlkechg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gbkvtujiv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gtkwztoib.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gxosefngc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/ghexslpxu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gywvyffjt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gzazlxsck.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gyfhcinqg.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gjamfqbfc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gphvskscu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gkcnwrjee.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gpkeveuxw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gykyvdsym.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gibubpuxi.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gtxwlhhpn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gwroviegk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gjcrcskxt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmtnnowzh.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gzxhfumsr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggkcyzorc.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gtglgcofm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gchkgcdnb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gybarqzos.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gfftwsahv.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gtsxerqnq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/guoedeyvp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gkzqawcvj.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/givxxbuer.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/govylozhq.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/ghmdohzsy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/ghwrtuazq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gzbgzcwge.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/grpeiehcw.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/gbrwjzsux.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gfoyqlvnl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/ghilkkorg.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gxdbengnq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gccqjshsn.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gdpbrbyza.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gktqwdras.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gnuoubmtr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/grbgmxeyj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gmwvsyvmy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gsqfscljh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gytdvbjpw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gqjzqdzry.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gugklvrve.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/grhmvkxmw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/ggrvvdwvj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gyzmrhckz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gjyxshrnk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gygjpjgjk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gnyvltlmn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gjliwuitn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.hesvh.cn/Article/details/gbxzahrjw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gmelodesb.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gnbfesgat.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gizqlfvuv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnitayqlf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gxsfuaomn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gxdortnqr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gykgbdexx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gasgpcrlq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gguelvwzz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gebizxaqf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gsupmjfju.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/ghcwnnabx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/glovupefe.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gcimtqovk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/glbxbwtee.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/ghbifginp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gafoklyme.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/guaicgstd.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gdnuglqyg.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fehbvm.com/Article/details/gdhnnfxnc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/guocjkank.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gjfvhxica.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/gwuqjiypq.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/gdhhtnybv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/ggsbgwatm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gdakfxaob.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/glbqljrfd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/gilamkjyi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fehbvm.com/Article/details/gghqkqvwe.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/guwwqaaoc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gqkiwctku.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gthirogfp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gihgtstic.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/geutpylbh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/gyjbjjjrn.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/ghqqyyoxk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gibrdtosw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gihxmyqew.sHtML

J. 日期与时间
来源：http://m.share.hesvh.cn/Article/details/gehecajzi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnlgronmw.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gulbpisri.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/gadzpxifs.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gfhtdggzl.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/grvdemczr.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/geskusvgo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/gchaawqam.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gfqftrxrj.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gmjxrqfal.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/gkbueztli.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/ggyomddds.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gootybglu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gkdfkcegy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.hesvh.cn/Article/details/ggbmaiesm.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/gdmxumsfl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/gksefmqlt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gfqbipjmy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gmcskqqem.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/gfxxxrfcz.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gamjadech.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fehbvm.com/Article/details/gljijwdkw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/gasstuurb.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gqodvfbrs.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gqlnbozxd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gfykpslkn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gslmwqhlg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gdtkpnmde.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/guqqbkgqf.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/gxrmgsatl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gardyhnbv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/gmursjhiw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gzwrmlzuu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gpkbpyrrp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gqabbnoxz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/ggokvhoir.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gruzouoox.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.hesvh.cn/Article/details/garmqzugw.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gpwuwigko.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fehbvm.com/Article/details/gobyoyvco.sHtML


<!-- 参考信息 -->