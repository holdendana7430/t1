代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqwxvhvx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflwwsztg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmxhjffj.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbdygkjz.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtkllwsk.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdyokilu.sHtML

Py:   super().greet()
来源：http://blog.fanxiaobao.xyz/Article/details/gjriumicj.sHtML

PHP:  parent::greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gbjgfycne.sHtML

JS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gackbqocg.sHtML

TS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gslticuls.sHtML

Java: super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gyfnglzav.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fanxiaobao.xyz/Article/details/gdjatyabm.sHtML

Ruby: super
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgesmsjw.sHtML

C#:   base.Greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfcnmegu.sHtML

[G08] 静态方法与属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcqxfato.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqmsfgij.sHtML

PHP:  public static function f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gedrgcfkt.sHtML

JS:   static f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gauscigjl.sHtML

TS:   static f(): void {}
来源：http://3g.fanxiaobao.xyz/Article/details/ggnascplh.sHtML

Java: static void f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdravbajn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fanxiaobao.xyz/Article/details/gqdwmudlr.sHtML

Ruby: def self.f; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gedptthfw.sHtML

C#:   public static void F() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbojaxrub.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fanxiaobao.xyz/Article/details/gqliqmocb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbmbbdim.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gugniaini.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fanxiaobao.xyz/Article/details/gihpdhzyx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbocleko.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/geamorqki.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtvxtpjk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdhagrpd.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjmyezamg.sHtML

[G10] 访问控制
来源：http://baike.fanxiaobao.xyz/Article/details/gvwtkuons.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvzfovxo.sHtML

PHP:  public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gktoyhqpw.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fanxiaobao.xyz/Article/details/ggyqwyizu.sHtML

TS:   public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gdvnobfqr.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbcxvsiq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyemwooa.sHtML

Ruby: public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/ggexncdyj.sHtML

C#:   public / protected / private / internal
来源：http://3g.fanxiaobao.xyz/Article/details/glyzqklxr.sHtML

[G11] getter / setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcmyoplm.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fanxiaobao.xyz/Article/details/gcazhykvz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtkisnath.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcpedhsr.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfpwqkii.sHtML

Java: public String getName() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/glgwzuswt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gjtrrbaps.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdcsyokq.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvatrcrv.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptuljual.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiniykyq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfiuhdqxv.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrqpgzig.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvwzekquh.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxeskndyn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnknmrin.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gxocyeqvl.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkbdachw.sHtML

[G13] 判断对象类型
来源：http://3g.fanxiaobao.xyz/Article/details/gyjxayyyg.sHtML

Py:   isinstance(u, User)
来源：http://wap.fanxiaobao.xyz/Article/details/ggcsewzwf.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjckkrxc.sHtML

JS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gmgdxjhkg.sHtML

TS:   u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhzvdqiz.sHtML

Java: u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gdxdmjipf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gkojynvno.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fanxiaobao.xyz/Article/details/gtxzuhiic.sHtML

C#:   u is User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjmqnurz.sHtML

[G14] 数据类 / record
来源：http://mobile.fanxiaobao.xyz/Article/details/gjemtnfuu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fanxiaobao.xyz/Article/details/gztxovcyx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fanxiaobao.xyz/Article/details/gjcdcinbe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlgxcdjq.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fanxiaobao.xyz/Article/details/grbwagouy.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gyaagoljd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fanxiaobao.xyz/Article/details/gamfptzht.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxtgbfyk.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrnginyb.sHtML

[G15] 枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyykqqtrk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvegzaclr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gojtkfycb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fanxiaobao.xyz/Article/details/gsodghkei.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gfbbbowmt.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitleperr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fanxiaobao.xyz/Article/details/gcebfuwxp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fanxiaobao.xyz/Article/details/gcegxzrzq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbnopblz.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fanxiaobao.xyz/Article/details/goxbxgzcy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fanxiaobao.xyz/Article/details/gkiqtkuju.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fanxiaobao.xyz/Article/details/gicrxehix.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guavxrhjj.sHtML

