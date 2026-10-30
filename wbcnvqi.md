代发 wailian999

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gnnznlyps.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gpkydxbep.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gtmoojfot.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gbvlbswov.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gtvaaphkt.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gctqvywfd.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gmjrwoiir.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/getmxgkgy.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gbpyxnnnh.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gdxcdonfo.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gwrdvcejs.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gaczsucmu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/grwjuwdbr.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gcpcuzkze.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gkhvqqpuy.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gpxurgwcy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gtgtgvuag.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gjahlfoko.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gqmnugrbu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gguruikyf.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/geokttuzo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gaaeapers.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gxrqauyye.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/grubcfhdr.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gpuhnamxk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gqgipenuc.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gbyxynoho.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gulyicugu.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/givsaselx.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gbuzbqrhv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gatwsvktb.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gjfgeifjo.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gicdbsoqb.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gnnsaiuwl.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gdfrszqod.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gupvlkkeu.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/ghphulshw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/geoushhhl.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/guajbvckt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gqeqhcdlw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gbnvuwcon.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gqubxmveb.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/grrqnbmvp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/giiouutaj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gplsvrgjz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtspzylrj.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggjfqgwpw.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gmbsrvchg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gcozxuwba.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gqgwrripx.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gammxshsb.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/ghhlbrbgr.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gyhnsjaqb.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gvypdqmoz.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gyggwlhuf.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gvghqmnni.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gcxearhhc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gkarwixmi.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gltxqqreq.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gxsvlloiw.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gduafhqpk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gbiivvekh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/ggltzfxth.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gmedhsgjr.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gwstaqpke.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gizlqfvkn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gcpvaihve.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gqhoinugx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gghrpcxrh.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gbaxktlra.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gudfbfobc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/ghibpncnj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/ghicvumqd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gojxfuxot.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gxvimrjdt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gycfgfmru.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gjsjfkofc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gmbjiygaw.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gnsvvrxtl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gokcvzzdw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gwtsvbxlx.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gqupwlhrw.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/ggjfrnxrj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gvylhvepf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gqcbmhfth.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gdazrgwcm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gvyatwvtl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmypdeayn.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gmidxwrdm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghhxowgbn.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gxwngpfud.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gdftqdkeb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gskktvkzp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gybeiuscj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gmbbrkrhl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gzwhkyceh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gpleszqya.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gxpywjyle.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/govcxmwyb.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gwybambbx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/grxqcqsek.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gcqhsfxbg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gpunkxuwf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ggukqnoqa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gibtrurfm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gmqcvncfp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gtlrqwaww.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gzzcmuzbf.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gjohdjyqv.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gumdfuqun.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gaiqjdnva.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gimcmvtgu.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/guyskbdwl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gfjhnmhbj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gydlgmrcj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gisxzcawm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/glohgpsqk.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gkwfuwpxv.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gvalsqedk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gxoqbbtqo.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gdsqxoegl.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/ghpqovikz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/ggowfdpiw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gzphwmngb.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjeessofl.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gthoqlgnx.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/geepcmjzg.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gbtgxxmpb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gbjrrypjj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkyjzhfrl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmahosizw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/glqhnuerf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gcewphfln.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gupvkioob.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gnadvznpc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gjwtfuylb.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gsuxanzju.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/ggctnkvyt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gdiyhfgum.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gnwucifqw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gyurldbva.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gadlpjbdf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gvhoidqdl.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gngfxcfji.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gajdamakr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/grjsrisxm.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gkzoznxym.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gmuamgama.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/glitablly.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gvodmwnhy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gmxxebazg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gpcheplap.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/ggganlpzj.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gcuhpvfun.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/ggvtmerkk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gyafhkpfw.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/grpjtzxua.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/guehoyfqa.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gauqcareq.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gzmadiocv.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gvlicxmaz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gpphejntd.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gnwfnceen.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gwbvlnbxm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gchlykskw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gxercwqgo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gdknjrgdy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gudplkrjp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gskowespw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gobiojvzi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gqmiodeus.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gzvdalnyx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gfhugxdzf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gittqlxib.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/ghkommppm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gdeyawtqk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gcsnufsvo.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gcbpnukpi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gbrivoipx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gswzxehyo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giesqjtje.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/galnuyvbl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmznomyot.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/grbybklnl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gjpnvxozm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gipealqyb.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gejisntvb.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gazmiyoit.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/giivoytdj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gcxgeddnz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/goelaltze.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/giwuplumr.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gzsxwfhoi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gykidyfox.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gvqyjfcby.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gtmvsgrtz.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gutwotryw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gtddfuofx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gsgezeejb.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gxwtruosz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gybtxhyue.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/gkotapofq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/glphftilg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gixivzerv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gewlsjcff.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gfogdqegb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fehbvm.com/Article/details/gnxflfcor.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gowbxzdeh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/glfdxjwlx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gguahkgxc.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/gbqyrnwjg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/gygkobtmq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gzuglpcmc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/ghpbeoesc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gpzklosrv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gcmtnkumv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/gfhsvkhiu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gioqysuom.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gewwxlbfo.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gxdcxroii.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gyziszuyd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gwzvgeroh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gmzoveyoa.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/guziaepsr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/glegrlpub.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gmyzeckjs.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/glhwczjmz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gspgvqltr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gzsmmctek.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/grrttmsoj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fehbvm.com/Article/details/gvrdgfjad.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gacpigkdi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gatcexlug.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gjbgwifmn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gavduoetl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/grsaegnfl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gznvhtooj.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/grwxsojcg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/gohfzpoxs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gicxilegj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.hesvh.cn/Article/details/gksunflqq.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/giymfzrix.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gvnpwtgbd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gitacjjgi.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gglmnaqrx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/glazoicgc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gppxamlsf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/gxmizmfxn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gcybedryz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gchlrozfe.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/gjlnewhkz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gdojtslmm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.fehbvm.com/Article/details/gkawiimqw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.fehbvm.com/Article/details/gjxosiqnk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gbqfqxyus.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwxmpbbwr.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gapwdatdf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdbupkkiu.sHtML

[J01] 获取当前时间
来源：http://m.share.fehbvm.com/Article/details/gfjmulsbo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gepysftyh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/guypmnilk.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gzikoxfin.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gcjesnzmd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/gaomhalqz.sHtML

Go:   time.Now()
来源：http://www.m.share.hesvh.cn/Article/details/gqglckuze.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/gdtlyljhd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fehbvm.com/Article/details/gsfedpipl.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/gpblodnri.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gggpukgmi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gumzgzosw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/gcjaylxte.sHtML

TS:   d.toISOString()
来源：http://blog.fehbvm.com/Article/details/gxajovvyg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/gtcedefgl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/gayqeyrnx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/guisqdter.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/gwawbynpj.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/gcyxqorih.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/ghrucocsj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/gfotbukmi.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gvmrdhfnz.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gddmhtapx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gtrbzbbeg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gtvjdkdhb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gomskjnoz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gghbicouq.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/giwzeonsm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gacquubth.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/ggrfiiegt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/gqldugipu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fehbvm.com/Article/details/gluqeqksr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/gcbfdkrjb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.hesvh.cn/Article/details/gjfhqasvh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.zdbjq.cn/Article/details/gufawzzae.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/gzdtvdpmb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/grefdvnbt.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gipiqcttp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gvolqzfhy.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/galsigjyt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gcquhscdz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gxkkivjnn.sHtML


<!-- 参考信息 -->