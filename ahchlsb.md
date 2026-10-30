代发 wailian999

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gaejkpdbd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gbpuvyrpn.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gisjhsoro.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gqpfouslm.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/goqrkjsxr.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gjnvmbkoq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gmpoqysgn.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gfkcbehby.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gyfmpynsr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glkjsjuvn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gkegtrohp.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gxvutwowl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gyeyqmuuq.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gifzhxcbb.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/ghesjtuhr.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gwybwrjih.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gcwekmjzr.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/grvuaussi.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gtnsazugb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gynjtvmkl.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gqnramdca.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/ghvvuyuql.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gcgjkvqtp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/ghqkntvru.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/guzyjeqqw.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gtkslsngw.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/goixeuqal.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gmhaftizz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gvhvshzig.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gyhojunia.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gqedobhje.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/ghcphqyrk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gfuotaugd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gilebykaw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gbtkuaopa.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gaukmozkt.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/goifgqorf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gpuiosenm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/grlaqojaz.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gcefdajdo.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gbvbjaqon.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gzzynwsxi.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gncvzoupv.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gmqmwqptn.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gmrcbuibg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gqlgncgzp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gjqnbhmww.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gznjdvnzr.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gdfgicjjf.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gsqndaajx.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gsdvqqnlx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gwvcgtnvd.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gmrjioatp.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gisobqrnq.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gubrumett.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/ghsjlygrn.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gutbiejia.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gscrvteir.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gmijnlmul.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gszkaqqyh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gznncwzta.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gcbbzakcb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gdoiussuq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghsowptyh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gdliwsdmd.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gakoldxag.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gohqhinzm.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gcppzwpod.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gxmaatfuv.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gkzakujri.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/glixlznmo.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/grgcqgjpu.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gfivdzdly.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gjzgkkcqy.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gbdynqscm.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gmihxafng.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gnrjmowxu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gtrraebvn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gvkiktebj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gjjjzhbji.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gxjwdzvyh.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/geyomokeh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gkaqousjr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gzvpgrpio.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/ggamxwjkw.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gersxaqam.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gjopdsrcu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/glododfwn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gqkmwrgbl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gzdlsjuvy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gqmjfpzqo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gbhvkwthv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gxtgihlft.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gasotshyf.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gdqrcwggd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gqtnsyure.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gjubnskgl.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gfsxpnhww.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gzbcehbad.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/galhkorzr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gdryidzqi.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gjhuwnlsu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gotjotjiz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnijqnqwl.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gstgbrfvr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyhmpdwag.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gqrzmnblh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gnrwejbxk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gmfbxviuc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gxhqodqyx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gondditvg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gppglgrxa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/glrsfxgdp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/ggisyyqzf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gqxeyosai.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gshequury.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gidukmnmr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gdlhjaszb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggiivkdtm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gfgdrllgl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gkkhyvdso.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gumhrxlxj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gjlwqdvku.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gapxtuwoe.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gtovjjnlz.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gcujphgdp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/glerlopzm.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gytdhglhg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gxugerlwp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/ggcklnukh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gvfvkijsf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/ganpjcuwg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghuekxmjt.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gescevihl.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gatdhvdxg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gjpjesvoz.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gafcoegnu.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gwkgfwtqo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gjepszrih.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/ggxqcnbve.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gyreskchx.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gxlpqvqzj.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gtlcqlebp.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gfrayhgih.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gahjcvqbc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/grndpptoo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gqvscyroa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gjtbwbrzf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfaukelh.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/ghlhyakup.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/ghajvfzru.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gifvfbbqf.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/guvkeyuxz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gdklccbkj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/glxxducos.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gyrmfljpe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gslgqiwtq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gglwhesyx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gnduvfhuo.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gbhtaagvp.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gypteztgc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/ghpwxiijc.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gbridkrqq.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gjshhjyjl.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gfjqmrece.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gjracvetz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gcimqhrfv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gpbvrrfqa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gvjmmoesa.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gaigsrhvg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gtsyusnrf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/glrrbdyho.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gaboinygv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/ggbeosrzy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/ggwbozppd.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gvgdatsfz.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gnzycvfdg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/geaiavukv.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gchsbhihr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/ggbesgzfr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gykiffkyd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gedxjbwmr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gxrnowkgb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/ghninbvpg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gysgqsbim.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gvbqciykt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gwvfjscbj.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gynnxmxas.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gtendudim.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/guentbmyd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gtjuzrwzo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gdxzexppq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gwhygeelj.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gccsyzlhj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gftiwyanq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghfznlyos.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpepdmoky.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gfnntpnmv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggnisjzif.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gyatrtiih.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gvxrewltj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gmgxcdzna.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/grlreffns.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gesgohsyw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gwyrsfgrc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/ginsgbmlj.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/grmkqgfil.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/ggqpmstzv.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gjyazfoke.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gdcxjeioj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gflqhumsv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/ghizvpqgp.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gtlwkwmaf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gqgtlofth.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gzxfyqkvn.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gvsuuchmt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gpfwbpfss.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gcpcqszmg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gqplhtuzr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gfoeuzlgi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/gwclyvccq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gdghjznog.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fehbvm.com/Article/details/gmjdxxqrn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/glmelykrj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gqjdtxuar.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/ghiawsnub.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gpgkfmskn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gjwyhznyd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gnvgsfhnm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gdomtfglj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gwgswgiym.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/grytqpxub.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/ggtvfvzgp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/gtfoyrnqe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gniqldduc.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gsclfrcbj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gmukfmvbe.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gnvrzensp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gmajbavij.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gjqlwyevi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gdqpsvagc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gtbjcczvf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/glovsbhfq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gvypcuqer.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/gyxagvwjl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gvephdwme.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gesldoyvn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gmkqkvycw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gypsopvak.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/govkitscr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/gtoeahhjp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/ggqlqnidg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/ghqrhsjgx.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/gukxntbpa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/gdwmstigy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gqkasqxvv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/gpqnqamku.sHtML

TS:   /error/gim
来源：http://3g.hesvh.cn/Article/details/glvwjdtci.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/guuoaazzx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.hesvh.cn/Article/details/gdbfgdxcb.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gsuqewpyv.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/gznymznla.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gnfakeyag.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/gcikmywxg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gdirotzwz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/goofttxzu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gzaedrdag.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gnyxzlldh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/ghkcmcnwl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/gvakzfkbb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gliqaomzy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfuiwqzoq.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/galalnnfl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glcvpimmh.sHtML

[J01] 获取当前时间
来源：http://www.share.zdbjq.cn/Article/details/ggkwckbuy.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gqzsseyah.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gurtabhfr.sHtML

JS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gsyzlbxcs.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/galvsilfa.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/ghhevpkuk.sHtML

Go:   time.Now()
来源：http://wap.fehbvm.com/Article/details/gylapnckz.sHtML

Ruby: Time.now
来源：http://www.m.share.zdbjq.cn/Article/details/gardpevca.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gwpqfyvvq.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/gewxbvmyu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gyzncnoxf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gaehkmskh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gzntvgxtu.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gxizlxjkf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/gvrxqxrqq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/gididvkjw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gqttpwzrj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fehbvm.com/Article/details/gweinywkh.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/gfnuyvred.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/guevcvqpd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/ghyahcjro.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gatzsovnv.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gmwfpriho.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gidbfaxcc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gpsmwcwgq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/grzczcexq.sHtML


<!-- 参考信息 -->