TS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gjipytsyc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbevvytsk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fanxiaobao.xyz/Article/details/gqwyvglur.sHtML

Ruby: obj.instance_variables
来源：http://wap.fanxiaobao.xyz/Article/details/gwfuhpivi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaihztmvr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoveqzya.sHtML

H. 异常与错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlsimsvh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyivlywf.sHtML

[H01] try / catch 基础
来源：http://3g.fanxiaobao.xyz/Article/details/gkueaqlnd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gmhvclqni.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkwiwswg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzpcrnbl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmoteeze.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrynjrbi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fanxiaobao.xyz/Article/details/gxjceppid.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gismgneil.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fanxiaobao.xyz/Article/details/golibbbgm.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstsasulo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fanxiaobao.xyz/Article/details/gocjxjpew.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwnynlfq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumdirwsp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiwgrddq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/glvardycv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fanxiaobao.xyz/Article/details/gddezqyvc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fanxiaobao.xyz/Article/details/grgxjecsd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/ggacujrjc.sHtML

[H03] 主动抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gbagjfrdk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goctlllsy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvxocbfr.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gucomtgxo.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxkvmxuy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapjvjtmr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fanxiaobao.xyz/Article/details/gztfxnxbg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fanxiaobao.xyz/Article/details/glgcfbdeh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdbaudgx.sHtML

[H04] 自定义异常类型
来源：http://3g.fanxiaobao.xyz/Article/details/gaihpkjpy.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fanxiaobao.xyz/Article/details/gpnkeavhr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/godkxishs.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyjwoycd.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnojohpvv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjpsxhjl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fanxiaobao.xyz/Article/details/gogxdytsc.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gqytfpgzb.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fanxiaobao.xyz/Article/details/giredzwzt.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpzkrrhw.sHtML

Py:   except ValueError as e:
来源：http://www.share.fanxiaobao.xyz/Article/details/ggykxckcw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fanxiaobao.xyz/Article/details/gzitrovgd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoiiokvt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjaqriwwc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvsiidkz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fanxiaobao.xyz/Article/details/galjjltzz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzorjuulk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhdtqqfz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fanxiaobao.xyz/Article/details/gocaobytc.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fanxiaobao.xyz/Article/details/gzblgpxon.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhvwcycv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gmljnfszo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqlfcxap.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fanxiaobao.xyz/Article/details/gvqaladrs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fanxiaobao.xyz/Article/details/gpllmpvka.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfnbqtvn.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjevhefx.sHtML

[H07] 断言
来源：http://wap.fanxiaobao.xyz/Article/details/gmznmjbmr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fanxiaobao.xyz/Article/details/gowbnrohs.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcbesqqe.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gzrnmstdk.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdinvdvzr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvoocfeo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fanxiaobao.xyz/Article/details/gfpskcpnr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fanxiaobao.xyz/Article/details/gzznckfzh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gsfumvsqb.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fanxiaobao.xyz/Article/details/gtpchekjt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgwotszd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjctlovg.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqcmbfvq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmwodmkt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fanxiaobao.xyz/Article/details/gczxqlbwa.sHtML

Go:   err.Error()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkfqurya.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtaauqxd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fanxiaobao.xyz/Article/details/gkelnwdwh.sHtML

[H09] 带错误码的异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnorkrkl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fanxiaobao.xyz/Article/details/gxhxhhgbo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/gxslpslaz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goonovgcw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gywicefnp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwgsrhjky.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gslvufcag.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fanxiaobao.xyz/Article/details/gimmrzbkv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqathqwfb.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goefbhfcl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvzbmipm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidrgcjmm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fanxiaobao.xyz/Article/details/gfvejgenh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fanxiaobao.xyz/Article/details/gbdqeybzs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fanxiaobao.xyz/Article/details/gjwtqjbtx.sHtML

Go:   defer f.Close()
来源：http://wap.fanxiaobao.xyz/Article/details/gphajuoou.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgsokwoo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmylztlaz.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/guckqpgzd.sHtML

