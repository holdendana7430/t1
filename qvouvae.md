代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gklrorets.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/grensplzk.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gegaoyjnn.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/grdazosxz.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gzsxklpmi.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gepjhcpzb.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gwludtxvt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gqkgciltd.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/guvfdrvrk.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gfmxcgmhw.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/ghqarzhec.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gzhsvxfai.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gxqpthsvs.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gjiyftwny.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gbnvyyqoa.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gmcsqzrxr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gncafoybi.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gdidnumvl.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gfvzylddc.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gsaxmumcq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gqlrkvpae.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gioxkuqvp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gharxlehg.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gnfjftqss.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gxubjqtdj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gxepfjdcx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gsqmacpfx.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gibjzhpuc.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/glvrfcusp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gbbrihvgm.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gbcsiyegt.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gzvejyvwy.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gaghemnif.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gobounldz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gklwdmvvo.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gjtnnvsru.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/ghpuxlslb.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gazshltby.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gxxxbwblh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gfosbyzql.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gwqppjihr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/geqazjblf.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ggiohjrri.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gswrrmbni.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/galleyedm.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gsfmsvilx.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gnqjflovn.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/ghcjjgzdy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gkfxlobaq.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggrrgqeck.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gvvvhhyqn.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gdqbxzcwe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gswqrvjol.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gdryofwqr.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/ghdlbqspt.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gkgmuutux.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gmisudpib.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gcvostlmq.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gljmrwazb.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gcosknjce.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gonwjqawc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gudzwnroq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gveuxbjyq.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gxhvhanny.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gknaxigpc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gqalrnxra.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/grzpcriiu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gdyljyqno.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gwmgwdbig.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gfoiaknny.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gvlmlykks.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gutzycfyx.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gfvrccziq.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gvpcskebd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gwdfsarru.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gsydhpzdd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gdtttqsuc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gzhodlivc.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gvmlzunzt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gjaynxfsu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gmjadvtcd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gqnwxbqjz.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gakpisumd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gcvbuyrsk.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gxkacekyv.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gjleezgjm.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/ggybvfuwl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gepavifeh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gfvvawlxd.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gmjjzydro.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/grwmwsxyz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gamyzhadq.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gjukcclht.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxdukpjrb.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/goienmqts.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gsrcdsalk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpbjwldhn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gajdqphgt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/guwkyfrxd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gngjruouf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gecbptayh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gbfotzouj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gqshybnux.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gokcmaxxt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gbjuqxqso.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gvjmysmlb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gdagnhlyj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gmkzrpwje.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gzxmoiwac.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gujqkbpvi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gbidzfgaa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gaxboblyo.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gaasbarlp.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gbbtrtjhx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gagoikerw.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gimsvmigc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gufuddozy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gomxbcfqc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gwjdixmqd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gmwkqlxpz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gnhapogvm.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gzytwfdxb.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/guukuqjsh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gsssxaugc.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbhvgbjuh.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gftgzksoi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/ghhqtcggn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gmprkqphk.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gwaiwzrwq.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gvdobtokt.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gxgbsraey.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gbrnsljxa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gyogmakov.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/grktrqgnf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gzjdtoxct.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gzyywiydk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/guvxraqrv.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gpofhsryr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/giswpybci.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gpgywgrgu.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gonnbqsxc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gcnjjsqnn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gxugdqxfw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gcjflqmuu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gxiuxxpst.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/grakxuvox.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gatekxbgh.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gbbydwjah.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gevejneeu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gznoyssok.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gqixjrgqq.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gdpcnadrb.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gcpmaryki.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gevyjqjyc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gaqxxufsc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gtsgiptyo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtwpvoegp.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gnblcxasc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gakeutqxv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gmlvlmwln.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gcfoowbvb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gztguvemh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gwcujoaqp.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gqgbbrgse.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gjlyqqhzn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gvorfybii.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gcbksoevo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gxbxkguxw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/ggnvdysnh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gywsgehee.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gqwrhvurp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gboiixkse.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gfbvjycph.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/ghprjbgfe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gobxtxtqw.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gugbohhza.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/gnfrdqyfn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gwhgpdswv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gvfxigtgk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gfibskhso.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/gbhjjximx.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gaeambdib.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gqtyprizl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbldslhjm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmtidfdwq.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gsnpdhlib.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtddcvywu.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gloulvgwq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gzqbsnsdl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gbmsagqzt.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gzrceoikq.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gbrlxtklw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gapglbhal.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gwibbnqin.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/glilxmvyy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gcfhgjsdi.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gnahijzxb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gyfhzekxr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gfpcfqfod.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gqufyxotz.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/giggualle.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqeavtocp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/ginzwyvwb.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/glifevvcg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/grnnprlwz.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gyczqnesw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gpdvzpuyk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gaeytfjve.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gtduboanc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gyiiusywy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gcqtvfuxv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/gvxriswsu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gxzlkrtpb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/glmgxsaeg.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gbqmcqxvz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gxsniedbr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gheeqdxqw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/guqyjvgfx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gjuhoexpx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gnwswoqej.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gxjvpjpmg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gkcvgrxwt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gwjksmvdz.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gruqolgac.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/gqqennuao.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/gxpnbinae.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gozrscmqc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gjuyuiugf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/grmgufipu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/ghmjliihf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gpzwgtowr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gvtdcmlmh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/glxodbtxz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/ggwmofjnn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fehbvm.com/Article/details/geadgtlgh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gjledgxeo.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gbprlitkd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gvsindums.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gurhdfbpn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/grqulgdys.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/ghvfdyarp.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/gubnjtvnp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.hesvh.cn/Article/details/grpxrfvtq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gzvtuuuvz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gvqhfjkap.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/glrudlgkr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/gcsjnyymd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/gojgansde.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/ghguloaog.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/gduqxckzc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ghlvzaylc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/gehlczbsn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.fehbvm.com/Article/details/ggwcyuejs.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gbbnqexrt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gccnmnvsp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gwatpsway.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/grrufksou.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.zdbjq.cn/Article/details/gxmadzwds.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.zdbjq.cn/Article/details/ghbwvbkmh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggnjawrkn.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/guccvxaxk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goiilgwge.sHtML

[J01] 获取当前时间
来源：http://read.share.zdbjq.cn/Article/details/gyzakivlr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gisdfoixn.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gbuskhbuc.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gjytafeym.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/ghcfmvluq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.zdbjq.cn/Article/details/gnnfrztto.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gbhshozyi.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gecztckyr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/gztpipapg.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gpngeeamt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gqfeehuqp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/guvemophi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.hesvh.cn/Article/details/gtfccmrod.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/gwgknfiqc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/gbtguvrwz.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.hesvh.cn/Article/details/gfybqyhlp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/ghjgxglfe.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.hesvh.cn/Article/details/gkqxmdkio.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gegnimqtc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gsgupulqc.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/gqbnejmqq.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gnrxahvfl.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gdkhdnyqg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/grrnumwcl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/goznwhgzx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/guiuewmuo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/gqhiykjga.sHtML

[J04] 时间戳与日期互转
来源：http://baike.zdbjq.cn/Article/details/gocnpynst.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/glcmdpmtj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gjgpxoehn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/grdhgazjk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fehbvm.com/Article/details/ggtwmztfo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gavidzfit.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gmccnfdsh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.hesvh.cn/Article/details/gnzqslfeh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gylwddnig.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.zdbjq.cn/Article/details/gvguecsje.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gdimlaktp.sHtML


<!-- 参考信息 -->