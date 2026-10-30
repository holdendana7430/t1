代发 wailian999

PHP:  public static function f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbvknedq.sHtML

JS:   static f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhiluiut.sHtML

TS:   static f(): void {}
来源：http://wap.fanxiaobao.xyz/Article/details/gihexuokb.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggbfkbdnt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gedbcegfw.sHtML

Ruby: def self.f; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobofndfo.sHtML

C#:   public static void F() {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghagiqxpi.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmzlyeiz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvujefce.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gofmarpfm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fanxiaobao.xyz/Article/details/gizvqaulr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstxojnwg.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gusiijbty.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fanxiaobao.xyz/Article/details/gbnlkcfqp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ggofdhiak.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcvgzaso.sHtML

[G10] 访问控制
来源：http://wap.fanxiaobao.xyz/Article/details/gmknzvauq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfygrbey.sHtML

PHP:  public / protected / private
来源：http://baike.fanxiaobao.xyz/Article/details/guxgczhyx.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fanxiaobao.xyz/Article/details/ggdyxleel.sHtML

TS:   public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwekqxxu.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fanxiaobao.xyz/Article/details/gvtutffzq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fanxiaobao.xyz/Article/details/ggmconhsg.sHtML

Ruby: public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gpsxwmjli.sHtML

C#:   public / protected / private / internal
来源：http://blog.fanxiaobao.xyz/Article/details/ghpdzmbtx.sHtML

[G11] getter / setter
来源：http://3g.fanxiaobao.xyz/Article/details/gyuyjzpad.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gzoduodoz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxluopnyv.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxtkejydp.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkrpmsaoz.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjvcrkde.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/govyhhnye.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garodxftz.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdogfskrm.sHtML

[G12] 对象转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjcyhrab.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fanxiaobao.xyz/Article/details/gtfrupbgv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gihdstoap.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gebtbhwks.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjenlfsky.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmqnrorqm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gscwqmnnx.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gujfwwqqm.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcybsatf.sHtML

[G13] 判断对象类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzchdnbc.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmdpkfes.sHtML

PHP:  $u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gelbphiog.sHtML

JS:   u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqyuwnxm.sHtML

TS:   u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcknhsezg.sHtML

Java: u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gnalpttjh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiokvglg.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fanxiaobao.xyz/Article/details/gxjpwukgn.sHtML

C#:   u is User
来源：http://wap.fanxiaobao.xyz/Article/details/gipllgppu.sHtML

[G14] 数据类 / record
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugcpxllz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fanxiaobao.xyz/Article/details/gwhbxuzzg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsgjpjxc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fanxiaobao.xyz/Article/details/gegrnmqxq.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fanxiaobao.xyz/Article/details/gutxzoicp.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gctxhlmwf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvacsynu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fanxiaobao.xyz/Article/details/gcijwtjeb.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fanxiaobao.xyz/Article/details/gafuwtazu.sHtML

[G15] 枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijctnapw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqvbvgbg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmyiiktc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmdpujyw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gghgouvcr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpwykoja.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fanxiaobao.xyz/Article/details/gpnyrdkoj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fanxiaobao.xyz/Article/details/gieedmahy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gswoubuyg.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fanxiaobao.xyz/Article/details/ghuragylm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkafgovc.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fanxiaobao.xyz/Article/details/gwbeiyypd.sHtML

JS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gdzsmzmfx.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeeecbjy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdhfrcda.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fanxiaobao.xyz/Article/details/gigcekhhm.sHtML

Ruby: obj.instance_variables
来源：http://3g.fanxiaobao.xyz/Article/details/gjsvzuchh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/gpkptdfuf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjutealno.sHtML

H. 异常与错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gebabkvju.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhvxbrfe.sHtML

[H01] try / catch 基础
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpgokibk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpzowxsb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmblsdik.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gisgnntwp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjckmsvuf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxpwchdo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykzqxjbl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gasxolaqk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjwbyljj.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fanxiaobao.xyz/Article/details/gagvmvfkl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdslvekgo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gshkyhpcr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzlczuwv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaikqitn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gydctuazz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fanxiaobao.xyz/Article/details/guvbktqdu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnoqfaut.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghdzadpiv.sHtML

