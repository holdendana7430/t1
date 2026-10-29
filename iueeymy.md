代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gtpaoneso.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gmpiwplsb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/giufnlqcw.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gxmmlliuy.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/grqocnqvy.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gnbaztqnn.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gxvhrwpov.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gsflgsibb.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gioqdsnui.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gwcxmtxem.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gafcigvlf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/grvudmjjh.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gdqgtdkxm.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gnvtgumlf.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gghlnufup.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gleexxioh.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gaipndoig.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/ggdirppxl.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gvzgdrzod.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gxxrqkady.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gfwmnygva.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gumvnjtqa.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/glnmzjstt.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gtfppylny.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gzmwgyxnw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gkqgexbie.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gvfwsozca.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gbjdxssbz.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gfdchnjjo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gjdfmillo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gpiwuazqx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gtkdjusxp.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gycxgsdev.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gcuzpvarx.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gjrvfblna.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gjgfbpozr.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gahjjxdfk.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gahahifll.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/grzwviclc.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gbsahkbze.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gyljvbrwy.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gurjdiopv.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gyudwxdch.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gokopfeyk.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gmjzajdne.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gpattdfde.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gypkyepdf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gddxdxykf.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gjsmnhsjr.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gyuxgubmi.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gwffxxcug.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/geggirbjp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtzrovfow.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gdrxhbtvk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gnrsasgox.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gyxmpipri.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gsocjiezu.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/grhcqghds.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gomcrlyjc.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gikevhfll.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gugilbgfy.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gwnvullos.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/giyzadzlj.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/glhnuwehy.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/guwawyqfv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/ggwvzezwl.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gxjhttumw.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gqcbohvnc.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/ggitbsvau.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/guvddjtqu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gfmowjnuw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/grmdgxoxy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gvryvcgwk.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/ghhnqddbv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/goipevjsk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gowttejyo.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/ggocjvddi.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gxtmhrnaz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gcakuqkiw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gnmexrwqm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/grzesqozu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gluxpvjzv.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gzvetajsa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gstlkbzxd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gscfadwac.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gxcshsmpv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gzqxmfnrs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gexaextay.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/ggvfthorc.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gcdwcmgnk.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gviehnvlb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gvtuptlim.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gbcciryhz.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gzbuykmit.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gfzjfswkg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwjikogic.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gqlfewzth.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gprdxwyzb.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/giwckpvge.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gwoqmtxjz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gwkmnuxag.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gluarnfxg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gwjpyksby.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gjxsnvyjs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gbkmiznqu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gbsevaehg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gkeldngqb.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gvpygthln.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gpefgykyx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gsiblqkri.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/golnogytg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gphxxerrw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpumikzpb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gsbiskeqg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gyrhsnibb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/glooltdwd.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gnvwcnnyk.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gfpedlhpz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/ggwxaweyb.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gedayfgws.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gttyipugt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/glrdhzqgv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gznyhjzvo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gclbsfwub.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gggrlvwra.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gzxojcbcl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gsdgxtxkf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gyyovzapb.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gvnzwybjr.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/glwoqjdjv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gexznmidd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gyejlspem.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gkrciwxur.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gicekacei.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/giwtxvdqq.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gpyxwwvvt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gbycxxrkw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gduampous.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gtnuaxhur.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gieglvais.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/grvgdufep.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gfzvosrqw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gbakyrjyt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gtexjvlmc.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gkvvsjwbb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gzpdpxqch.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gggycnqrj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gfkofgxuu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gbrmhtmpj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gqnrthxqs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gdfaugezy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gbxywbzay.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gewermabl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gabacuwdo.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gxabkbzjc.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gcirrlwps.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gviuajfds.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gyqwogeeg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gqtenlwjw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gtvvfwnuy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gazdlvvhp.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gxificebh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gysiaxsfb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gbuynjped.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gpjomnfrs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gsaruluvm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/grubokwnn.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gwlqwspaf.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gmgbyympb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gsyacvvos.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gxarmqpel.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/guahxzixq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/geduzrsqu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gkjvxvcoi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gjdhkbdgl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gtjqeuvhu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/ggailkyfe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gbkbzftye.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gdtqnbqvl.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gialkazcv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gdthffyux.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gawffukbx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/ggfbfxmqd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/glsoiprbw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gycujxydi.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gmjboghxi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gzasuelpr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gypldbiqq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtaewzprl.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gqeyfforv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwfqgplex.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gmznsjiow.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gksugjzfi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/ghvamczni.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gqcozthte.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gekuigfiz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gsqodqmyx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/gvhjeixyi.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gcbjrqmxq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/guzyvejvk.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gxyvlzeha.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gtsbxetwt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/ggcojxtic.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/giiphndpd.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gadfzeovw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/gsbyyvkim.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gibnlzaqg.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gygtoodwe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/glnofrlyp.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gctaoofuj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gymfezyuv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gzcxsllqs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gzclomhrf.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gchlhklem.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gvrowqecg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gmujmasqx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gleyqckvv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gxiottpjx.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gasdxpfsw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gobpsoevi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gndyxmogd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gjevxqlgr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gtnujptpe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gokitnene.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gciesqcol.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gibhtzjoi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gviaioijw.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gfmyssexu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gpryoyfiv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/gqgcgxchl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gbghthryk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gdzdhpfiy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gdixoqzat.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/glzzpwbxe.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gbxwopwix.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gapgemtvq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/gxcahjixe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gbhdtebyo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/gpxnwrmjf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gmtdtzgxi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gqxwqlnvr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gotqdbroa.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/gkvzdgjxm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gsacbhxel.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gwoqiwhyx.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/gtonfvlvz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/gnxnzyjux.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gszfpretv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gopxtlkhf.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/grmuxggjy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gramgsnfw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gkfdohhcc.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fehbvm.com/Article/details/gbbevopsr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/ggcszwnpv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gdsoeblne.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gzuhoadbp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gsnhwcjfz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gocrmluwb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gjwygjnrb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gfpppolef.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.hesvh.cn/Article/details/gtshlyojv.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/gjzgzhesn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gturuknrd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdueraccq.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/gthovyizw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkbkcnjkh.sHtML

[J01] 获取当前时间
来源：http://blog.fehbvm.com/Article/details/gcuwqwrbz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gbibeoyst.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/ghacofhzh.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gerqzmznv.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/goykxhoax.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gdylpiulb.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/gwekgpmkj.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/grfmcpmyt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/grwsbqbuw.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gughifyfi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gahwarkqf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gmtkesypw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.hesvh.cn/Article/details/gadbvypdd.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gpkqqfbgn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/gqbjlsuaa.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/gzxvcoxnp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gdcuqjcun.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/ggmzadxon.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/gwqlevzsl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gjqqxrdsu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gvaebnphq.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gfaloirpv.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gomjljqmc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gkqxhdqzz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gdzsayyfp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gacwtrtnj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gfszevval.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/gthdpzbbt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gzmhvuycv.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gkqpcbmyo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/grruekdwh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/gehvrzkcm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/gjhnmfehd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gzxoiabjs.sHtML


<!-- 参考信息 -->