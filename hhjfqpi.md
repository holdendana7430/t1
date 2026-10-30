代发 wailian999

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/giqrpwipn.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gwckvlnsn.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gdyndaqnt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gumymgkki.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gqqgjurhm.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gtqrmgokd.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gwljpwwiz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gcwjawtqu.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gkhsghdwt.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gpzrpwtpp.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/guignjseb.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gymjcxrdt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gbtaxomxj.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gglmytrtl.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gvkvbuoan.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gktbpfdce.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gmkdgwrhi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gbwjiljgt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gxfvkqztx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/glpiyluic.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gxvgsldjw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gmlakowpa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gzybceome.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glszkzcwc.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gxtgvuygp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/goeyraspi.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/genkxytny.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gstrywmzh.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gqhyrjddj.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/grpknqbqf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gaakeyyfr.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/guagniigw.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gldwgqjdv.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/giradxjxh.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gftyhpjbb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gfiivzlfg.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gflzytsno.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gcfbmkbxt.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/genkbdclx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/ggeagrere.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gjywttuhx.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/ghiecwdmb.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gvpzfxaqt.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/ggmootlrc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gkvjlorwz.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gnqnremsh.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gviwadfax.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gwnrsihpw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gyzurrnsm.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gbokqnjad.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gjeoorfog.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/ghyhxmgch.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gxncogcxa.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gyfgfbvnb.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gsgzigajh.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gdeadweul.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gyovfeqno.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gzpqkjkay.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gwdjthfgq.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gfppiypza.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gypnlqetd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/guworlinv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gzxmkejfd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gdzwjadpp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gcklriofl.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gpydozewu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/giscarfuy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gmvzvpofs.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gsmpeqgmx.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gmfqaispn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gouduxpxt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gxfzghlzo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gioiplkto.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gsqgddxts.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gbpkqypoo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gjwwasbch.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gpwsoxmzg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gklujbnzp.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gcyswjjub.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gahurwydl.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gbtbuygtn.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gjsfzadzl.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gbjtehbrk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gutecpqtw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gjnghkkin.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gjoetatmc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gpkqsnorq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gatafbwjz.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gbdxcbgiu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmmrlkyld.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/glylcuhrv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/giekkktsr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/guomhlswq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/grkfqqbww.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gmmluvpid.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gwpacflfw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gitoolcjk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/ggcvstpux.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gfpfstukw.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gpmtzfqyr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/grmmwpqew.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gxhuycrto.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gsaxsupqo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gefzjzeie.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gahacbpev.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gmwyxiprq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gyppjktea.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gvxfgwhan.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/giizqiaey.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gmqpcjgzw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvxmgpinx.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/ggztcqjjs.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gputwbumk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/ghyjrgvkf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gzevghsoo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gfmazgxva.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gquequozp.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/ghjnnsqed.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/ghsdfiing.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gfbeesvat.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/geemobtva.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gzoyhicnu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gqcbyjcor.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gtuojdqnd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gpnlbgkur.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gbobsigkk.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gfuubsqfg.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gylypzqmq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gvizcqsft.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gutzsddgp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gxqxazuof.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/geekwqphj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gvrkeburo.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/ghboakwmy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gndoliivx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/ggxecwrgb.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/ghqsqxjbw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gqitgjuod.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gxeznqbru.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gpfrguivb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gucznpddu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gxkpngubh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gkrmgguor.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gqpwcuhpk.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/glmciixcj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gywroaiom.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gkycgsxjg.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/grooptlqx.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gvotorwit.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gjykcmntg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/glzgayfhz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gnbtpfvbb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gzyqnsztg.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/geiaduqfy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/ggnfveelm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/gcwyiguek.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gvseiqkvo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gsfgamyos.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gkkfofqsf.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gfqqkzrbw.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/glbmengkm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gmeesiqvo.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gbqgyhitl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gefgltjtt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gkagwefun.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/gbypzznpv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gmgemqwsn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gptdkmbzc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gslzetfxg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gscmbzsxm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gskrgkaut.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gpwmbohsd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gglrvccda.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gxjcetmco.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gpnmxzfxr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gbhzvlqeo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gjohufvjt.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gpiaviqub.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/gvgvuuzfg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnwiwkqwp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdcyetrbp.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gztukviqn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvtrmnnwo.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/grnlkxduw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gqunqequw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gftteyiax.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gfpdjkvtp.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gpazhdaez.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gojunzmli.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gmvnmfuph.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gatzwhyqs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gjgfpwzkd.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/glakumeca.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gadyyycbh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gmttoiibz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gwfynounb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gnygmxzsj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/ggxddllmb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gjualrnyp.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gzxkfskah.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gdhhydkdg.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/grypylpyb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gkzdjzyoh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gyqxprpne.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gpqultrfq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/guhqfnnvx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fehbvm.com/Article/details/ggugkcjfn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gwitbmkzm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gajhupuoq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gjaisylby.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gvmqhheax.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdlrqgxk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gylfjhmqi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gnbsscsaj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gugiklrnm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gifgxrpgk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gemzuadvg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gchrajdmz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gsejrunns.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gdnemurmv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/ghspjzrgt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gvqatgkdv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gouutzibh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gpcxmmdmm.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/giyxxuflo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gawnageqh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gqzrdtfnx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gwjzitnjj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gewenhupa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gqwbecffm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/gjaxprvvd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/grvrnsoir.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/ghspdcdgx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gwnvzxzlf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/gztgwyhee.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gupvloenf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gwsuyljas.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.hesvh.cn/Article/details/ggnpcabuh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/gkhefygct.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gyiwmeqpj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gzzouzqpr.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/gfwlevnut.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/gjtskfems.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gcchcabvl.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.zdbjq.cn/Article/details/gkjleqksb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.zdbjq.cn/Article/details/glckjgene.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/gooczrcvk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.hesvh.cn/Article/details/gbkeykwsm.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gkcyuddjf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gfgdsbkei.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gqrbaddno.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gdptiojis.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gdzwrmhvm.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/gbbwvprld.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.hesvh.cn/Article/details/gxgxuewft.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfihkgxdg.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/ghlqdazom.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grhyplcgo.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gaoeuumpm.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.zdbjq.cn/Article/details/gjjqoneqw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gihmlluxw.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/guleryilw.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gijhawzjd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/geoqobdvn.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/ggskwxllm.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/gdamrtnlh.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gpugoxzac.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gldzltezc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gddhfcyrj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gezjojosj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/gjpzbanek.sHtML

TS:   d.toISOString()
来源：http://3g.fehbvm.com/Article/details/gwfpcforz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gmcoucdxe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gjestfbjo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/grmvlflwc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gykvnmdmz.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gykduipdh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gfqarmirb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gvsmljdyu.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gfoxsfvhv.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/ggukekldt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gycvviypz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gwsdmdufn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gnkjipbcq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/gzwcrimzc.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gqcagbmoc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gqvnfdzwa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gasmjovmh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.zdbjq.cn/Article/details/gtdgapels.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/gdmyuzhif.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/ghwtbaojo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gidsoxcuw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gdabvzbeq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gmiiybgyd.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/gsiteqney.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/gjdymhnal.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gvmucgboa.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gbznexuko.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gpflkmyqm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gklbtkzze.sHtML


<!-- 参考信息 -->