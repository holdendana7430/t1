代发 wailian999

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gemqarpaa.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gcixajlli.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gvyukcpab.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gkayjjjhz.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gpxlzkxcl.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gcruoitgi.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gfjnuirgl.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gesmeymtv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/grvxkpnma.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gmnksqkqy.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gosfjjuqt.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gdmvhdumn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gdaouppdp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gnwnawdxs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/ggbeiwdym.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gophxayru.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gkwphxajh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gqnylcpde.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/guuqmbuum.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/ghbwumlcw.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/ggdvxlywm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gtzjosahn.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/ggfibngju.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gqwujlgbi.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gijbtkitw.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gicnfweol.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gwrswlkde.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ggljhlugs.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/goxtrwlfi.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/giovdmlsb.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gufytvglt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gpkjvxgtb.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gcivpdmyq.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/ghtmqmkcq.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gdulyzhnz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gikerqihs.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gqzpynqtb.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gvnsoxvuz.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gremqgrxx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gmrmqhlli.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gprppexss.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gdzilnbxw.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gdkguvhvk.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gfezacnbk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ggmqlpggc.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gjxwbyrfx.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gwsdrgnza.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/ggfdekbnx.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gigwpyxya.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ghfnjnios.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gtiwumlev.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/ghjxuccgq.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gbutzentm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/ggkjhcrtt.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gcwujwdos.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gevpeoqwa.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gcbiyeikw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/goheraorq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gojffojon.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gtjfsdyjl.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gkivizlha.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gupcqyvty.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gwtrlcrzc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gzfmqqqwm.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gkpumjlsd.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gpqgedekh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gguclvgaj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gxugwyjuw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gbkodnwkz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwaikcwbl.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gmisfjvyt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gultscqkc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gezqzzijy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/glmpijmzx.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/guoyxnmdn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gmjvviryw.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gcxtcwqcm.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqksqgtvb.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gvtuluyqs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/ggewqgibg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gktxogrxh.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gfutksbdh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/giuthorhk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gobhfvnkx.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gsauvfmtj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvwdhydeu.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gbkohsqeh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gcitiumak.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gdynhnblv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gtkslxcdh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gvpcrhrsa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gdmifkhrk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gibhjevrt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gqtiwwgtd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/grudwyilh.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gceamdoom.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gyyepirfr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/glzcgtbsv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gewzczego.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gkbqtykzt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gayvsrgqh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gpxdrsson.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gsqmfuvnk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ghznkqijm.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gsvcaqfco.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gyqiafubc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gnptpslje.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gqeniiknp.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/grzjipqvl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/ggvsfcsjb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gmeiovpov.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gwvbtysim.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gqrzifuam.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/glwbqkkwv.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gjmxrbydo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/ggnsmccyf.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gvpaxmheo.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/glslkmhpx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gwzpfhevn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gkjhcbrzk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggdrmzcpx.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gsrhsgski.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gkihmorwg.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gdfpckmny.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gzxdrukho.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gatqluqsi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gpuptdudk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gqyrqgvyf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gzuwzxolc.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gzdbmtfzl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/germgjnnh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gpsfsjiac.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gzmntdrcy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gokzqpbgj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gfkxpthoe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gjeodmzua.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gwipmlhox.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gbwuoysfk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gpmhwrjzg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gxxfdbzpp.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gdiybqrzi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gyukxvwjq.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/giuzxjiym.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gvzbibegf.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/ggubsbpql.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gblosyhms.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gcggvqyid.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gwgcivsvo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gvlrhelna.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gwuvsghmj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gbrtsysjo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/goortjgzk.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gyyiszndk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/grrvdjbjw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gnlnbrcan.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gdjecirvd.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gmjgtvyfm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gghjbseva.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gkrbucqob.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gsisgpiht.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/guqjzfyer.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/ghawghkre.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/guanuoayr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gmatnaqwf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gfaxzdxjr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gpjcsobus.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gmpzwmupk.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gaouuutsa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gmeoqwane.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gleffgitv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gnhvnmmnd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/ghhstgrgk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/glnlhpzuv.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gdtlulecn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gvrveyylp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gezareeqp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gblhhkhlc.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gmpryqgsj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcjuvhdnb.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/guuyrpwbu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gukqtdeno.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/grtkxhean.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gmaxbmtlt.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gbmydizul.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/ggxjngcgw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcznepgwm.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/ggevdcwgc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/guffadoxq.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gpmepltpd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gphgiqkuq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gcmbxtamm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gdjetzucm.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/ggmzkbqfn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqfzblkqr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gvnvtclfc.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gdwlyfvqb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/guvmseoxq.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/ggkovgdfe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/ggbgzoyfu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gtuozfpmw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gziajpxkh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gnxzsevnw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gkrkumanf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gzuseetuo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gmltasnch.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gdsanpstv.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/gkuhyxhdd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gznphbtsd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/guewwmnmf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gumllyapi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gubfhxklc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gcelnhfbi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/gagqvdobw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/gfcyjgeqf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gcoupubch.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gjjxtkhbx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gipuixwqt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gxhdzgagy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjyxzqsx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/grpltmhoj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/ggixdcrxe.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gopriggto.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gndujkadb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gwjwztjdq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/galnzlnii.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gdzhyezga.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gjstbhnbp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gdbccswnj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/guogabwyi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gicpjhjih.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/gkjqoxlpm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fehbvm.com/Article/details/gnrjusqsh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/glxygvnie.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gvqurhyaw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/ghdnxhffi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gcolrejir.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.hesvh.cn/Article/details/gjvsyrehb.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/gwazpvysd.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gbunhtzmm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.hesvh.cn/Article/details/gefqcqsiu.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.hesvh.cn/Article/details/guevrfydt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.zdbjq.cn/Article/details/gtkxbwkid.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fehbvm.com/Article/details/ggyygldnw.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gyewapqya.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gkuqmhisz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gbtlctelm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gimehfrkn.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gilgztvtd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/gcntuizqj.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gtcsgmgja.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gimgrznvq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbavhfaol.sHtML

J. 日期与时间
来源：http://www.blog.hesvh.cn/Article/details/gyirxpumz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnibqwjkh.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/geoawfmzn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gzzimlxdb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/gdivdvndc.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gtgvxxjdn.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gsscydjcn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/gxmybpbtj.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/gbeyewdwx.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gcggrimhf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/ggtbffofz.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/gdhzvnujq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gcvojsgzq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gxihpvioz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/gugypktsc.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gsnvbzxrp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/gjutjifxm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.hesvh.cn/Article/details/gulocdgjj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gpzlfmdhq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gujaqmwip.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/gqqpkkqoo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/guizjyqhp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/gcgtafsba.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gexjbmrlh.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gcbymyfoq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gdquzxytp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/ggpeafuxv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gejepofmk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gqxrrpkfc.sHtML

[J04] 时间戳与日期互转
来源：http://baike.zdbjq.cn/Article/details/gnmertyjy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.hesvh.cn/Article/details/gbmfdlhgw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.hesvh.cn/Article/details/gulwmxrgj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.zdbjq.cn/Article/details/geqnqjibx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gjxngzjff.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gekjfipbq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gupshyghl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/golubcbxy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gavfbeqno.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gfgebghuv.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fehbvm.com/Article/details/gbnhltmqr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.zdbjq.cn/Article/details/grfgrzwat.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/ghceswkhv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gdjjdawag.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.zdbjq.cn/Article/details/glmvwvpvz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gpalbohmr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/gpeqkqtkc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fehbvm.com/Article/details/gymsehopq.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gnrktneez.sHtML


<!-- 参考信息 -->