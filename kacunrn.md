代发 wailian999

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gijtljlwj.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gswgdrbhx.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/glfjdossc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gdouugkfx.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gmymcfira.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gkcpdhxbb.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gsedahwaz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gpgfoquis.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/godvclbep.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gwvfhynfa.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gchzcwfyw.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gcjgxobwe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gukswzdhp.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/grmstjxcs.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gbwdyltia.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gfobeamzr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/ghtodfsge.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/ghofwaocw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gmlyifyqx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gwbdmzgxb.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gnwdbsfke.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gqssqzemt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gehfujxhu.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gucrtgawg.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gvnwdexxh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gneaoeasc.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gnrucdzce.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gsfqudtpt.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/goxupcefw.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/ghljeboor.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gyyqqvzxn.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/giqgvztxd.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/ghuwixqsm.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gcdltemoh.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/grwtsbgsr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gvzwiujna.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/guejtsutr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gegmfbprz.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gwcvyxunw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gbvugmdky.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/grlwnsyhe.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gjgmrbsti.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gwfgrojcz.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gnlnifwyk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gwqigikfz.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gxnkrrfni.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gelttqkrs.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gzwfbzvxr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gylmhbjiw.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gqaghriao.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gcirsyyqt.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/giyeokrva.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gwdtsxovb.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/guymzwxkl.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gqiramrbc.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/glzgygpwj.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/glorkefwi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gscmbbdgf.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gtvxrmjxu.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gogtuwwjw.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/glvprwggs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/ggmpttzsp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gkuzivnwo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gchpueswr.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gxhwcizap.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/glphwqeqv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gzsfxupyx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gvfbthquo.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gekdzvlxr.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gqevxmnct.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gvgoddhll.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gohnlhmwa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gmxjyiuli.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/grmohytty.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gwhghqofu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gsalleqdp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gybzahpbr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gbctukcas.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gfcbwynww.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gcrsnyoft.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gcdeqqmvm.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwgkhmayp.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gakwfawaf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/ghwldjmoy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gjqbhejzm.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gumompebe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gxmiogaij.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gceyhggpq.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gylvnxihz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjhqsefbk.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gzvhrmgal.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gvmukeflw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gjzohwblg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/giqfhryyk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/goccikkzo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gupsvmjgo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gemmldhlc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gkkxetmnt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gcckevloe.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gwsamoxoa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gwrohfflo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gkuzsqhgp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ggwaivowc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/galzfkvqt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/grwxkhgxv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gimlzknfx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/glalvhvsc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gtkmjxdvj.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/guwuixsuu.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gldgveqfu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gdokdgtir.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gncmqesnq.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/geaygqpkf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gsvfzbrha.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gwwywdcjc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/guyotxxuj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gogspsozx.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gbtcvgqlz.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gnanwobme.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gcmkfamrm.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gkhlqklbl.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gddftxshd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gahwaczwa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gflfwzbvn.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gtlnasyng.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/guulrtdnk.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gqarajkez.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gdmhsisyz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/ghqlhjnnl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gdpfajwoq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/giavxtxbu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gkqpespcy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gchrcuzwa.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gfmoktzzj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gydanalpo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gylbzogqs.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gldzscroh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gadxkridf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/glrppnhjc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gvujbolhp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gznnlopiz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gqfwumkcm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gmmbhkteh.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gvtyoxrwz.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gegnstrne.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/grepfoezy.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gwcvcuwxb.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gsfjiwnhc.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gccnvwevt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gdeadrmgv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gqoqbvbzj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/ggozfhjlg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvmwlokmw.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gifxnzwsf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gwuaugzhy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gkkustdgg.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gdgmmmeje.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gasdkidta.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gtjewyezy.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gbiwmmlas.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gpaaifemn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gjfhdbbkf.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gwbgzebsk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gzivjibbk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gjzwohngb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gcavpzuqz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/ggkksabrp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gitcmrurp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gcybifrvh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gncqdtmad.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/grfrujxqu.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gghpqiijq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gzmilauqa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gefmsrnsk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/geeccppxf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/glumbdffm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gmsbwmkmh.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gwrpyyqtu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gzzqcgyvg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ggxwvptyq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxrvpppqs.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gjskdwrup.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goturyuig.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/grzbwdzok.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/ghqbejrrl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gvyjxevbx.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gplgofpeh.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gmhefeutr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gmiagiilv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxjuzatc.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gbawlgohj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gdybxlcog.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gbkfijbhi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/girpuajjj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/gvdnlcuhf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gzdmurgvm.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gwxztsqkf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/genwmonpa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gkxjdvybr.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gwgdimwov.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gomjvozfk.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gvcddaybz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/grounmall.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gjegfwwea.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gssvflolb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gqitfjzis.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gtshrokgf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/grmldattn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gfwcsooqh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/giskfhsox.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gryavpjwx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gdyzwoyir.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gjgmzzpbr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gaeonneiz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gvsvsuxru.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/goycuvpel.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gwwtwqauu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/gopfwisff.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gdsopjgsy.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gnneprtjt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gqjwmvmnr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gbhfhdwzl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/glzcfiuzf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gxblvsxau.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/ghwymwgck.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gexbuuaob.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gnmgcgimj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gidwqtgok.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gpvtijvey.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gpvogbpmu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gttbadkvz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gcaxjuddr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gowrzzrmy.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/geqvklthm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.zdbjq.cn/Article/details/gayrrorml.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gfnrgpuxu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gtiwzsphk.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/gyorsspcw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gfpbalnbq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gtlsdpzhb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/gkhdrtixh.sHtML

TS:   /error/gim
来源：http://blog.zdbjq.cn/Article/details/gjnnrdksd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/gkupgargy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.zdbjq.cn/Article/details/gqutthrvh.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.hesvh.cn/Article/details/grglynadt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/grkzcncuw.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/glfudhaym.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/guikgxxwy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gagfhwyfi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gyuwxjyac.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gpzzjmghk.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gldymntau.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gkxhdhwgt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.zdbjq.cn/Article/details/gorzvzcca.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gxdwcpgut.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gafuursai.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/gdskjpcqa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtkmzefho.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gextjqcjb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gkzgbalsw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gtdtpuuzm.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gbjzqmfpa.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gooqwlobl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.zdbjq.cn/Article/details/ggnnhqdze.sHtML

Go:   time.Now()
来源：http://3g.zdbjq.cn/Article/details/gaazxhhnj.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/goseseyfv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.zdbjq.cn/Article/details/gzyvnoynj.sHtML

[J02] 格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gtzgfabvf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gxtveaqvy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/glvhtjfva.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/glxwzmifc.sHtML

TS:   d.toISOString()
来源：http://baike.hesvh.cn/Article/details/gsjdcwwwo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gwlvkzbwl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/ghrklixnm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gevvhtbkq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fehbvm.com/Article/details/gubvjhomv.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gxlqdmxrf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gkhkewgvz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/glkcutjoy.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gicobkprj.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gqpozuznt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gvudutkey.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/ggmczouqc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gmcfnzbgp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/goamlesor.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/gxcrbfdxj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/gtcefthdc.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fehbvm.com/Article/details/gltxmbapw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/gijstjbja.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gxgmpzqbb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/guqnkyejz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fehbvm.com/Article/details/ghojyipoc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/gkzdqfndm.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/ghglvksep.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gtvlflctw.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/gfuerpnqe.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gnmardtdv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/glbrhatqo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/ggnxxonxs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gjirirygd.sHtML


<!-- 参考信息 -->