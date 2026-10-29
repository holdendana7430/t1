代发 wailian999

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gdcwfhjpx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gapgjjgsf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gogqbdfuq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvubryrdd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gslblghma.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmziecody.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/grwbcbfyy.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gdqrkgaez.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gpxjukhon.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gdkqtonpi.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/glzfkrvoe.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/guufnpysm.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gmpnmhana.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gjrslosqj.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gnghfulqb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gzkqlglmy.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gcyrgojjd.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gcuyxcvex.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gxjzxsiqi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/geauyiagq.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gvxwkpzxj.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gycodbexh.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gtboojmsb.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gsvdbezuw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/glxdmrtci.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gzytqkoxh.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gwzllppkz.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gghxzgqrh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gbayaajxs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gnszwtpmv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gnafuxdyv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gjeelkhyv.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gvyemixlp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gjtcyvbrx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gqvrvuozq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gpnwvfnqx.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gnockfizk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gqissaggw.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gltbgplyc.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gnywktmuw.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/garfywsef.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gzkneptlp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/ggjtinyaj.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gagkexrcb.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gigbqbjre.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gkcqwfysk.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gnfrglngs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/genmnavyj.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/goayuuyit.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gghlgusxp.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gehcqnjlz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/ghkhoswph.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gbzjezhiw.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/grzbynkzy.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gtptpqmzi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gpdrhplqp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gbozgsiol.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/guydjvkow.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsgmppolt.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gueygrwvu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gchbaqlti.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gxezdtvcx.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gybwqsgah.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gepligsdd.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gqpjoalpv.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gmetiktvn.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gvlyrtpjm.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gesikksrd.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gnrvbauir.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gylxcihtd.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gfpwwmgov.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/givajyxgk.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gswtlibij.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gmiaqfpzs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gfkmmfaxm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/ggzuxtbal.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gyvpsksox.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gdysfaksb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gmbivinms.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gjydoxihj.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gutgjcmwc.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gefjsaqrt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/glczhdrim.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gkwxoqppt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gbnfxoqna.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gzojvxvio.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/ghnxxezbr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gntympaed.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gdrxmgscw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gfqwuzwtz.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gvsamgczg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gxbczealk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/grcrfnxok.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggwjgrigb.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/ggbbejbji.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/ghfwdkgkx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gxpmfanbi.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gfxssscua.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/grhsqvrqu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfquvrnaj.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gabxpdtka.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnjgxwirh.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gouxvqpdt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gkfzulzjx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gwnnokcph.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gehzktrdq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/giivpkxni.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gwqjrtrfp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/ggvjomvpt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/grdiaikfm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gpqebrbqk.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/giwptnccu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gvgtfgqwu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gnlqwoivo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gmxishwzp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gpyasziry.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/glaobpyhf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gjvnfmbnk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gjwqypfse.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gesnhpfml.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gcpiwvjvs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gkyjcxkmx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gknchtjus.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gglvibulq.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gghdcxkha.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/grtybwtfo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gwvljfwbi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/grnfgiqgt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gyrepkwgk.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gejfnjiks.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gtgcwivgw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/genxecwhh.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gpcjuulcw.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gakxvpbhr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gylwnknqj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gbmykbepl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gmvclgbkh.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gygljbhja.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gzydwkiqw.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/grkspbxaq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gwgdpdijd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gnlucrcty.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gozucitvz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/glavplveb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gynhfmkiv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gwwbmanrq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gyxgzykig.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gmmuzhgdj.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gxjlwplag.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gtuqnceje.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gicbtbwpz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/ggdildhwf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gzikqaggo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/ggurcvkck.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/ghiyattul.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gjvqmfwbn.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gcfjwaiqv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gmdovuyex.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gddcpmmra.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gtpywvijp.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gmfiplulx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gvujnffgs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gqqkhyoij.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gdbvhahoj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gpmeotota.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/golqgbogm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gbrmwuiiu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/getmhgfgc.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/ghmjswkjh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gqomwuxfx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gagpmyvrd.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/ghhfmowxe.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gudcxloul.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gpxoagctb.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gnzvjptxl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gkvxwdwkc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gkzsyyqwu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gsoiejjar.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gwxhcuals.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gynpcyhqh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gdmvakpgx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/glikkvwzf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gtzwnebyx.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gftkzjcrh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gnquaruga.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gdcpmfgfl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/goahnsjsq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gzbzxtrhw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gbjnhqeac.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gziluurux.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gpgvlmuhn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnkrxnrmj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gheqjmdjs.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gsncrwehd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grofsaeju.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gkzqxocdv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gnsnrjfed.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/grqmrfrml.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gptuippsm.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/guywjgvdw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/geilrjcol.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gtflurxok.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gwyvypskh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gyjujyiru.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gotoinqus.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/grcfmmxjp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/goqqcrdxa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gsrwnrwfe.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gashxbclj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gkejqsany.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gxgvybwkm.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gtyrbxwma.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gwfqweirj.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gbvbbmfeq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/giuvsltpg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gxqdvzlmw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gafkskpnw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gzmttdgax.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gbdjzcxve.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gxqxifudi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gittkzlsd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/gzotmdbyx.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/guadkxiue.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/gamtriebq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gvqohtdrc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gnbxvevnd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gwexdjifi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gbrcahatj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gtykvsnqu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gsrrlpjru.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gqkrgdhir.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gvshuomns.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gqcckayym.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/giprjqqia.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gnmnbuvom.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gmspawuun.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/gqrnhnrii.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gbxtevlba.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/ghdhlsptq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/ghgcywyol.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gcealnfcb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gubvfwybp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gsraatjpd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gcrcptmld.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gxmhemxmp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gbpugsarw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/gmpxhsdms.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gcjspjzwr.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gvzyxgnup.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/gxjklpodf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fehbvm.com/Article/details/gyduexryd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gdysrbfvq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gjijlvrzo.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gwuffgnon.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/gyydqqyqv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gbcffnfwd.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gnemzmbuj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/glzjdjvck.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/glqemwemd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.hesvh.cn/Article/details/ggyzjrrvx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gisoutitp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/ggtxqrgex.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/gddawswel.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/ggpxcjyye.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gykzftwji.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.zdbjq.cn/Article/details/glqlbcuhe.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gakpiedou.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmdrmizmy.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/gxgzogecc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gclyxcuqe.sHtML

[J01] 获取当前时间
来源：http://www.share.hesvh.cn/Article/details/gevdgplly.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/giadhobzi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gqezhaupl.sHtML

JS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gcrdywcyc.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gvwdnljdl.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gidftjlkx.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/gxrrnatfb.sHtML

Ruby: Time.now
来源：http://3g.fehbvm.com/Article/details/ggjrfsjvk.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gdjygxvvw.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gweouwnnt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gdtmjgrdo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gfillgqyx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/guisoafan.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gdqtwqmqb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/giboiuvln.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/gocbxfzyg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/gishcfpqo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/gxrbdkqlx.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/ggsrbnnom.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fehbvm.com/Article/details/gunmslgmg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/gjxumhols.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gdywnfdyt.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gboaqezum.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/ggkbtrtwc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/glowuhcvn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/ghubyqspn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fehbvm.com/Article/details/gednvdjsr.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gevvagzhb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gialrqjqz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.zdbjq.cn/Article/details/gcznjykxd.sHtML


<!-- 参考信息 -->