[H03] 主动抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gbpgfliyp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqgsurdo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxanoaiht.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwglvwzjc.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gfueefpzl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gvpdsfxup.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgljimoj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fanxiaobao.xyz/Article/details/grbdydctw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjbjtasq.sHtML

[H04] 自定义异常类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqjyxaex.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fanxiaobao.xyz/Article/details/gbpjhzesx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fanxiaobao.xyz/Article/details/geisizsds.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpvjmboe.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmwahvgtz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gffxyxbsc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fanxiaobao.xyz/Article/details/gwtkgbohm.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gywylsaxi.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggprnueyd.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnptynoyo.sHtML

Py:   except ValueError as e:
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlbkvkhb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gntdlpzad.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzwsdeeoi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gefyytjnk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtilihix.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fanxiaobao.xyz/Article/details/gventiqtm.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnhlnugh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkwyrmyv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvpcmqik.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fanxiaobao.xyz/Article/details/gsovixelq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/gdndhbvgt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyphhfss.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeyspiuq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fanxiaobao.xyz/Article/details/gdfmbhghl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fanxiaobao.xyz/Article/details/ghndylwbh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fanxiaobao.xyz/Article/details/gfuhvtuwl.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/goqbmtaus.sHtML

[H07] 断言
来源：http://3g.fanxiaobao.xyz/Article/details/gzpsnctvn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fanxiaobao.xyz/Article/details/gahalpkyk.sHtML

