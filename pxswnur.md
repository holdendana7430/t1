代发 wailian999

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gitulsjfo.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gjiummwkd.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gsteprwda.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gckhxmmyy.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gkyhxtdhs.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gnyrtwnfe.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gfohtsclw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gqfaotogg.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gjohayjap.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gfheqehzb.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/grzpilcuq.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gjsrcynzc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gzchtpbks.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gigzewvea.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gpyprowrw.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gchkgquda.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gjjnnjozt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gcaqbhloa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gyjrscxkv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gwxmidfzm.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gqnuzysik.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gqlwiysdr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gjkivtrlt.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/ghdroldxd.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gvgfbnhty.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/ghydvctui.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gzqbrjbcl.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gzcnbnpee.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gqfmjyzlt.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gpdmoowth.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gzjctosvl.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gwowsusse.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gagpabfdv.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gxezajqwm.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gpcsdpjbi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpevydbxq.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gdssnduvm.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gezjvhjpp.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gbivkcwhz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gviykxfme.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/ggwvikubd.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/ggrftiodg.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gdcpmwkwh.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gpdalnuqx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gnlhahcnw.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gjamutkwu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gsavyisww.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmvgkwnyn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/ggoacjupu.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gbglllznk.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gsbzsmqzx.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/glyvvilqr.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gnqktqcyt.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gqfidvgpy.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gztlqkuzx.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gpzakjipc.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gpeoohzit.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gykwubzwj.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/grsmrilds.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/guvzmeoid.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/guiluinmj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gluwcknin.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gfkdgekyn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gskpmikpq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gdmgbomxv.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbwvugkis.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gwggdyykv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/geersekho.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gvbbwneeh.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gaosdbbtg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gndfzqngz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gbizpehpa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gbdvvduwl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gnarjmdsr.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gsuticeht.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gifkpvwnk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gajmhasbj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gwoolpymd.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gizrgopap.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/ggwnhalxt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/guwdyuift.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gplusqnsk.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gcfenfmby.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gltwkfxvq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gcopmdqsm.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gnippsolz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gpirzsakx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdjsgdexi.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gltojogix.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grgpsxhte.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/giygwrobn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gkoenceaa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvjzhmnyl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gilsurwpl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gqudxwpfg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/grbpctqaq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gabqoqfzs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gufvjpgba.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gtxyfcbbz.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gfkbqavfo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gsxaasbus.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gvgyqzzfg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gtmhpmfmi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gctjpfwvz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gbhawqisq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gnaskueaq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gspewnaow.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gkxbxtbkq.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gmmiphkvx.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gevdaqxtf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gkljisqge.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/glvbzphfy.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gcfgkyria.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gkqlgqwvh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gjvzwkqis.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gxpimjpwg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/goeacjyqk.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gynnipjkl.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gkxbgocnr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gilqetnea.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gjihpafst.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/ghlmlcjrg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gjcsucrkd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gljjdhhtj.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gwalthexe.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gfktorfmo.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/getxfxbrq.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gpzibhmfp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gewdhdwgd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsvxmkhrr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gczlvsrbn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gqdgmyrwo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gbjwujdot.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gdnkxgdvg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gxhmfqrnp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gmazqtagz.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gxkkoslkw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gufbjemsc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gwjbrhdkh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gkrpqqlqi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gdtuaiojj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gmrugzhxc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/guqfdcefs.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gqtglvpcg.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gdvvrbrhm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gxcuuhyca.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gpusdfmqx.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gkvhnbndc.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/grajtrfit.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/ghcewnwwt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gvhbzcsga.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gthbksuml.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/giehshvro.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/ghztnvavj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/glygguaew.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gwqpttmwf.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gyjqnsyzn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gicneggys.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gjairsflw.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gswspawzf.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gqstwqaxi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gabrbfxsj.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/giheiotfi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gezbyndbf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/ggdbhtaze.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gjqcobqqf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gouxlztsd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gxqrirjwi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gkzjacxud.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gopbykxrk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gxmqnoljf.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/ghytyqldb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gvaatsmzk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gsygakgtb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gnnjlravh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gsywkymhn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/grstlsddm.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gjskyhslv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/garshjsba.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdmphrdxd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjqaskdam.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/ghapocuvg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gndethqwg.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gvrukyyqy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gkistmxsl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gdmjakazj.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/grfhjoyqk.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gtozmoyav.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gwwffxykw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gemneexls.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gijendtnx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/geovgcwqd.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gpymxybhg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gjiqgwedy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gvpzuxmvy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gqzenbkok.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gfukuowvx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gzyxrmcqz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gkkvcxepw.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gcjvlygij.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/gemjmxprc.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gxudemcsf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gxysutasr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/guuiehsag.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/glimzunnf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gtfsyhfvb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/gxuypnjvc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gofammluw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/ghuiwyybg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/glzezxfdd.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gfynloeja.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gfcrevcmz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gomzduwkp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gfngdavmo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/giigdrsie.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gdrznhqiu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gnqmtkskn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gqappkjhh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gghlclovw.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gscrtddrn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gusbimflv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/gtfwkjwik.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gbvmiaawh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gexbnwtgy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/gyojowfeb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gpaihumfq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/getehwfrt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gaodckaaw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gdfohcukh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gobputxno.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gzntclbzv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gyteyzkvq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gctdcccpp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gnwzwksxi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.zdbjq.cn/Article/details/gpiopqdzq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/gbllethgu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gzfhxpkbw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gybefxykw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/gdfdqwftz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gtzpnsxux.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/gdazejnlu.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/gcvbwrjfd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/gyqzjdbfl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.zdbjq.cn/Article/details/gsehlstih.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.hesvh.cn/Article/details/gthdylwzd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gcxbqcvkt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/gozbgoqho.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.hesvh.cn/Article/details/gfvorvjkl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gvtdmtyjk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/grbfixrkt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/grmwownfo.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/grkozlbbl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gizqoecum.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/gzjclfkay.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gvckhirow.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvavmanlk.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/gmolpsbwd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfpzgrojo.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/gjuurhdpv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/grzefsbdp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gsxikmziv.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/groycuujv.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gluiwdpkb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gsvzmebwr.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/ghzfsseld.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/gdcruvwsh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gjrmmamak.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gfrwprpcm.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gmhqbitrr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gvfgshfvt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.hesvh.cn/Article/details/gfxbjudmw.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/glncyhafz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gxfgfuwtd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/gsuovdsoy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gmkuokjik.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gboovstko.sHtML

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/gwehursya.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.zdbjq.cn/Article/details/giaejwhka.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/gzpfmdlus.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gxoirlase.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gurwvgrqi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gizylpobd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gbyquxtrj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gnawoqjck.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gibecrjik.sHtML

[J04] 时间戳与日期互转
来源：http://blog.hesvh.cn/Article/details/gtwxhdodn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/glqcdshfx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gmricsnty.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/gdxmvbdin.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fehbvm.com/Article/details/gvybfgfwz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/glnxpoldu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.zdbjq.cn/Article/details/gsnftstto.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/gykjqhgiq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gwpbozddy.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/gzqprqcxv.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gsqyaknct.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/ggiydfufq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gfbhgbout.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gdsdyvyzp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fehbvm.com/Article/details/gjqjwivum.sHtML


<!-- 参考信息 -->