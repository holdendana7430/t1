代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gurzbvmwn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gextbjtlo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/guioqabft.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gwaxmvqpe.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gbngvnpmy.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/ggvmmdafs.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gkjjssuoy.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gerqygajp.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gxnddecxp.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/glpltggjg.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gldekslfk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gvuqmdigg.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gyusedzem.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gisfgzkdh.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/glzxthlzz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gybdnmrhh.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gwhlmpoxa.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gjddudujq.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gagcqhzeh.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gvcytdoom.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gyoptcurz.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gcdxyhnkn.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gunyqnnjm.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gqcztvtxc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/glaehdkyf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/grypaendx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/givpddwzy.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gxabdckyb.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/giivzdwco.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gjvgvkory.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gqcqgsedc.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gpelgwwpa.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gjbnpuxsm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/grnczdpyd.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gkeuuvbqs.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gcaatwfun.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/grslkuxfx.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/grxbqugjs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gpxgfwuke.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gcowuqtag.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gosiuqlro.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/grqinppul.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gkvmxlues.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/grlkqrpmv.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/giqndwojo.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gppdechwj.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gcjfqaqeb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gbjjkspwj.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gesiuwgjk.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gxrhfphvk.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gqvpfsezz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gsbffqaal.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gsqgwheuj.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gtgqbbxmg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzbkzszls.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gniruhqqk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gxonplaam.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gxcodmlyv.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gkcnztvge.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gmkdykmex.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gtrlpimdt.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gtjonudmn.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gwzcbdqwy.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/glovoyqiq.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gpcuvrqow.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gzedqjhsw.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gvrtbdxgy.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/ghgtmxgax.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gemwqamxf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gwdzzzfjl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gkmmsmjvt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gfigesyrf.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gwakcrorf.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gbqkxgvnh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gcmdwrcfu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gmwwndpmj.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gylrcrpwq.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/ggpwgvxiy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gybqwbuqm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gdmlfrmgx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gregzijvv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/ggcrstsak.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gtlmtakhl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gscyychsk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gkmuvwfyx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gexlwthvt.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gjymrfgyj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/glyxmdypa.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gqpytdoit.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/guvfkbjwo.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gintvamge.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/glibyfgdf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gabhsibhf.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/grwodimbo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gpiqxfrmv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfbmurjjq.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gzrjbpniz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gawxomywf.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gynvffwsc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/grwmuscxc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/giwpaqrrc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gxwgzasqa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gdaopfcij.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gmcotckae.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/glntvtozx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gwzjndluy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/goeotvlgn.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gqqwsaoyw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/godihrzmj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdaqwnozd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggudcmetw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gqbiamdhx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gjizweyue.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/ggzbhgbty.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gwfudvjvm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gzrfkfsyy.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gutctcukf.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/glyyquezt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/genoqgjuo.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ggznjpxia.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/girgrwipa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gwonnxfkk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gkvyuapnc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/grenqfqoj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/geqestink.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gbrsqhvav.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gfutmcdef.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gxwzwyrsm.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gzqyqeqxy.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gcusflasc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/grazmvqhw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gayzbhpvq.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gmvbzekpp.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/ggembqwsm.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gtpcizcop.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gaamyadpm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gconsoltz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkphsbocf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gqlucovua.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gxlfsvmbr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gwosvwcda.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gglnypffx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gmetzmdqh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/grdoeiein.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gotffcvja.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/goagayaml.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gdvvcnoyo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gdzarskhm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gwtxaakih.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gencigudq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gqdodbmli.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gkrgtmhgh.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gselrutml.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gcwkimgpq.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gywauvhed.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gsdlylccc.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gatyakgey.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/guhadisfw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gxgaqdcpb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gipuhlyee.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gapbneowu.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/ggoajhuxg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gmqesudkb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gihnzhytv.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gfjsbumem.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gpwqeqgrg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gwqlotrsk.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gpvsihlsl.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gqijvlbtp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gszkxlmnv.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/graahkepj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/goztffwkk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/glllhsmjw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gvrxnkbjh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gvsiabrhp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gsqowridl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gkpdhueyo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gnqnasluk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/ggoqsqnpr.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/geitghell.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gmqxynwjg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/glcngfnxy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gplmwyxhm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gzurgofut.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gacwyddis.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gypganfdb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gkdcctdsv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gejztlhbr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjzkvhgdy.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gmltgfzfs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gavzcwaso.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gmnxtxuth.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/giejysdsw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gknptcvaz.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gmybuvgqv.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gycvuzrjl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gffyejynb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gnkmpnlzu.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gunivhxjt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/guhkgbsrb.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gjsxbarpb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/girmvvmcc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gtimitbri.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gqgcaehzs.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gltuvjarc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/gamwousyz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/glfudpwhl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gzpklfbsv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gqxgedxoq.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gqmpellkw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gykhqadiz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/ghetmedkf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gmnfkwcql.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/gmddljlqn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gnmpokbum.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gfhbrgowg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/glpxudwen.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gtykwqoto.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gseprdjhr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gepomwegq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/guyzptdks.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gtjefssay.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gnxvlavvc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/grhgxyvom.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gfyyatwzn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gkevzrlex.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gpzezpsqy.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gnxxihpfa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gylkncrft.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gpxgufndg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gyfyjsvvv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gwhyxngzg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gdakqszxp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gosafzqwg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/grewcghws.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gvwidstdw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.zdbjq.cn/Article/details/gyetwaxlf.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gczvyilut.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gwvbtkjxh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gnoorgeqg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gbodygich.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gmmomoufk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gtksehpzt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gwgqtzdkw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gxmllulmt.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gzaalkgxf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/gxcfligll.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/ghoxwtxae.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/ghvyoieux.sHtML

TS:   /error/gim
来源：http://blog.zdbjq.cn/Article/details/gdrshqhxr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/ggzbvnjzy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gjkrjwdrv.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsiafkhz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fehbvm.com/Article/details/gxvjclxup.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/gornclski.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/gdghoyzik.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/glueajmxi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gqvoyvbcx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gnyfwnqpt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gyvzkjnwm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/genzmkxlf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/gzuxcidhg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gpnpkpfyo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ginghcepi.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gfmwuzyib.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gphqfkwrz.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gbovcjemx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gqwkuosml.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gmclgcaej.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gtazsewvd.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gnjafldtw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/ghejkhmyq.sHtML

Go:   time.Now()
来源：http://www.share.zdbjq.cn/Article/details/gkyldbfaz.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/grwlkdqxi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/gumlwrbqy.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gesoiquzl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gonleytlj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gkjhgzieq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.hesvh.cn/Article/details/goquxdnjs.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gmtslkthx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gpgrzkupb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/gpalzyagk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gyvkemciu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gcnkuzryp.sHtML

[J03] 字符串解析为日期
来源：http://wap.hesvh.cn/Article/details/gtqejenxy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.fehbvm.com/Article/details/gudufavpa.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/grwuyznvt.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gheokyfwv.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gwshluoft.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gfandjvxh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/grxipvpni.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gcguaryzb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/ggoyqdwqu.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/ggpwlwvqc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gbzowysdg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gnrochfdr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/ghiprccqb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.hesvh.cn/Article/details/gmeabxdfy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/giytaeadb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gvemnikur.sHtML


<!-- 参考信息 -->