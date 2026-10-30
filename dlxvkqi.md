代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://blog.fanxiaobao.xyz/Article/details/gkgyavujf.sHtML

[G07] 调用父类方法
来源：http://wap.fanxiaobao.xyz/Article/details/gtibxdygt.sHtML

Py:   super().greet()
来源：http://blog.fanxiaobao.xyz/Article/details/goygdivlf.sHtML

PHP:  parent::greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gewxombng.sHtML

JS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqatfjem.sHtML

TS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gpbomiabk.sHtML

Java: super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmkhloqv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gykdngkpb.sHtML

Ruby: super
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrnvrocr.sHtML

C#:   base.Greet();
来源：http://wap.fanxiaobao.xyz/Article/details/ggqmjcyfp.sHtML

[G08] 静态方法与属性
来源：http://baike.fanxiaobao.xyz/Article/details/gujpdivet.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciwfgnky.sHtML

PHP:  public static function f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcblvspds.sHtML

JS:   static f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gybisojfk.sHtML

TS:   static f(): void {}
来源：http://3g.fanxiaobao.xyz/Article/details/gktmbsupb.sHtML

Java: static void f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgdywlab.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fanxiaobao.xyz/Article/details/gphysnqop.sHtML

Ruby: def self.f; end
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdkgjqdz.sHtML

C#:   public static void F() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gltozyvgc.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fanxiaobao.xyz/Article/details/gfbahuinf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlaifkag.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graobhkwc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fanxiaobao.xyz/Article/details/grvsefqtd.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghnfdzwun.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gilfhztuj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fanxiaobao.xyz/Article/details/giqvxttye.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fanxiaobao.xyz/Article/details/gxndikjmx.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gbfzdtlep.sHtML

[G10] 访问控制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybgtvxam.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxytzfpg.sHtML

PHP:  public / protected / private
来源：http://baike.fanxiaobao.xyz/Article/details/gjrlvccvo.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fanxiaobao.xyz/Article/details/gsploeunf.sHtML

TS:   public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gafmizcvz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcrijmvj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxkmlxzb.sHtML

Ruby: public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/grulrlodj.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsljkikm.sHtML

[G11] getter / setter
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyabktpgn.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvlcmahd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggibxgkon.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbwmsxriz.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gakfismit.sHtML

Java: public String getName() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwbxtfuws.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmiqnfcz.sHtML

Ruby: attr_accessor :name
来源：http://baike.fanxiaobao.xyz/Article/details/gypftcciz.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdtvnczvl.sHtML

[G12] 对象转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gdwnmojrp.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fanxiaobao.xyz/Article/details/gokrjqrxc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/geryvdvwy.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvxtorhlc.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gflvwlpjd.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgylgpmb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiuoikau.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gmnpwfcwr.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdbwitvp.sHtML

[G13] 判断对象类型
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqsruhev.sHtML

Py:   isinstance(u, User)
来源：http://3g.fanxiaobao.xyz/Article/details/gbqdrrvbn.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjdjimnh.sHtML

JS:   u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gghtreljx.sHtML

TS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/grlplhbdi.sHtML

Java: u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gowksywxf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fanxiaobao.xyz/Article/details/gxvvbgljt.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxambdrff.sHtML

C#:   u is User
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzxxfqjc.sHtML

[G14] 数据类 / record
来源：http://3g.fanxiaobao.xyz/Article/details/gluirulvs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnsdhqby.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmhojpxn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwfqvtvn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fanxiaobao.xyz/Article/details/ghygeavvm.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsabnonzr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzamccbcp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyrtkclc.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmhdktgl.sHtML

[G15] 枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gnkxpydiz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaeccmva.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfqujucfm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fanxiaobao.xyz/Article/details/ghkjclzqz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/glferlzur.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtothailk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fanxiaobao.xyz/Article/details/gavuuasmd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdbnwvmc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbkfuxxk.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fanxiaobao.xyz/Article/details/gkeivbwbr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fanxiaobao.xyz/Article/details/gnbclsljy.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fanxiaobao.xyz/Article/details/gmasakese.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gegthcjld.sHtML

