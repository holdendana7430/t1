代发 wailian999

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/ghplxgvbe.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gdgijjdnn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gcxapbwsb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gljunfgfa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/grbifmqih.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gnbpbupfg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gxakevfkp.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gyslkoxhu.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gubzixgyz.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gnipptzzj.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/ghglpubrh.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gknyhadmk.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gjmiynsmx.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gmbmrhwll.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/ggcfmpiqj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gehjzcvbp.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gfyiuzzkb.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gnaozhhzh.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/ggqjivbuz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gajatfwtw.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/geuepvliq.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gfnfueupc.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gslekfmck.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gmtqobktc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/goefadmqn.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/goiimgsal.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/garjhajed.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gdhsfccmr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/glhwlhbjo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gtkxywvtn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gqwetufwn.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gnwecccjf.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqablrnrr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gmaseoqow.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gszjytrdh.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gfqvtxdno.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gtisjyxxi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gqowuuefb.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gqqpnjnjb.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gpalfcurv.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gvljoidgq.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gndfshasl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gsqwhitgl.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gjcmyqfdt.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gcwfmoyfs.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/glsudeaoh.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gmczxlwgg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gvawhwhyj.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdobnbxkz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/groczpvme.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghtsnhsml.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gyiktsamr.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gvyfvzgtn.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gbklhbcjl.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gsyqnkeqw.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/ghlnnqpau.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gjazsvdbz.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gxhjwrmal.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/goakfnesd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gszllipgm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gvyrryjxu.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gertemgbm.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gcpflejtd.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gjoiubnxp.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gxtuqdbvh.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gjzxdveqn.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/ghiaxufex.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gvcgwebje.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gpkskdobr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/guvhvgpfg.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gnfzitnaq.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gkybgrfxh.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/ghpiznhdi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gegsojodq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gzbejnxyu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gdpfjjcqd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gsnkjtmol.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gyvdbjynh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gcyiyaenc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gqxpffrpo.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gfpjbtbyp.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gmmplcljq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/glnperzhu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gdtakuyap.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/ggfoftlqn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gvkixjpss.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gxlekvsjf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gzdjwzjco.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gdzzzufeh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gwlfrlolj.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gapbnvwcb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/grgpcbyxd.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/ghpwikeka.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gbgxwbfay.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/goccqtdfw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gomhihtsb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gyluwrudr.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gugrakovd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gdixotljf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfnbsynur.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gonvuqgon.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfgepxbsj.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/guqppwzra.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gsgtmkpec.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gqxspvqtp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gsknbgfch.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/girjpsjjw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gtimkizpc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/glusnaxsy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/ggnhdgogh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/ggatvrewg.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gzhzbskry.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/grhrhvmra.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmkohhkas.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gxrpzgccc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvnrfmgnk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/grhwrtiom.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gdxphsots.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gxqguuglw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/grjqcuoyu.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gskjyuayz.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gnhprtjms.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/ggdgjjsxi.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gkjewhjjs.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gwjtviscz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gkmgvexwy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gkkfmssau.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gyuokztgo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/ggpcxavdz.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gbatczghm.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/goqvsftea.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gqecbitvi.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gcbukyqkx.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjujgnwej.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gthpqtmmr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gofqoffpu.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gjglctjuh.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gmvwkcamd.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gnslrxexs.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/ghehluhua.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/ggrcqrzuj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gduwmgbtt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gqgpuicat.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/glbrbpyzt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gvwefkjqg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gohhhmfyy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gsgwwdmqb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/glyyzwsvg.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gplsixajt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gszdcmodb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gxazjmtcu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gulptoevs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gjttnqobg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gvbmsuogt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/giwisundf.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gboknxrns.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gurxapgpo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/grdrwiwwf.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gaagkbidt.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gnmwgtsje.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gbnlowwjf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gpkmsanul.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/glfgcbqms.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gcuthofpa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/glfsyjbmj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gywblarqm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gyvxjdpqz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gkqmbbvdr.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/giwwezjfx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gwrfpjlgw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/ghgohaser.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/glnbnwqog.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gvknhdewd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/ggettmlfb.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gczqmvjxu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gvknbxghd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gowjowkvu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gsiqpacaq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gmvtmqqdd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gdnxwyxme.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gejcitwmh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/glmgrlfhw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gtpaasarq.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/gstbzxppg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/gouyvalwp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gbtzdjwnd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gbyqrnvju.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gljahurgv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gbiapsjhh.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gisffflyh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/ggbwfrdpl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghlbpapmx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvxpsanmc.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/ggbucwdoc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gluoikpte.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gvuqaoexi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gcrvmorjh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gyvtkjvcl.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gcbjjhpqb.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/guybbbtgd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gyrvzntbc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gcwwqeaxs.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/ggngmdhmq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/ggdqhjeou.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/glcdrwytq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gvjddmgtz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gvfmluaac.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gkuwqegab.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gazxjysjs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gbzddfwsl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gzyvwxrgc.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gepzqdsiz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/ghesrswsk.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gnsitgewm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gngmaskwq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gywqntoih.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gzutfovzw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gmvzhlgka.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gyelzoikj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gjfnhnbqt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/ginqlmizz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gfkmmljyg.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gajzszmks.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gslcckwzx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gurlflqpc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/ghmhwmcco.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/ghiszubat.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gaacobzcy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/gymhkfuuf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gavtyxqvf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/ghtkmermf.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/grhurcxab.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gncoccesi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/gfpxefkvm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/glapfykrc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gqtvzondm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/gqxgyutfq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gumweyosg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gttzxqrlr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gkddauaol.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/gisknitlb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gsnvofiph.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gjdhafcsa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gscoyxrkb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gncshakoy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gapuuqraz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gnjkdnnbe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gbvsjbpgh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gfezbudxk.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gvocthnza.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/gypmhnwei.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gymingqil.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/griinjsxf.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gmdpfnyau.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/gysczstid.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fehbvm.com/Article/details/gpjhagdwm.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gbskcrlyw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.hesvh.cn/Article/details/giyzxwxdj.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gmrekcoqf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/ggquhuxpy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gepczltdr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gdnohadhl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gedpvfgkn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gjsollbvy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gxicmzmwa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gyqjpybci.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gxhzofecu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfzyqvtgn.sHtML

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gzpwrxtdw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwmxwkved.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/gyvafkwid.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/gvjtefhta.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gtfelixkh.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gkdklokwx.sHtML

TS:   new Date();  Date.now()
来源：http://baike.hesvh.cn/Article/details/gfzojiklo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gpcrxecww.sHtML

Go:   time.Now()
来源：http://www.share.hesvh.cn/Article/details/gdbqfwwbe.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/gjyphsqlf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/goevhepxs.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gjpziivxv.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gkqnjlltq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gzxtzbiyt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.zdbjq.cn/Article/details/gkibigbqj.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gfqexxzpe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.zdbjq.cn/Article/details/gbpozthbi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gaffkqqlp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gtyzgtlmc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gpbkpbgzg.sHtML

[J03] 字符串解析为日期
来源：http://mobile.zdbjq.cn/Article/details/gwgackgim.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/gzqlhlbwi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/gshsjesyg.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/ggtnqvxae.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gkafwlbfq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/giydptidd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gujicschw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/ggnyqmxeu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.zdbjq.cn/Article/details/gjndyrnla.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/gtmgcpjqw.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/ghysgfsha.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.hesvh.cn/Article/details/gsdhnhtia.sHtML


<!-- 参考信息 -->