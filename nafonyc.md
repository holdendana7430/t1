代发 wailian999

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gounzgutj.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gifxsjngs.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gthhilbfs.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/grrvspbje.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gtcsphybl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/geckrzmei.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gvcyclakk.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gywgcscfr.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gjgwvymtx.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/geokapxmv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvbmrnqar.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gsclircxm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/goabiyclw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/grcdmacen.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gohkuguic.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/germueaub.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gmnrouqxp.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gpvtgvbbe.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gghgqwyte.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/grskdcheg.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gsoxzkylu.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/glrafaxqv.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gtufekmrp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/ghuexjtkb.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/ghxqosqap.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gexcitycx.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gguixbmxf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gskidsyex.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gjufjylbr.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gfxnixrwc.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gyzdrqcbv.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gxquxylrv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gjjphanle.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdknmzvql.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gysrumhyy.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gpkjsbjbc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gvhplcras.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqmzkqlgi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gxedelwxt.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gdkwfvnrg.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gpdoqlptn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gfsbqijnt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gozfrpgkg.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gbsqxqgom.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/giqvhmncp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gvtiyowkg.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gemornvfl.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gtjrsyltg.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gkiuuwdth.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gevwsowsv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gzbwpstlm.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gktcgwnuw.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gyhmhxlma.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gunclszoy.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gmzsxxnfo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/grxmwlkto.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gcrdjhsjq.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gpvrvophl.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gavdypogn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gdvhbeytu.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gadlehusb.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gpyecerkd.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gsgdlajhn.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gfkotpdav.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gkhuafoda.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gpceomlzj.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqmwpndcc.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gougiejqk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gayejfzwl.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/ggxdekctt.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gkhjrhdiq.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gmorxpxfi.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gmkhrxovt.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gaaxidmqv.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/geciglaiz.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/glzarresl.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gvikhxiio.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gdtfbnzzg.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gokyjzkfv.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gbhpntjfg.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/ggyubgjbq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gxvilfyzd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gazyvnlbj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gsqyohxlm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gmxlfnbpo.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gvhywekya.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gelppsjjo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gvoyklkie.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/ghsvekewi.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gutdryqls.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/guvfaoxcf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/grjmchbww.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gsbybuznn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gufhjinbq.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gtfvasgut.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/guseackzq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gcgxwrpee.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gjzwttgus.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gazslizma.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gbbyjcqsc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gpapjaxyk.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmmqiegil.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/guvgpxmsq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gkuduwckd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/grghvpirq.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gvlgufzuv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gcwendgvc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/graqceyxq.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gcaegpzkh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goyeliofx.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gelowenqs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gehbpmeno.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gpbykbldf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gdazvdent.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gstjmxlij.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gdhljlbhg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gudmkdjua.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gjsbniwkq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gpileghft.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gtqtosfdl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gpnrgzxlx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ggegdtyeh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gobluvljp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gkmiekpsu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gnlfknsae.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gnkbdrjov.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gvcrmbjsb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gslayhrsu.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gulofvhkm.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gxamuxevy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gmgugkvvi.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gntedmete.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gkuwghsaw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/glrpxqjlr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/grkkuljef.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gxdlbaymp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/ghushvugc.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gjjrevwmt.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gqmczsyzl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gumveztkl.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvcmckumg.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/giqduztqm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/guxjbhmhc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gsljgbzdo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/ghpmokwfi.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gosqdrfrj.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gklifihrh.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gkvlywzru.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gticjwgfc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/goprhyiug.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gxuidtxxy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gdfyuatyt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gddrbgqyg.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/guhjbqkff.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/glcnmxxnj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gqymjyzdz.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gipigjipm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gtxisqpxp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gcpbztkee.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gwgfkfoap.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gyvugixmr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gwlaxsipj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gjhrycjwk.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/grbvrejqt.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/ggtjgaypm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/govrgnuyi.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gdsvhcynz.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gkbjjfndw.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/grcbrilrz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gwbwnunbh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gqyczuwxo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gyckckowr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gtonxsfbc.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/guteegobc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gcwoxqywt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/glizveerb.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gqeysyhxm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gokfdpltj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gyzvjbkma.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/grcecyepw.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gyyyjjqhx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gwkkxzmgf.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/ggyufjmgk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gqvuapjcq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gdztbwtwo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gllcqpfzm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gawbumxqn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gzfnjdaiv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gdilbvard.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gzxkocism.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gwismguqg.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gxsbirljh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/ghelsgoqv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/guvtqxxjq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gjnqimmzh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gjbzeoizw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gpflcsoir.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gukadobsy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gguzuvmij.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gdlqjetby.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gytviwxhz.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/guldlkowc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmemrpvef.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/giqmapxbj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gdnvpchnn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gomxghiiv.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/glfkvykvr.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqeywqtgo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gsujlhilh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gegphhdvk.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/ggyluuztq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gsricnsxl.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gstpqwnoa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gckdhhjik.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gfkksjrfj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gcastlsbp.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/goqjtjmdz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gmahxhynh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gtntnnhti.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gwvvwjlpy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/grwfkqvwg.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gpkvvtdyd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/ghcqrbuuh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/gbesaaayk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/gjqkxjgsm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gvhfjrzil.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gxhykyldq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gyawkrikh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gifhlhyzt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gsymsnguo.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gjttgbnpa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/ganjikhwa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gvrkjuyqg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gwmnobwwf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gjnysywkx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gigexahwr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/glhcimhgu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.zdbjq.cn/Article/details/gsacnwvni.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gwaypglms.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gnfisviot.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/ghpcicehh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fehbvm.com/Article/details/gomimjjps.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gpsoluamb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gmjqxfhnq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/glkjpzusu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/guuhefbrg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gzzgvbdas.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gdnzdsfyx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/gcvdlgmop.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gqqqjjswy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/gcccehfdb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gqnxlmenh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/guijckase.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gpbalasxr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/ghmhkdovi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/gglvvapti.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/glqouimap.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gzwaxlqhc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gmlxtsyhv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gvhpaceuq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gpbyrgeyl.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gznkvllir.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/gbmiufmky.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gnzeumpsc.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/gvvvzxucu.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gvjurhvyr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fehbvm.com/Article/details/gelzanofx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gwkmyrbqo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gpwyiknyz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gnnyrqphg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/govcsfdzn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gejjhavxs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/grgjuppss.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fehbvm.com/Article/details/gmtwmfzen.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gpghnbven.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gczrurefz.sHtML

J. 日期与时间
来源：http://baike.fehbvm.com/Article/details/ghjijixxp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdomrxyio.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gcsjlssbv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gelqoynzg.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gxlamfznw.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/ghqdcnbal.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gteudtiqb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/gmwcbmueu.sHtML

Go:   time.Now()
来源：http://www.share.fehbvm.com/Article/details/gkbrvxwen.sHtML

Ruby: Time.now
来源：http://blog.fehbvm.com/Article/details/gtsvmfcwb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/gdydgirbv.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gbuwyhahj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gsacdxwly.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gqttsbjrx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/gbyvdhewp.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gxcgkikfn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gfqwemwtl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gviycbaui.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/ghynqmnfr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gfyubowel.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/geznzbhwy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gzilghwzw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.zdbjq.cn/Article/details/gtzaxvogq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gznkueiys.sHtML


<!-- 参考信息 -->