TS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gtwjqegyr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsbfgveq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fanxiaobao.xyz/Article/details/gilncjghe.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwohdoyy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gyghfddly.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbskftbc.sHtML

H. 异常与错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gssfozakn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guigehvnw.sHtML

[H01] try / catch 基础
来源：http://baike.fanxiaobao.xyz/Article/details/gtwindyra.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fanxiaobao.xyz/Article/details/gsxcyspzg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fanxiaobao.xyz/Article/details/grguxjtjx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/goighmdga.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/grvpebqkc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fanxiaobao.xyz/Article/details/gflmbpaqa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fanxiaobao.xyz/Article/details/gftsrirgi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/glckfroni.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzruhavjf.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fanxiaobao.xyz/Article/details/gwceohdni.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoouclnq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghusnemvb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gizkokfig.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gxwercbty.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljfsbsok.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fanxiaobao.xyz/Article/details/gbwwmnsul.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fanxiaobao.xyz/Article/details/gmoiasodt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdvnuwrl.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvwyahvr.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fanxiaobao.xyz/Article/details/gghxsksyj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gwxzkryxq.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsaclnyf.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdvvwqux.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeqpxktz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbfwkksg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybulevku.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvddaxrl.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyazeyypn.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxzyztkz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgcwgwsb.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiohmevn.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnpmlsfc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnvnihmi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrsetzcc.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfcmkdjg.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fanxiaobao.xyz/Article/details/gpazystqa.sHtML

[H05] 捕获特定类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqxwqzxv.sHtML

Py:   except ValueError as e:
来源：http://read.share.fanxiaobao.xyz/Article/details/gwscuhtus.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpxlsvva.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnswuzwa.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbmzwvqz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkghflkh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fanxiaobao.xyz/Article/details/gdsganlsd.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fanxiaobao.xyz/Article/details/gsmlocksw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyupudpzs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fanxiaobao.xyz/Article/details/gktexvfit.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fanxiaobao.xyz/Article/details/gpzydokah.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuolpsys.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfkqefbw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/ggjeswhdl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fanxiaobao.xyz/Article/details/gehgzvnps.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fanxiaobao.xyz/Article/details/grspxrvuq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fanxiaobao.xyz/Article/details/gzipypzbx.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gwxgozfzz.sHtML

[H07] 断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtgugfmo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwruxetnd.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmujinmn.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gucoiggrn.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gxpxrevae.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fanxiaobao.xyz/Article/details/gpqratzmc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gauiiachp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxokgzoef.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjnpicjl.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fanxiaobao.xyz/Article/details/gbifcixtd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwecahvda.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fanxiaobao.xyz/Article/details/gdxopapay.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorabbcvv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fanxiaobao.xyz/Article/details/glhxitgls.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fanxiaobao.xyz/Article/details/gtzuqhdvf.sHtML

Go:   err.Error()
来源：http://wap.fanxiaobao.xyz/Article/details/goddysjlc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girxsluws.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fanxiaobao.xyz/Article/details/gppyhjdbl.sHtML

[H09] 带错误码的异常
来源：http://3g.fanxiaobao.xyz/Article/details/gwomhoqcz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtlgmqta.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/ghxeldnyu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fanxiaobao.xyz/Article/details/gogjjdrxp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiqqicps.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsifbbdh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/grwdtjhxr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvryeacx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fanxiaobao.xyz/Article/details/gfczqnitq.sHtML

[H10] 资源自动释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmjpqlmc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fanxiaobao.xyz/Article/details/gehsthupm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fanxiaobao.xyz/Article/details/gocbxpmmg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fanxiaobao.xyz/Article/details/givoxztgs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gzouwnkpb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrhwpnuv.sHtML

Go:   defer f.Close()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgfnxldl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlqylbpn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/goqnlrrvi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkgdwypk.sHtML

I. 正则表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeskarze.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxvlvbpno.sHtML

