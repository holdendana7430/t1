代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gwkhpsowa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goissanpl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gtesgfbqt.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gkmhythed.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gclrflcpr.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gsjpyqczv.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/guocupuqy.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gnrbksjyb.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/goeywsvgl.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gpamaitch.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gykbzhuqa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gkuzcvbjj.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gbwvjdrjh.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gosalxzos.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/ganstzsbg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gfuqtlokv.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gmdctrjym.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gocgnnvsq.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gitzjifsf.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/grnhlgjgv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gksvgprcu.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gbqarthnl.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/grxkjqhjp.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gnvpsjqha.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gxafwsjnh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gxsbpzock.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gpvvrclbq.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/ggtgvtubj.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggftxwueq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gxquonbyy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gqihevrok.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gogkfygfw.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gaqudlklj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gzvwptdud.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gtjunzhme.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gkpubgvel.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gtfdztvwr.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gueksxnun.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gzxnyzbmi.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/ghuolfpik.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gplgiumnm.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gfyjknazh.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/guafrzbdj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/ggcjvuzae.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gxyxnfnwx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/grkerontc.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/ggnqqhrjg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gdvevwqwn.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gyjhwajcv.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gnagpldfi.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/ggjbmizry.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gvyfqrhol.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/ghfjpavci.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gokvromls.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gxjtegmgb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmxmnmyrj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gnlokhzpv.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gbvgjvdqc.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gbxeuocpq.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/galnbqfah.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gjdwiuetc.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwplsckll.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gchngbyox.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gmeeptsqu.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gfbgefowv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/grczdavsf.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gbkvnvrad.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gofgbcxkm.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/guhtjfhyn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gobugrwdz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gpklkqirh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gdmtrzhzp.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gwclxkptt.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gladmymzt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gnjelebzc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gdezwsfmd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gtmkzizas.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gfezyatvq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/geoqdcbtj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gftmafzse.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gzjapenwz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gtvraidyn.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gzdbipthj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gmdpvvdru.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gyfsfoayk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gpntiuqzt.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gdmmeqwdd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gdjutcivc.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gkapoyawc.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gvhcpkirl.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gwbiulwum.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gblxrqwfz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gctxnloob.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gttxwmrei.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gyqrsjhqr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnqaeyqha.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gryixbafv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxarwupxh.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gpcsknqgd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gtlsvzmbn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gknudlwaj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gmbwatgcb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gfqzzfdjv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/ghtfihlhd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gvcveflnc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gqcxthaoj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gcoviazpa.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gafdfcogi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gfdbmhsct.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnpbvoxxg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gcinvjrem.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ghgpuivdc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmfwkazee.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gcxdwjgsn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gulhenrxj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gbkkvcpns.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gauyubrxy.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gjsmgxovw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/grdatpwkw.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gpfndgoqh.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gqukppdpb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gazcwedhv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gmwwyhgrt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gsidufljy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gvtubibjq.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gtnssbaip.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/ggkduavph.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxuibzmnj.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gbisxuzfx.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/glmtoxuaw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gfazxpcts.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gjnqxtvlx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnfunsawy.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gpznvxham.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gbpuloawo.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gfiztyxhm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gcwntryfm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gtsetdbnq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gafcnxkaf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gihivpplq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gowupwlcw.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gioijnjhg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gtmdbkdwu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gznextfnk.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/ghlnueluj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gxfcvigpw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gnnstadlo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gljcvzibg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsrohddi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gliiuedwj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gxeofiiul.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gkjcdjxsn.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gzrtzujbv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/grpljwtsl.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gpgbikahn.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gecyheptu.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gurgtzjbb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gswgqfijs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gouxdwznp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gphquipsh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gvvtzqlhe.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gagvcylkp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gkwatsngv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gwgcztaqt.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gxxorzhva.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gcphbzqnw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gllecsacr.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gmiunvquz.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gsochreli.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gndvjcrlw.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gmccbnxpt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gconflolq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/glauxezye.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gufjcejvh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gsophubko.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gvfwmpjfy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gibpiiuhh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gwtlhfhrr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gbpmeaowm.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gwzvsewkt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gojzqzpnx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/guyfwmqsz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gslcmhyjv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gfjdxmdgs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gzkrurcje.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gllfrukgx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gyjsjoaux.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/glojcxizm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqsdaquub.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gcvrvrwfm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnageokws.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/govhlgyvz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gtiweenqk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gfenmwqkf.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gcicmvzlh.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdrpmcwvz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gfaczqydg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvczykhmd.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gugofpbon.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gkvkqhipz.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gtjozjiwm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gwxhcwadw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gcnskgkjt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gihyiyjyd.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/givxbwuno.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gbusdxkqf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gppghaswk.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gddsjsvrs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gjvfgdsnz.sHtML

[I03] 提取捕获分组
来源：http://blog.hesvh.cn/Article/details/gxzbwohyw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gnvlqdtrt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gwooviwlw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gkjxheeus.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gzpatebak.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gwdswtgaq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gyyofdehh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gehwrbhvm.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gweijgmnx.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gtbldlnhk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gntywbiwh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gvqozdywq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gtndkgaxs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gdkyayfao.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gjsekgosn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gebeaydir.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/gdqbxjtnl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gbnufjlzm.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gydrnjjot.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gcpkkpcms.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gddtqvcef.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtehsuhut.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gtshgcgsf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/gdxsazmtg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gqaagxsqy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gkquyppuq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/goqhczopl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gkzrnmspc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gxjubyhyl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gnbknxcbh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gynkmcdvv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/giftrftrt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gcxikcsxn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.hesvh.cn/Article/details/gktmdduxt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.fehbvm.com/Article/details/ghefpdjcm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gqeohuydk.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.zdbjq.cn/Article/details/gjpqviocr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gqharkvkj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gvuhtabld.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gotplhutp.sHtML

TS:   /error/gim
来源：http://blog.zdbjq.cn/Article/details/gjotmmske.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/gbvlytphf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gkdklzcvs.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gewwacprc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/gbsrxherr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/ghvcobtzp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/gfbqmtxrl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gzuhmrziy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/grtqzcpmw.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gagcmprxf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/guqviyuxx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/gmgplhmxi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gothjnzpg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gfobmziuk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsncebtbx.sHtML

J. 日期与时间
来源：http://www.share.hesvh.cn/Article/details/gevabirgu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmkqrfrph.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gjezhlurn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gidmjkxti.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gyaxhzgha.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/goflxyglj.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gfrbvtyiw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/glokwynfj.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/geabjktce.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/goqavdcnr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/gjyzikypa.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gmgqpqfcw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gjwajwbmc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gbqasejki.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/geqwjwbxh.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gqwoimyxe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/gutrmnfpk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/gdtigxgqf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gkisppxho.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/ghobnhvgm.sHtML

[J03] 字符串解析为日期
来源：http://mobile.zdbjq.cn/Article/details/gqeqlfjdz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fehbvm.com/Article/details/gwepadbqj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gfafwfjgg.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gcpffubjc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gyyomhwkt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gznsgqocs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gayofrxgu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gdnuqehxk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.hesvh.cn/Article/details/gpwekfypb.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gcnkxqzzq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fehbvm.com/Article/details/gnphxbmhg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gttieprbs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/gudoqptzm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/gsdmwxcku.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/geljpguqt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwxhwiqai.sHtML


<!-- 参考信息 -->