PHP:  assert($x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gaymjmhfl.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gzpzaqlzi.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gkzonecmf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fanxiaobao.xyz/Article/details/gsaedpjjk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpsxjztd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpcucxlh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxztzmzip.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gufleempf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuawptzx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmqvifcb.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fanxiaobao.xyz/Article/details/gaujceoyj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieyfrttl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbstvkaqo.sHtML

Go:   err.Error()
来源：http://baike.fanxiaobao.xyz/Article/details/gtjbsgyuy.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fanxiaobao.xyz/Article/details/grrxqgnwo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fanxiaobao.xyz/Article/details/geqzdwajc.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gombosfqz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fanxiaobao.xyz/Article/details/gxulxrgig.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gdshapize.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fanxiaobao.xyz/Article/details/geypcctty.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fanxiaobao.xyz/Article/details/gvnagxueb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggoeghqta.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzihiikq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fanxiaobao.xyz/Article/details/gztelzain.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fanxiaobao.xyz/Article/details/gdnnuobwn.sHtML

[H10] 资源自动释放
来源：http://wap.fanxiaobao.xyz/Article/details/govcfodle.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fanxiaobao.xyz/Article/details/gomghfktu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxzitveh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/gsaqvrrzw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fanxiaobao.xyz/Article/details/gfozyuxht.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fanxiaobao.xyz/Article/details/gtljuybeo.sHtML

Go:   defer f.Close()
来源：http://baike.fanxiaobao.xyz/Article/details/gxvjelkqq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrwoohrf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gufmzqyni.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxupolziy.sHtML

I. 正则表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuvmegzc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhaoffea.sHtML

[I01] 判断是否匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuluolwg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gfbuyqnez.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gnzvfhcmf.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gwbacxclq.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gkjdizdpk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fanxiaobao.xyz/Article/details/gjyskneut.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzbjjjuf.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkzxwnem.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gddcuwjgv.sHtML

[I02] 提取所有匹配
来源：http://blog.fanxiaobao.xyz/Article/details/guzfvvvia.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwlibnxt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqsameli.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxvsupnf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqtuefkw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gxgfwgsqt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gnxjbbxcl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlgcptvp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/ghshevqak.sHtML

[I03] 提取捕获分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgwzaoxc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwyxumgb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpegunlv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gqckgxmrj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gvtsdvopr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqusddiwq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fanxiaobao.xyz/Article/details/gclbfhfqx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gjymaqxom.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxqpeqmf.sHtML

[I04] 正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gkgzmeabf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghflgjnzw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/grethwqwc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gnkcwrvet.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlmqboqb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/glcdqrkkx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/goqprrndi.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbgudnrl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fanxiaobao.xyz/Article/details/glggkafva.sHtML

[I05] 按正则拆分
来源：http://blog.fanxiaobao.xyz/Article/details/gqeirwtwa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwayccct.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsvoxdrk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/gkzangwpp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpzzrukx.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/ggitxtyvi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fanxiaobao.xyz/Article/details/goolvpmpp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gzovxjqhc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnlrtstq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpspbuoop.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/grvdfcajm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsrrpqyj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/gbrvfxyhj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fanxiaobao.xyz/Article/details/gjthbjhcu.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gznaxdweh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fanxiaobao.xyz/Article/details/gnwfvpmnf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fanxiaobao.xyz/Article/details/gszapcmlt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbcngxek.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlkovbvh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstpkgryh.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/gkwdnwyix.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifbawvon.sHtML

TS:   /error/gim
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtawsfwof.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fanxiaobao.xyz/Article/details/gsghnadhx.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwmfqreu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddzeozbz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fanxiaobao.xyz/Article/details/glctshtrq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fanxiaobao.xyz/Article/details/geutvjqwg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdfsfyps.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghehmonho.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gwmldqbqk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gyejqtefv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgcimait.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fanxiaobao.xyz/Article/details/gqtmsllmb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fanxiaobao.xyz/Article/details/gbfsvonwb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuirivcv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygkckxpc.sHtML

J. 日期与时间
来源：http://blog.fanxiaobao.xyz/Article/details/gpzneqwtr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdsdzfowv.sHtML

[J01] 获取当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrtwbmyn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxqhbazf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkxkcjzw.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gootefuvu.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqiynwiy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnldrfmnm.sHtML

Go:   time.Now()
来源：http://wap.fanxiaobao.xyz/Article/details/gvswodvwa.sHtML

Ruby: Time.now
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnzpaywa.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fanxiaobao.xyz/Article/details/glulcvqas.sHtML

[J02] 格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gksrsmjkb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fanxiaobao.xyz/Article/details/gdgptutxz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgvlensk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fanxiaobao.xyz/Article/details/gqxcpohlb.sHtML

TS:   d.toISOString()
来源：http://wap.fanxiaobao.xyz/Article/details/glhodvxtm.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fanxiaobao.xyz/Article/details/gbrrxvkhk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fanxiaobao.xyz/Article/details/gpcudlfdq.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqazegnje.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzlmxmmb.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzwhfsmh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpkqbkaw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fanxiaobao.xyz/Article/details/ghhlandtr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtzylisx.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjuyranj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gujrxnvlt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybnqdrja.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gltbpybba.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrnvnsqv.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fanxiaobao.xyz/Article/details/gtqwrrwhk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golkioqfw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fanxiaobao.xyz/Article/details/gurxszelp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/gmdjzrwgf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuxsyfwd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/glwmkzgof.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxthmzpoy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmqublsn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/ggbrzttri.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdhapbix.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fanxiaobao.xyz/Article/details/gbwzkbwpp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fanxiaobao.xyz/Article/details/gvdzbgxjf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmkktskz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonzrrcub.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gajubljut.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjhtbzbd.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fanxiaobao.xyz/Article/details/gmnaiuoke.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/grinmkvgv.sHtML

[J06] 计算两时间之差
来源：http://3g.fanxiaobao.xyz/Article/details/grjmcmvxx.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fanxiaobao.xyz/Article/details/grachljbp.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fanxiaobao.xyz/Article/details/gwufqzmfb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fanxiaobao.xyz/Article/details/gadbtvkjs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktyyplso.sHtML


<!-- 参考信息 -->