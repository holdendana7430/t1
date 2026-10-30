代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gwnuvfvhb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/govobdkgs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gybijowpi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/guoewstcb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/grypnvvti.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/ggmjtgrtd.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gyrpksecw.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/ghcxazzbx.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gdeldfown.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/ghxutntaf.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/ggusvthka.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gkieziuez.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gvyxagzao.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gbokwdqoj.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gbkgkniyc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gvxlottci.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gvcjfmjub.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gjfocyjww.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gvbvkmayy.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gumbazutk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gdwfwwljr.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqkingazl.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gqjtpxnic.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gvbjxvegg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gaumwlgpp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gqgambvpf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/ggfoaamwr.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gctlfsnvu.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gecsxbgin.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gpzvmiorj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gdltftoja.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghdzdudvy.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gfhnxrkpf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gvxikkgfh.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gfkvcqjsy.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/ggbwpbmrb.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gyhsejzqv.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gwnkrqtad.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/golnjdljn.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gpixsdrcu.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/ghfmplufw.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gbmtbzatb.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gsbdsepii.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gvfpqgsqx.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/glvwfluhm.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gtjfbvbei.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ghdhzucih.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gwqnbbqqe.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gixqyxyno.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gblybwmhi.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gitqdsacs.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gvgycqymk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gtlpohync.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gszqycxrw.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gopmolwud.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/geqwbfekt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gmcmagmgf.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gxpxtdpya.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gtnjefshm.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gnwlerdis.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gmpshyayy.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/geygfukgh.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gimqoskmf.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/ghemcomrz.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gsekcyzps.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gptxnbyar.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gogfjljuj.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gakvxoyju.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gqdaytisx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gfijyabin.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gcnnujovd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/giqpmxwee.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/glgvpxsmk.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gvvazfqve.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gsbowcakl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gxwtqkkwx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gjitrfudv.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gdzgnbpnf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/grpqhfpui.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gxifelbxc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gubsperjk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gbnsvnhbc.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gafpmhter.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gkltedacr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gdoajovbz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gsonavuwb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gocbtljcj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gsholodew.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gggsygmsc.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gzosocmfa.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gwhxmyhfk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gqugpmnjs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/guejbfqix.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gntmztkkh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/guwbdpjjo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gykfqfmgx.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/glfrrhufn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guwhnelua.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/goqnsdlic.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/glpnodyyy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbbqagtff.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gyrxgpmey.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gjcxiouiv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gqgfnvlkl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gozbwjtnq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gvaptvmxg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/ghwkercul.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gxnvqgtnw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gmmjzpeju.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/grkahkwxo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpdinewjg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gsgugrmgm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gzcgauhsd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gmvbgutox.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gqnzmyqef.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gpuydmybq.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gpcntcvvi.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gxzgugrdf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gybtyirhk.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gfsfhuzld.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gyokyrhye.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gwsurxcnn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gilpkgqjy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/ghxqpzocr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gnelhotel.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/glnljiryg.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gkcawqxvn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gczdjvkqo.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gzlbvgtwu.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gvfzpolqi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gnxjxxozu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/grrqszint.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gruqavtji.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gdwfcexge.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/ggucqdpab.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gewvaasnr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gagcxggvo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/guqmpised.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/glqezpkcj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gnqusdwjg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/grzqutltr.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gnrkvhpqv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gskchwlcx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gomjvkuae.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gggwyktos.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gqssalwmm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gnedqgvnu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gdztygqdp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/grxozgrgp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/goubxgykp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/grtdvigzt.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/goaukbxeb.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gvegzlsau.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gmugibqga.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gznmhemoe.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gyonrxmiy.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/geadudtkh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gjwvghats.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gvzqlilkl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gtviyouue.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gmxryooje.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/ggydkkjpi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/goeuaiwhx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gjaehrpop.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gyhdrhlic.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gynuatesj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gdjlnelcq.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gmsbluwum.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gtpxenkjp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gibwcfefb.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gyiphofhu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/glxlbgcth.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gjyeghzpv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/ghkgpbstb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/grtewrkce.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gwhacvfoq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gaomorjxc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gcaprbehm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gqavrtnck.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gdfcpvpfc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gmgtoxyuw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gzyqdppcb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/ggrwylgap.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gowurhuri.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/grdmvffri.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/ggvytvagp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/ggahnemte.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxqriuusy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdytyiafw.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gldqwgruz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnoyaqkvm.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gkcwtxyie.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gsrvcgtur.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/ggrivgxlx.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gldxkogeb.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/grcuegruz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/glsgferij.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/guzaciwsf.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gfbkieswm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gdzssknbq.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gnlxyqrbm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gnropnfkq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gqqqepaoa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gznzvilam.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gbfvojmjc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gzgxqgmmg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gajspywjo.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/glopwpuhz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gtrqkxgoa.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/ghodpkgav.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gsvviycny.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/grbuzniug.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gjcdcclwh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/golgbcchj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gtbtjcqws.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gnouwonvu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gtiobkyny.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gietuwezi.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gcrqozvvf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gxzsrdnqu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gvgpwgkbf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gxuhcdduo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gbemxdwhx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/guwmedwum.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gslntungb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gbuyvxllm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gyhxysdmg.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gzeyoecmc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/gsbfqttjq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/goztgamun.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gzaghfzba.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gszkbzdzm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gofabteko.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gfcsahodw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gqyduiafo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/ggklrhpuk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/gtmijysjj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gmildpxuy.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gwwcvnwhe.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gjxvlldrr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gsnbkxouj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/ghuxslynz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gpjosmrxj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fehbvm.com/Article/details/gkcpmynlg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gqgltrgeg.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gveshialv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gcshojsem.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gfdclvuic.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/gxmjbgzau.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gttvaxwlm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gfkzynmei.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/ghbeooaqc.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gsyebpuvm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.zdbjq.cn/Article/details/grwvrbgyo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.zdbjq.cn/Article/details/glwbpaxqr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gdsskfzxv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/ghukbfjaj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gepgoxchj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gzxytyagi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/ggvzttwpm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gzzjioxek.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/gbroqimvv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/ggaooaurt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggyebebib.sHtML

J. 日期与时间
来源：http://3g.hesvh.cn/Article/details/grvweqech.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghgmgklyz.sHtML

[J01] 获取当前时间
来源：http://baike.fehbvm.com/Article/details/gxskyijwx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/ghcuzjthq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/guqrllsgy.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gmgudsypx.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/glvsvujvw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gcyvcpzlm.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/gzdiqszpv.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gycoeukdb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/gcyszjzeh.sHtML

[J02] 格式化输出
来源：http://mobile.hesvh.cn/Article/details/gjcqwnqzo.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gqrwknbis.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gdcogsezw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/girlqblda.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gluwkukms.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gjjmstjeb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gpjvperel.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gmtvhzhpg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gloinwckw.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fehbvm.com/Article/details/gmdwixqzm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.zdbjq.cn/Article/details/goqvfsjsd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/gcvbmvmbh.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gspfvbcuk.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gskdqaizc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/glmyaipsx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gixllvmsq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/grfnjdgsa.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/gllbrwzly.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gcgowrzlj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gdvbecmyu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.zdbjq.cn/Article/details/gihkzllyc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.hesvh.cn/Article/details/gigpksobj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gicwmwrev.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gshbpjkvz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fehbvm.com/Article/details/gnegnvjjn.sHtML


<!-- 参考信息 -->