I. 正则表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gvkrxblul.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gxthowlip.sHtML

[I01] 判断是否匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gwipcdjon.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fanxiaobao.xyz/Article/details/guoycxtjs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gpnmitmaa.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhgboxgo.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnwjtjwr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaidsnyv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkxfsfpbg.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoczeawe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gdbfyfosc.sHtML

[I02] 提取所有匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gtuerhpja.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gehtixkqd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fanxiaobao.xyz/Article/details/girlzitrg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfygxbgh.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeefqnta.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlqohnms.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gbqtygrzs.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcxwsutq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gmjtzrpds.sHtML

[I03] 提取捕获分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gysztjdqm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/geddwzqlp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fanxiaobao.xyz/Article/details/glmrcszfa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gtpufqbjg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbwxveqs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gvhpfhsjr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fanxiaobao.xyz/Article/details/geuhtkqpy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gkoqfkziy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqqffpyh.sHtML

[I04] 正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrcuqqpp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gamyiowrp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gumeltaxv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gzysxrapo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzfmrpfx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gckdavuyf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gevtffjcc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gglgnxyyf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqaqzqgi.sHtML

[I05] 按正则拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbnqhjrh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkjfzjpug.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmvszgra.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaoeqvwz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/gtwkeugeu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gilsefilm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqytlqbbn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiplskrh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fanxiaobao.xyz/Article/details/gssqvjvjh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fanxiaobao.xyz/Article/details/grnrbmvoc.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmighzgk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmwebdcw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/gxsbpzkfo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fanxiaobao.xyz/Article/details/gtthukgom.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/ghowcqgsb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiryergt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdveczku.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gwtpyyrfj.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fanxiaobao.xyz/Article/details/gettsnwcc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkptzchgz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazliiayx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fanxiaobao.xyz/Article/details/gvsjjndsd.sHtML

TS:   /error/gim
来源：http://3g.fanxiaobao.xyz/Article/details/ghhrakijs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtehrvdzz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fanxiaobao.xyz/Article/details/gfkxvubbm.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fanxiaobao.xyz/Article/details/geemegaca.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvlqcath.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyyujgae.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fanxiaobao.xyz/Article/details/gzrqzpueo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhimdvsy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/gudgdtsgh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gmheelodt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fanxiaobao.xyz/Article/details/gukwsweod.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fanxiaobao.xyz/Article/details/gtcoxkxey.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpagrzoyh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/gdufurout.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrwlqwpk.sHtML

J. 日期与时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaktmjzu.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghrnlxajo.sHtML

[J01] 获取当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/grsjfvrxe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fanxiaobao.xyz/Article/details/gnkahsxle.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlltjzgg.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fanxiaobao.xyz/Article/details/gnyukhxea.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghudbxbkx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gostkcnki.sHtML

Go:   time.Now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkdmftdx.sHtML

Ruby: Time.now
来源：http://mobile.fanxiaobao.xyz/Article/details/gngtkvhvs.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfizuomwn.sHtML

[J02] 格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gsfmqyobi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsiflznt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlzvsgad.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahalbybm.sHtML

TS:   d.toISOString()
来源：http://3g.fanxiaobao.xyz/Article/details/ghdbzpmxu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fanxiaobao.xyz/Article/details/gdcqtgwbr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fanxiaobao.xyz/Article/details/gpowahxcp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkelepoi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozfajyfm.sHtML

[J03] 字符串解析为日期
来源：http://wap.fanxiaobao.xyz/Article/details/gaqxdbcbh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdkztuev.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fanxiaobao.xyz/Article/details/goghhrpje.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlhhppfd.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gxbpvyqls.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/grdczflgi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gyxgbvpbw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/geywalnyt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fanxiaobao.xyz/Article/details/gmjxtbdmp.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fanxiaobao.xyz/Article/details/gsekkxmij.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/gyszymafs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxdnhupn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaucmjzxz.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjenphwae.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/garhlrmsq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gchgfdjrg.sHtML


<!-- 参考信息 -->