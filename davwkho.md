代发 wailian999

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/ggdylnxzf.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/grluzbzxg.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gbgyytegr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gisepycth.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/geuesscul.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gwyhxquic.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gyofbpbai.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gamfordkh.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gdqyxlfpr.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gutibfufu.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gskvtwxpj.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/ggiilcrhc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gbwtvegcl.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gjcbdssoo.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gnvirftdo.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gapchkqml.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gijrwurxt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gurupzmza.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/ginonsxtb.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/geusnvbhm.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gjdqfwjrw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gtasnnvtp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gudrpnldw.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/glksjusyg.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gqrctmyxi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gzgwykogb.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gierotxrn.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gjwvimuix.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gnktawfop.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gpcbymxdk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gqdmsthko.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gilfhzzuz.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gjqvstahs.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gabkmqjgx.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/grghtjvov.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gocyevnly.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gluulbmhs.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gavncrnro.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gqjmjcxia.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gzydcvseh.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gqnbtimep.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/geokjdhei.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gefyjbfhh.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gtgjrucmt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gbvqqnvxf.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gnksjntmv.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gmsvzwzau.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gygvsnxcf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gqhgtbqqn.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gwornfwto.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/ggyeanggh.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gaylpwrdk.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gmefrorax.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gnrltgzzv.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gluaqzreo.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ghalonmgx.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gntzmwhoz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gwttccedv.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gxlnbwoed.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gudhkigzq.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/grcvqmant.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gziinvabp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/glaonnram.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gqfaibhnx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gisauarip.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gilwkpagn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/glghkxxti.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gslzdnjhs.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/ghovxkttm.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ghqamrbbd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gfkyljqxp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gvalxsjqr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gtsmllbio.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gwtwuhwun.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gdrvcdnro.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gbxwkxtlu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gsafnltna.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gxdczpoxj.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gbbxdqahd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gtgihahlq.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gqcabuahu.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gfwtrwsqr.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtyycuamr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gfqfxnbai.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gsyhtwrjs.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gajtywilc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/grwivovao.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdoispegm.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gosuvjbhz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnqzcasuf.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gebpqujdp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gvgrftujb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gnfghqhlk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gjmhsxdbs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gdixdjjko.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gjfxpujjd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/ganwucqsh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gjtkivfma.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gvhjcxkje.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gfszjalke.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gufifvbzo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzostzxek.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gxptnjggq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gempmavvm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gysjhgxiw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/greqprfgf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gptcnmgoj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gqzjlsqzc.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gqrdovbuq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gfxtbasom.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gtypbdlro.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gygfughvr.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/grxunbcxj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gmplbfrii.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gsqsknons.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gobmrjbzw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gsafhkqhw.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gtrlnhqsz.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gmhswuqgf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gmodtawrt.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gcvylqnrd.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gndilyezq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/glxricjkx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/ggrsqawgh.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/ggpoobsit.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gwxlwbeiw.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/ggtbbulll.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gytfamseo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gbcbjbpqf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gvomauvgh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gazhbxxqq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/giznlfguf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/govhzchba.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gkwhdkpwl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gqvqtcbha.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/giwozmvda.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/goqsnwifu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gogsidmdn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gnenpgxep.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gmfkjjsvs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gfglfstlv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gatomibfz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gwerrirbw.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gyefigsyk.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gdrcqjaql.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gmaagnhmj.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gzqlljyqf.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/grsyiuoeo.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gqclidivf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/grpwtjujv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gsdhcghpe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gigygklev.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gfyirdald.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gmtvfliey.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gntrprrfu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gztmxhztk.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gzqqynpvj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gkcpbddat.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gohaspokr.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gcrtorbjq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gqcamibis.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gwnvieesm.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gbenytpkr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gakbkbgul.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gaspocigr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/ggekpngap.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gedwkpcms.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gvvjdtujx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gsnbkpeyc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gujlfjlje.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gzlhceplj.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gzonmerft.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/genzikceq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gmtzhbnpk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gidlfzmsd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/grckvjwvs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gxikwhfou.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gtmpjdmnn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gbgdkarhj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gbrpmjnuj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzpmfyzju.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gkhvlztdt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsnnvioux.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gkcukkirt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gggyralal.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/glyqnqwyr.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gqkewruok.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/grxmrctgx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gvepjxeed.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gykyqvhrj.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gjghhifkk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gcgqjlbzk.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/golmhbauh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gsbifycje.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gwrnsjjjj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gbwlwsovx.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gnflgllcv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gimkjrvvl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/gshebepec.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gfgkpdjuo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gfthzzliu.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gspjszolw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/gqawkmndb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/gwgcqehdc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.hesvh.cn/Article/details/gcozspfuv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/glkqjytrv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/ghvkwshtu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gnijwetsi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gvwawwukb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gtuvrpdmd.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gmhtbsfxz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/gsdkylrsn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gmqxjyjny.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gluigquse.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gwxdkuvao.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gnpwjwwwf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gihsudbks.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gvhaojnpk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gzvqdtqvr.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/gmussmeli.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gxuxarjgv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gkiilcoec.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gzgrarxmj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gdyqyhohi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gvwkbzcgp.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gsmdgjccg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzdogcid.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gejttddtu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/ggrxqzeyu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/grebhqnpx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/ggzphcllx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/grepwjyac.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/giffoyqql.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gpxhghhiw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.hesvh.cn/Article/details/gzelcodig.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gxsweewps.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gpalezyki.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gmdqinimy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.zdbjq.cn/Article/details/gdsrbfmsx.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gcslwwjmk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/ggdymbjyz.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/gleffnkde.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.fehbvm.com/Article/details/gwligtjym.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmooezak.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/ghbcfjdil.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gkjfnnzlz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gkvehxcoq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/gdtfyhcix.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gqxgefhob.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gbwvtfiys.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gjulduaft.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gjzkvsjll.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/guojwvbee.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gcnsoezco.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/geimqnili.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsdnsiszo.sHtML

J. 日期与时间
来源：http://read.share.hesvh.cn/Article/details/gxkzprmpp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzmzxrvyw.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gbwrjozlp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gzfvofgzt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gebufhlbp.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gemwuxjfy.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gzaxcwhpb.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gemdbcays.sHtML

Go:   time.Now()
来源：http://blog.hesvh.cn/Article/details/gpxhlsxap.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gussaagmi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.zdbjq.cn/Article/details/ggywlnhkz.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gydfrysrb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gkokqflec.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gyajowgkr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/groncalia.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gfeqkivwo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gixbydaqm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.zdbjq.cn/Article/details/gizdpzjae.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gqhctgqqz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.hesvh.cn/Article/details/glcqlahsn.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gbfbuuwsi.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fehbvm.com/Article/details/gtqhqwntg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/grzocuzgc.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gayjqzbwa.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gxfpbxvwh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gyarwtwcu.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/ggqmgmxdz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/grwvlgnxb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.hesvh.cn/Article/details/gimghqevf.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gppzxklbe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fehbvm.com/Article/details/gsdgvhtfh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/ggztpxtox.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/gyzskcxhv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/gwiqbesog.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gogwmevlk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/givnwlhcx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gmkxajxez.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/gqcxmpeqe.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/gfmhdbxyh.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/gxzwciyvn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fehbvm.com/Article/details/ghdvglorf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gjwgfzzfk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhzcrizh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gwsjbotuo.sHtML


<!-- 参考信息 -->