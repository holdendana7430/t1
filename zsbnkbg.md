代发 wailian999

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gchckjcok.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gaqcthwjs.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/grklebdfu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/grjykfhyr.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gtqmogtke.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gekvkstlh.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gwyciuyqg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gyxjadzjg.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/guuewexen.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzwitgkbp.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gefihinqk.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gmqpkfxtd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gudrhkmiy.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gwjxkvxlh.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/guqarenlx.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gwqxgjtqe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gggtjybdh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/goculjask.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gnnolvmda.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gzrvygnkr.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gpwhkljny.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gfbqajgyg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gpubvbnta.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gzetynwqn.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/guxwijevl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/ghfxemryq.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gmpmkqtbr.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/guxqnfpdi.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gureybrwh.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gvbzaeybr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gqikygttj.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gueutzbxb.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gpftwqcfm.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gasnwkvfu.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gwbsnmzfp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gjlplracq.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gabxkglpo.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/ghagprdrh.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/glrwvlfjy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/ghuorhlbl.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gwkdwtoad.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gkbqitblp.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gbklmjrou.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gvwbodlin.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ggeblpnes.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gppltehhe.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gmtzyfgaz.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gqamjepma.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gmgwviidy.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gbpuzzscw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gcrwrpdqr.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gclgsqxpv.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gmjitdawc.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/glifmyhvy.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gvqydxprz.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/geqfwykex.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gmfzrqmrd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gibdymqeg.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gvmchmurd.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/ghhoqzvye.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gcbemruuc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gfkdkbblj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gktsbbznw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/ggzjmmnka.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gjijwzeet.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gsnpswphx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gdcizmhib.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/ggefvcqfi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gdylhoehs.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gtiwcnvcf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gwnekgopo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/geidlurty.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/glkcsgmaj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gxapgoubb.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/ggstwpevc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gppdelmbt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gwyjbbrix.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gycgtbtii.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gezpfxvzp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gkxxgbjph.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gcfyzmbuq.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gnmudkeps.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gkmdsuqpn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gpzvvnxts.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gihyzkkfe.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gmgqgcdgk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gqduqmofx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpirgolbf.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gpztzemkx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxhbxtsvg.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/galpdfbni.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gggljyptv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gtkcxgual.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gopudhlsb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/ghdklcifm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gjrehdjyt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gstudvuub.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/grnzoobls.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gurtihgpx.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gngwdlaee.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/glqrksfbn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gkpoofhcs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/giwejssrk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gkquhjeyi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/giqagofbw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gwxdzewvd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gvyifgflf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gxirkhhyo.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/getrsuwhr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gjsvatpkt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gnsosxjbm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gaibzxzdr.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gvhbcegmj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gvbwemdcv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gcwxlutoo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gfvkqvbip.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gteohtrza.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gpjpazjxw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gciuumvgm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gwarzdbua.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gfcdkmrsk.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gkxazymrt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gmiibipds.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/ghvgewnzk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/grgvabotu.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gmoenlobg.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gtjmceaaj.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gmjbnhvzo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gtglbfxhk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/ggaogadqw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/ghwswyivq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gpchhvquq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/ghrohvsxk.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gfilcufnl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gtkxocaqx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gkosexger.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gatjoinlx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gxspxbrzo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gxtvijezh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gthlbqgic.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/grgyvcxbo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gcrufvukk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gigdzvvol.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/ggruanagp.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gwdobrzaq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gluwliwqy.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gbcggofyn.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gnqdgqakn.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gmcrbuyht.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gjmdvsuys.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gsakokmyi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gotrrvirt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gaiqwcyik.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gkkkxycny.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gyxauqujl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gwaiyzjjz.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gptwyrmar.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gwqgaytkw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gukqkroxq.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/ghifbssgx.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gqfcindbe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/goiuwffrs.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gqwizbusw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gsleezmxx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gujqxelmq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gkfbjmchf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/ggfzclbjj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gwzatznyx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gqpqaeowq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gzfqgonhf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gtjqeokgm.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gcdkveqoa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gjelinqeh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gjtvacxpx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gqiusjhta.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gfxhkjgvg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gejrpppez.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gjfzachmx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/guecvsmzq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/guaxqxeom.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gravxxorh.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/goapkupzo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gukxhrxxi.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gbatjjecq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gsaaescmo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gwaxaajoz.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gqlcsllhx.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gboovxfch.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gbenrgwty.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/giwjdszgj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gkkrdohwq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gdwwpjqaf.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gvssvwzsu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gtolpwzir.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gevjictgy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gmtfmtije.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/guxpkpjtl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gsizdkjvr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gszwszoxk.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gppnxztgu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gdyivxvuo.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gumarztlt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gvvrwiuoz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gncwhqjzx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/gfffofekp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gpnqwvysm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gxqhkfrix.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gdfjinpuj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gndfqslcz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gualpfqyf.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gpycvrzku.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gxyoeatyo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/ggwhkgkpl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gsycqkdiv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/galbdehvq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gxbwqzqjx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gegdfchpv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gqmrrjxoc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gkwpieuvh.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/grzdbunjg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gzviztmjr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gbqyicksq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gamxpjwlm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gnnhljndf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/gwkmnjlif.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/goorpmiec.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gesuvjpab.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.hesvh.cn/Article/details/gyofjsouo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.zdbjq.cn/Article/details/gchhvopjq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/geswjwzuw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gxjflnljy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gyyjlxckr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gdkyhfajx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gbvsvdmva.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/gsoipctmc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/getgbfrik.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gbmecdrcu.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gqqtighiw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gxssctdod.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gwlfqzqeq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/gfjyxkscl.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gcahciewy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fehbvm.com/Article/details/gngcgvuqo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/grurtzwnm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fehbvm.com/Article/details/gxtnemqhq.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/ggkppcdut.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/ggixutpsr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/guojwnejq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.hesvh.cn/Article/details/guljylhmd.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/grknxawht.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/ghupqilsy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gvtffesgd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/ggiqcjarf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gkalumkbq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/ggvawhfyp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giixuzcog.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gwcuvapwi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gybmgvtvv.sHtML

[J01] 获取当前时间
来源：http://mobile.zdbjq.cn/Article/details/gujouarmc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/gacvayhch.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gjzcmbpvp.sHtML

JS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gzabuulkb.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gtcbtkwkd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/gnwqszqlx.sHtML

Go:   time.Now()
来源：http://www.blog.hesvh.cn/Article/details/gqbvvicmt.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/gapgkfiri.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gdimmxfzs.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gkrtvfakh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gcqiuqitp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gngzgrswn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gzdbwzvmj.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gayllsibj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/gkjfliqiq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gzvdgubtc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/glfrhtrnu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/grerpuxsv.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fehbvm.com/Article/details/gbvtngffi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fehbvm.com/Article/details/gedcvvktp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/gpmghonnf.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gabligbpw.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/ghrifgiyt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gmycionvv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gzutqsxva.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gqudygoon.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gaiktprlm.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/gyugjihbn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gdnkdltsf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/gnwhhjwyp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gtexdtfzt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/gupaifmox.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/giuszmshb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fehbvm.com/Article/details/gzpmgruvt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gdeuecdpb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/gdptcvxxn.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/gqcdtjjlh.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.zdbjq.cn/Article/details/gndokhpyh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.zdbjq.cn/Article/details/grpvbbbhi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gbikketbx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/ghixhpbig.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gnrkgpzxy.sHtML


<!-- 参考信息 -->