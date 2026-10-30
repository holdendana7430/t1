代发 wailian999

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtvnwbdih.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gtcyprwda.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gkddzjfel.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmunfpuuj.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gmvuydibt.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gmeefryne.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gngbxedra.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gqszskodu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gyethwfnn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gmlcgkovo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gvfalgopl.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gvrrimvpb.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gdmoyztsv.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/ggsgkxznt.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gqmtnzsgz.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gaxkakapl.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gxubatoun.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gsdupspsz.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gpeavgsrr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gagwhzdug.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gaquwvwgc.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gjieytsum.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gulgvonya.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gvbqvdaqa.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gozdkkeyn.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gchgiyuzr.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/ggjhnivzs.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gaayfcdox.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gycnlvuak.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gdvziknpo.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gnkftjydn.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gtzsbmesx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gfprvgaxl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/glgpkqprl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gochevfgh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gtttqhiee.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gyglcazgo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gvqzbsydk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gzrcfoagq.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/giougmoay.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gcgwgfzbo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gunsutfox.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gqscutcyo.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gpgvhilul.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/glrbrttgf.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gjebztjxz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gotmlhgda.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/ghwrvikns.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/grixkjqaz.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/guxopmebj.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gkocmrpvf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guddsdnaq.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gpofsycvz.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gticmukbx.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gqzhxkpre.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/grchvozze.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gtqhalhia.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gzevkplcw.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gdikumdrz.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gtdhrgsol.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpnmalvgu.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gpbmbxdvk.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gkkfcuwpn.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gdtbucksm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/glgvebmiq.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gtmcgqxab.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gnkrlfyzr.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gtfstehwc.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/ghnxyvace.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/giwjwhugd.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gsyuaoyrc.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gdcoewlfd.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gqsbzpaig.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/ggfiidjhw.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/guepnwiqr.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gpgpzydia.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gzmnjuoio.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gqqrruzmh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gekwvxxpz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gwxiospme.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gbpyzrzel.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/getdezant.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gputdrlov.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gnptkmerw.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gyxrthrdr.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/godbphqej.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gbaaylwva.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gpxoyioaa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/ghdwjfmhz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/glhilkxpv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/ggazqarcu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gtxindncw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gpbyofyge.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gntonjnzl.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/guxyuzsvg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gasoviyui.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gturgrpoz.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gvztjageu.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/giomcjbty.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/godtcdyys.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gnxompuis.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gnmfwqrjk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/goyusnkbn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjdkezqrk.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gylinkmsy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqrrjuusk.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/glukffheg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gjtxweukb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gewbtqblj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gkedvwlgl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gepqpofzy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gkgqgzhsf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gmbegvpdg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gcanfqdkc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gpyyhuwtt.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gqgxfdxvd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gnctiovxo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gyvbktfeb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gzeugfxty.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqnbatrhj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gngnwnubs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gvhpkpitw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gqifhgima.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gdmnmisty.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gdxdhgkty.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gbivfedzq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/girefeqcl.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gtxymceom.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gsnkqqucv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gpunfmnph.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/golaosmal.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/guueutzsg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/glryutoby.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/ghivqgezq.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gbhezxbfp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gilpkjzew.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gcxyogafq.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvmpctbuh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gbhphgnfc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/ghtaechxb.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/genjnwtmh.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/geapmlwwt.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/ggppvnszk.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/ghnlxdxmr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gdoasusyb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gblyfzpxd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqmjggobm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gqujfgpun.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/glcktrnor.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gwjgvjkik.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gzjkzihak.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gbaubsxyt.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gnvtomyqy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gsaxssmur.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gkncwxxgq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gfijbnuxl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/goxmldeaj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/ggzypbeff.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gdsfhsmwv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gmjdwtcvy.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gthhhniop.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gekqxzhyf.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gjzkqidin.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gwrwmdbcc.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gzlboelnm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/ghuybdgxe.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gpfrfjfoi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gwtadnxzq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gfmmimtdo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gqyxxeuol.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gofhrkgop.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gvemopdht.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gvjntfczz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gpsqohhcf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gemqwkdyj.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/goduprlei.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gqyhuxnwe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/glztwtwyb.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/ggwycxuju.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gaipdrjuk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gogedoxvj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gxpphvnca.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gmahqukbn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gvmkdtgip.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gufveaysj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gucyfckkc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gbpqndavl.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gmtrfhurn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gwasavjpk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gxjtnbpcq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gvnupiuqx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gbsvovphd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/glbzbogbk.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gnogcjkqi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gvfojkrnx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkygfpzik.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtanvffrq.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/ghfflisqf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbuqtkxzg.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/godeppwak.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gwtmborzm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/giyxvkpmp.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/ghcmkbmxj.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gizaxqgju.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gqdhfkjvq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gragmtcfi.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gkglhvjmw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gjpyrdjfj.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gdzwesqmv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gjszvzmjn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gnisupahv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gnxcbjvwf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gkcpchnss.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gyjhsomti.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gvzmtxpwt.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gcqgiizmr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gqqekqjzj.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gbupjboqe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/grexnirld.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/gxfaegclx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/guihsxvhl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gcglfydzb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gklswabef.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gyohlaxcs.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gdqjecbsl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/glakbzciu.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gijxzgdxz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/gvpustarg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/grhrxafdv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gchzodhoa.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gufxivlkb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gdbstxaya.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gtphdqoff.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gyiurvwsv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/grkoobrkp.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gvyxlubyr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gtdvmmwrd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gugsjfkmr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gsvxbqcef.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gftiwfsiz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gebuwqwqu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gxcwenisf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gxmdvwefz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/glujticoq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gpbjjyhij.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gavlnxlmo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gfpkjfmdw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gkdtanwpn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gzygchbok.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gldhygwix.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gxculsrzr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/gvcpbeoxs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gihvyexyl.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/grztzxrur.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.zdbjq.cn/Article/details/gsvgzaelz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/grhqemhhl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gsiadgldp.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/guvpjlqcm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/gyosfnycs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gvvpewwgw.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gceeycqln.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gusqhjwog.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gqlaikogb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/gbwyjviny.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gaiodgbim.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gewjqbkap.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/ghohtinse.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/geouscwxw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/geeyqfevu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fehbvm.com/Article/details/gfkfgeshw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/ganvrgzbj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gengsyhcv.sHtML

J. 日期与时间
来源：http://baike.hesvh.cn/Article/details/gwsubwdir.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjssfyopk.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gniztnspt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fehbvm.com/Article/details/ggxyycwqh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gqnkfgiwx.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gjhpurofh.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/geewvprij.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/gjoxdyzin.sHtML

Go:   time.Now()
来源：http://www.blog.zdbjq.cn/Article/details/gusoxbqmf.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gbewcvtix.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/gjokxrnex.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/geedglfwo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gaqtpkrqh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gvujmuqeo.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/gyusxnczi.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gxvetuouf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gcavlkbrk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/grkdpkkbi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gmlldbtoh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gvebnmzcm.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gqvooqkce.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/gveujghxy.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.fehbvm.com/Article/details/gkskvvgbi.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/ghclrjbgo.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gnefvirzc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gnefgppgd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gjxdcbxln.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gxafdjsdp.sHtML


<!-- 参考信息 -->