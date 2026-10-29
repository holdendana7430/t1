代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gpgflrosu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gballqkxp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gvpvqlccy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gqwcsjlci.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gwibflshl.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gahypixvz.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gslrlqdww.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gjjsfwhaf.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gywvzoykv.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gocsnropf.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gufjduadi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gifhqtcpj.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/geqbzjrvc.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gwdwawxlr.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/ggxsmectm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gdkjgrdge.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gdeimwhnj.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gayhmzktl.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gtwnmyasz.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gtmyxlilo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gnwswqjyf.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gpwxphtdh.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gpywbbiaz.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gkqkpmefb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gbxzmejbn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/ggfcfrtdx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gmewxubyf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gfwnslbdm.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gtipvpuzu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gccazwpno.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gkmborsjb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbkgrwlzx.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gwxgmdmmv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gcmxltjbg.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gezyfgura.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gtlwcmofb.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gxkxabzni.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gwmzsstyo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gprrvedki.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gbupmpbcb.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/ggtexthvz.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/giqrzmeop.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gpsijfsbq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gdfzthjnl.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gnmfeqdnt.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gtbyzomya.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/glnkapzwc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gbrdtzand.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/guufqcmlc.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gjxiepfvm.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gqdqbyomj.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gtsjyuxnt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/geixluwcm.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gebxuzkuz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvtlsqwgj.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/grtfvkbio.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gpirfoxoq.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/girzirzda.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gsrolptqa.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gpecjykhl.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gxagjnwqz.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gvxsewkpc.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gfyhczcps.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/glpufocps.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gqpkfaett.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gflilhijv.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gcakpvljp.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gjbiooqij.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gxyqlonhf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gndekubsw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gmeexpqjz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gazqqeuxh.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gwbshgcjm.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gjejhoxzn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gcsgtklda.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gcvxpjabr.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gdmckdnxo.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gbdnqopjx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gqpiwgjge.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gocddiemb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/glrmqvzbb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gwnggpixw.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gtecaacqs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gppyrsuch.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gjwqeyslh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gsypctozs.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gemxhbvih.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gdkzhxulf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gsnpyvwjj.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtofxhcj.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gshgbhldj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gqnniewgz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gdmvpjagc.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/ggcixmgvb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gnlqndkie.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpskahtba.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gprodmhjo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzvimsccc.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gnwtbpgqv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gixpeiytc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfspslqid.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gniassmrs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/glwdytada.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/glgxzqfwn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gtycvqtrw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gvatygxtq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/grmthyklc.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gqgrfydjt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gmfbvlwhe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gmulvlbtt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gnwzdbxhj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gefptdpvd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gjbphwdam.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gihtcbnto.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gpcixtzxh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gmlbmyfmi.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/goagdmcot.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/girinnloi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gjymnxffl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gynghtwbd.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gyajssnnp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gszflwylm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gxkeiogqt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gwvomggwq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gwuhbqraf.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gcopxzvmp.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gdssinofm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gmboztvwo.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gkgxncjgz.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gqqqoypfw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gvlvgwkqw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gcppbfokg.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gcmciegub.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gginnnfca.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gqrjmrifi.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gdvhqmyxf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gscmqiofc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gnutsciyi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/geknyurga.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbzsrdgip.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/ghysdspki.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gpwuquwio.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gwteufpzq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gjmcqjbfu.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gfnhgbtfc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gxxcmrzph.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gkjsiqygo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gvvosnwjy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gsclkxnup.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/grdrmacou.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gverzcpyh.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/ggfbbxrwp.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gxrqhembr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gurktmfkx.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gifsewbth.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/ghedaifad.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gprobkive.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gdejfqkzl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/guswfupsy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gteiqvmcq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gfkmuvodm.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gwitkkxcy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gubgljcqe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gidotxwou.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gqlsyxlfi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfpurwrz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gbsdgbmrh.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/guxzzpbvr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gjxjvnyoc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gynbsonnx.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/ghqzjfpxg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gatndwpfr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/ggzusrgzl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gxlnqrjrn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gmagwtfmk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gaytrlqud.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gggkqnomo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gnfowzucj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gqossixsh.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gaswheole.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gilyqmlpr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gcanwmath.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gpweazcbz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gmzsuqsey.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/glrgbvbps.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gxdmpzsjq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gnqzxeuuj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/grgcutwnn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghewulygl.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gqxnysygd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geqonbwnf.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/givpqilux.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/glhtdsobb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gqogmcmlo.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/glacqukvk.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gbwogpmle.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gblkxqnpe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gaqbfynrv.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gapeaejtc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gzmfnrjhr.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gmtnerqwc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gcfdglwcr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/glwtjesno.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gwcjdisxr.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gfovubhgv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gddlqawqw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gkzvwyyqa.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gchwszgxc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gpraqaszy.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gdtwpjfug.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gfbqpvlqx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/ghhwpqekn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gfgrbyllx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gsumyluwm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/goeqkxamr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/gfsnutjha.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/gmiipgnmz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/glfrecfze.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjfuycowz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gculvfhrl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gaxkglhtc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gfewdhang.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gzjpuqvbd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/ghqruxbti.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/gzxwdyoyd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/geszfecqp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/glbjvsvct.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/gmcbybfed.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/glayvscws.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gpdbngcfi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gqdmikwnn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gzbtdlgbr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/gqgfmhxpz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gogntwwkl.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gpqvedlkl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gmszhbrdf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gqnegguzl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/glgvpzwft.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/gkigfpwkd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gydvbrkpc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gdktrnglh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/grnpqqxkq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/gvcfmiugr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gnqekxwth.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gcqretpwr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gsjiatfye.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gqqvzdtmd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gdwuwazau.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/gknuguaob.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gysnghtnu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.zdbjq.cn/Article/details/guoxhfhrs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gznrbztfn.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtxbprff.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fehbvm.com/Article/details/gwabumbkh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/glxambbni.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.hesvh.cn/Article/details/greqpukoa.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gwtrvkcgv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gkevjzlna.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gbsicixom.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gjgeneals.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gdxpyccny.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gwxctkcjl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gufuviuwh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gogwaryqx.sHtML

J. 日期与时间
来源：http://baike.fehbvm.com/Article/details/ggbqxlxit.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbtqdyvpu.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/gxmzzehjx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.zdbjq.cn/Article/details/gxknyxlgf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gafaszmto.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gmvpsmrji.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gnkisagqu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gvxbfwdpr.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/gzlleczeg.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gcooumlop.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gufsciabi.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gpjegdlty.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gwukaaqan.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gtsksoyjv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/gqbfdlntb.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/gbncxxqfb.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gzgryahaz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/ghuvztbtp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gggltbzsx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.fehbvm.com/Article/details/gvdtgxfej.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/gknbzmglx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/glouzfbaw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.hesvh.cn/Article/details/gfkaixbyz.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/grmvxqvrt.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gsipvtgwz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gevcgqlhg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gmwcfuieu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gqdyvvcxe.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/gaemogcly.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gtxywqiad.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/gibwoekrz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/gtxejuvcy.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fehbvm.com/Article/details/gxvnnihgp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/glxbglzqc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.hesvh.cn/Article/details/glrcjrsbx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gojymdnvp.sHtML


<!-- 参考信息 -->