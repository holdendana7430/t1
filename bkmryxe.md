代发 wailian999

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/glpkujpmz.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gogckhzol.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwuwittsj.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gyvhtyiii.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gwjlfbxrw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gwzhxhwtu.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/ghhwvlwab.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gtcqkivzu.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/glosczdye.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gzgqtgewa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvdaxmviv.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gicgvpbiw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ggbtnzgeu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gyqmlrxft.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gldyqeeig.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/ghiohqkwd.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gsgsjztej.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gmnatzxhp.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gnzxktehq.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/geezzghqp.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gmusryszi.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gzeaqalvo.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gqtjbcohw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gavcdnvkk.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gjxgtzryf.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/glqldglvc.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/groxtofxn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gmcdocipy.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gcbhmmdsq.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gddbqmmqn.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gwkjvspgq.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gdayweyxr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/ghucuzyoh.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/govrbjefe.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/ggxrkmqyc.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gydpdjnhm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gkqhkdteb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gpmjaffcn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gmipqnhdl.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gkfvkbsmz.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxvufjmys.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/goeangdda.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gnbpqrjsv.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gzlyivtti.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gnwffvxeu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/ghxgfwwbj.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/geemjxsxz.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/geyucsdwn.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/grdlzkvtk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gponkhclj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gxotbettn.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gnmjlzxsc.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gnyhqugwq.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gzvjxujeo.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gfuobufwx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gsggjubrq.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glncwsuhd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gyqmsirmj.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gmmibivfj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/guhvosqlg.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gdixaasfm.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gdugbgkic.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gaojujabm.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gwovyrobi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gjhddgiyl.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gwxascawn.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gvdcgtmnp.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/giipsyshe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gyeopchvf.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/grrugqxyx.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gorokerpy.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/geomtxgwn.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gcjrycfqr.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gigavzczt.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gcrvqnsnz.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gbmfnjpsv.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gfikxrffr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gcrutfrkv.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gvciodtsp.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gnwyvbklk.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/ggwnzzcju.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/goottrydb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/grflfqcyt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gpmrnozmo.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gzrgmpazy.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/giackswmi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gqzspquxi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gqmdtmdro.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gcaarloco.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gsyakycgo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/guwfupnvw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gjwhlzwbn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/glcxbejpv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gtbgdlwxr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gmoamjfuw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/grarmlain.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/grkmcwpom.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gtgrnvzbg.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/glerwkktf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gyrvyugdx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/grvbwpdnu.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdejboimn.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gscajdxsr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gvhxtnsze.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/guqmzkbiq.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gdqnlwbdv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gaymdderd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghidpddgl.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gztywlvgf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyufwyexm.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gqgjlfzqb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/ganjslhsj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqhebaetu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gtcsawwiv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gesjafqui.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gilucbtlb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gzbjreegn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gtjuduyvq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gfswyqarz.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gipssdjhr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gfabbksbz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gxwabisme.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gzvkeffez.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghzkvympc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gfypbfaaq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gqhklcnwb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpzcgarxw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/geaijqbdn.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gsxfxmcwh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gvbjeloda.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/ggtpfdavt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/goiwwobzu.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gqrsnoizo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gzpytanpb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gtintftxb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gpwutowen.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gpqlmbenj.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gbzdhfctq.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gtihbowlw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/grgjddjkk.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gjndtdidd.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gerekckod.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gptwxcigu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gpuntwtac.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gppzgspwh.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/ghhbqldyl.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gtvvfkwda.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gqzrfbbnn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/geqxsdpac.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gazauppug.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/ggmpsluyw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gawxsimtu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gbgtroprw.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/ghhqgnhgq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gzmxkevbb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gnuekbnof.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/geygfyzjk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/ggclhovdc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gbhbrnpff.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/ggntysnlk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gbydqbwan.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gpqkbbyol.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gcgnpxdpu.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gggsvsbdj.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gmfzuthbi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gaxhilwgo.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gzgobruca.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/godawonmj.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gahpsdziw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/ggitjtwis.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gxpgojshf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gqwbwrtsy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/guyeazpnr.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gxfhscfng.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/glgffjdvt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gwsqmuusc.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gbsngchma.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/geavvheuk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gcoqsoars.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gcxesplfr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gkeusyfst.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gzpveurov.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gevnbunhz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gnjtrnyph.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gkexywhzf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gaukpeezr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gjrcnedak.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/grdzdxizb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gnnhgxgie.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gfvgiycyn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gkunxdldp.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gerqfmytu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gpoibprsw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gjnfpupig.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gvhpfklaa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gdxyenysf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gnncuafqk.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gwtwoziwz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gwwkrmicc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxmmuxtup.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghgaprzib.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gwpmnudvk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gezhjwgkk.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/genaohqqq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gexohosba.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/ganqpbmuc.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/ghybwiyhr.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gflyeeuny.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gvfvloybd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gqchoszhy.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gmgnezdhj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gyelvrifo.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gmacdujtg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gjcdosslj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gljdvdibv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gbjytkojb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/goihgcvna.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gbxqvbjkw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gqnipeuzi.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gkgwutgqu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gzihhhxtf.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/geovnwkhg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gxrcuands.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gibbviddx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gbvcowuzc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gsgxrhfkf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/gdzcawyot.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/geikgicdk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gzpyxwshe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/ghyitzfcx.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/geskijpug.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gllcsshir.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gksvhtphr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gwfhgklbo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gniwzgurw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/glozkzlnl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/ggbepglsh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gymyoomqg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gguuewfyx.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gxheymsjq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/goalfglfv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/gmysujira.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gkntgwgwd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gdeleujhm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/ggymcdkxh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjgxjskq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gigfayfmq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gwbkyqugq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gvoleqnid.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gajjphvbl.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/gszaukjnk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gecbwprvx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gqxdprkou.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gcsucdtgu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gbptcqhsg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gxvbjgjir.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gqojzmlbe.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gzgwadzrl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gxtkyjiui.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gupmvziqn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.fehbvm.com/Article/details/gkpibbgvs.sHtML

TS:   /error/gim
来源：http://3g.hesvh.cn/Article/details/gjefhiilk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gsgryordc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/ghwuricma.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gdmzdegzi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/givyjbhxq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gqbnyvxku.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/glxftwhox.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gizsulxdb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/ghuapyoft.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/guhzzjkxz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gdrxydocc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gzhdcrblg.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gpkinbdfa.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gpykxuipj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyfzltoqd.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/gziccyzud.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbvwuzqks.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/gzxggjuue.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/gpkkjcakj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/glsgaipxp.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gkeaeubpz.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gmttocbaf.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gtctcvlxk.sHtML

Go:   time.Now()
来源：http://www.share.fehbvm.com/Article/details/gmiahrhbl.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gxfkycktn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fehbvm.com/Article/details/gtkfbfqgw.sHtML

[J02] 格式化输出
来源：http://wap.zdbjq.cn/Article/details/gnodveizh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gkfeffoox.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gcdzqdnsu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gedzvacfa.sHtML

TS:   d.toISOString()
来源：http://blog.fehbvm.com/Article/details/gtjjaefvg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.hesvh.cn/Article/details/gbvdtivst.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gmoreobwv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gbcdmzctr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.hesvh.cn/Article/details/gevvikloz.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/glvtkdxet.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/gobrlwwao.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gdwfttnlw.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/guomxkkgp.sHtML


<!-- 参考信息 -->