[I01] 判断是否匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzkthzkg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gjudfsnwg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmanwdyxl.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gbxlxdxap.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbijauco.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fanxiaobao.xyz/Article/details/gxyffvufr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyltgacxt.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqujksdwt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fanxiaobao.xyz/Article/details/ghwtmxcpe.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqwgjatk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fanxiaobao.xyz/Article/details/goppzivqx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaywofba.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fanxiaobao.xyz/Article/details/gzhqlexuh.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fanxiaobao.xyz/Article/details/goecxiwqe.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/glejtqtqt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gutnxwbfw.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gyuvobqej.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggatzqxhe.sHtML

[I03] 提取捕获分组
来源：http://wap.fanxiaobao.xyz/Article/details/gweemlkjg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gzqgdnkxv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gtelcntka.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gtpeqixfj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/glaovtifn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fanxiaobao.xyz/Article/details/gfbkvcvia.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqketbqm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gyeejsoyp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpztqeef.sHtML

[I04] 正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/guolmluou.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpenasqkr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gfhbkbzhh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gwrcklgwv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gszkivghl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycwzwgtr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/grixoawmf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gboirwpsj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpjnkvoj.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwpazhqa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gpcycscns.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/grdhfeopa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqobrhbbz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvytdcku.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/glzzxnbnu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gslrkmrsu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcnnfnha.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsipifnbd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fanxiaobao.xyz/Article/details/gndvlpyav.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gkjzewlij.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzcutltr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fanxiaobao.xyz/Article/details/gftgvgcws.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/ggonlsrmj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvydkezo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpyahwhr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsargjxv.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fanxiaobao.xyz/Article/details/glfrinwic.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtmhvobc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwocivsrb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fanxiaobao.xyz/Article/details/ggjsewmki.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwafxgfs.sHtML

TS:   /error/gim
来源：http://wap.fanxiaobao.xyz/Article/details/gcbsjrqwu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdfhcofp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgtprdld.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryrwdcap.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fanxiaobao.xyz/Article/details/gosxfzaqy.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gevjxcxiq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozrzzjbw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhmniwov.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrnfozmv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gzbksgacy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/geamwgdct.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fanxiaobao.xyz/Article/details/gmiicwazl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fanxiaobao.xyz/Article/details/giobhqsmc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/gjkytqkzr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gupdzfzch.sHtML

J. 日期与时间
来源：http://wap.fanxiaobao.xyz/Article/details/gglbndnld.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gezqgttxh.sHtML

[J01] 获取当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbeastcf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.fanxiaobao.xyz/Article/details/gembnjwlk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnbwcygh.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqgxhajn.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwnrpasg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fanxiaobao.xyz/Article/details/gywzgbwiu.sHtML

Go:   time.Now()
来源：http://3g.fanxiaobao.xyz/Article/details/gyhnkbudd.sHtML

Ruby: Time.now
来源：http://3g.fanxiaobao.xyz/Article/details/gkmyoloho.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.fanxiaobao.xyz/Article/details/glbuohjmr.sHtML

[J02] 格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhogguxc.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fanxiaobao.xyz/Article/details/gkygfiixb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fanxiaobao.xyz/Article/details/goaikghyc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuoeldgf.sHtML

TS:   d.toISOString()
来源：http://wap.fanxiaobao.xyz/Article/details/glfzcsqtl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpkrajwh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fanxiaobao.xyz/Article/details/gozwfpavg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkidevhx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fanxiaobao.xyz/Article/details/gmednlvvo.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fanxiaobao.xyz/Article/details/gsflqitfp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppbmohbu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fanxiaobao.xyz/Article/details/gtkjolfwr.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/glontgplu.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gqrwjcajn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gobvvcaoh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gvfohhecd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmvvrypt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwdelowv.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gukrioibn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvajlvefs.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fanxiaobao.xyz/Article/details/gbeduqwss.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdweddung.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrshyjwe.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/gaxjsjmuh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafdmefbv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gostzogis.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/ggtkvekbj.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fanxiaobao.xyz/Article/details/glzaeajvy.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsnevufz.sHtML


<!-- 参考信息 -->