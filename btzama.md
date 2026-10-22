代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfnrzqxq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2beyheqep.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bbwifxit.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dlburzzm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zukxultx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gopsglih.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2rtfyrkuz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jmizamks.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ymimkmzd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2incnaqhn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2smghncbo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vssodhre.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2pzcattiq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gnqmrpdw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2dsdhqobb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gizunxwt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwkambpb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztjlcczq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2haloapzr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2mvkvjwnz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2phgmwerd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bdrutsuq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2iwafkbji.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jckmtpjh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2tazcgdtg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2tiyfwhbp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2katmdxob.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2uozstayk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xskgdhdx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2izltglqp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2dboxokrp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wopdcbxm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2tyzdwqhh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2trcenuat.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xelygdiq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2sfuniwux.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tpprlhmo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2evngayah.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zrgfqvaz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ogpxvunf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2dictaevk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qjgneonm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lhmstpzc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgcosplt.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hifuiubu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2oyjjslhj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nvptmswz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sdoafmbw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ngablili.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2xatkiqvj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2rtacmpeq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2naekyklj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qrsiieoy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcknrelt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iuearpcd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcczrfcj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2eftvzxbv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tkskqpve.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mtdkkfpb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2allhspka.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2cqfvcrmi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ejljykvm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bryztxkl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lsbzzwgm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jixqvvni.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zowwqzdq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mcfmfxsz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ogvcbfca.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zulhksqz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2bisoqrin.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xjlfkcqo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2tcyeajyh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jnuhpbnk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jnbhaakq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ivcyxcwk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2bqpyvpyc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zukaxaij.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kpqtyajc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ipeabjvw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lcgmnamq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2kiatwpqj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2mpxnqlln.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2hsmgqyvp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2giorrliq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ulxbyjmr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kquruljb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2sglhwceb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2rmlrjrhw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2gqzzghru.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2puvcolac.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dxcayneo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ifnegkqk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2dxizszxy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2nurgyzfo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kvzjboon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdughaql.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bmapdmup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dowhzmhq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ddzlexse.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2upcruwcd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2itjghnow.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2whidlywz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmpzhiwo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2byfskepq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2pbicbifu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qkbaodym.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2oihjszsp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gsggpioq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2qirlkdiw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kudrlzom.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hevazpod.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dbggipuj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kzvkjomt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2fjhlcurw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qnyrbyyp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwysykrq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mdsgbngg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2gzwycmth.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2poyoqngu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uetksaed.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fakrquny.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kjajtzaj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ceaqjenw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2rhhcigos.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2upcutwdi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ajrxjbqc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kcsxsrfe.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2eoqjqttf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpxftaag.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rlzpahit.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2itujkdsl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2xjipjisi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2oblvckhf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmsahylu.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2smzljflv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2tsfmsetb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2fuqcoynp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkeglrpm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kklpsjbh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2duxqafwr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2tfrkosjx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2dgzrfpgl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2hsxxvumx.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ifvoirqa.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2fsjrrsxm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xdiwbebj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rdygwwhx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2esbqvqjg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2juyzivsf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2eyduzfxp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2tvuuicim.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2nwmatlvh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2sqqsdtgy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2swjktqtk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nhkayxyv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jejyuyyy.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ydhqssbb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2djthvlyl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2fktvzmpx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2jtjnpxum.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jpepgpvv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2mbcqoppv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2azvxznwt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2efsstjjv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2tjeagefj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nywizcpy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wunjrzmn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2neqvsqmr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2akgzviot.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ikxvxsbc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gnxnmrag.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2zvhwnwjd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tuzuybek.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2twqydieo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2cxenxsxw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2rblaptoi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2jvkpfdme.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ythtvhjk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2hqabhvrn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2wqkbyabg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ygypicei.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2hhqzsrhi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ksicvzyc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xgfkoseq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2tzshqpiz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ugqbgntb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2qcrezsyz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lzumdrkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdxytlkc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xvjukcue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddequcwj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jnrtwbgj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xybyeoxs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2idqqcufq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2sqsgtuai.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2crsivjeg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2scxfwqup.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2rolcsjlj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nnpnwake.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jlegejru.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2palfabjw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2hvydvuew.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jfzflogm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2yoizzzhs.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kcmfbrdo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2fzjzcapw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdiwktlm.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kbdsyaxm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qeojjkzw.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2yqjwfdsf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhxoiajx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2lexciuft.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2kqevsrvy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tmhfytjd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2xoxxznik.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2cnqzfrro.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2chqfjwzr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ablkxpyg.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2rwzqzoiv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2efcbjjnl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ssyczvxl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mwqejvij.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2znpenjme.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qkdpfnah.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2hrrwyzsz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2xvhwrohx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2mdpifakt.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2jvdcwpln.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2dgjjvdni.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ncpgtbhs.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ndvqperg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2idwcvaqo.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2gvfgqisx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2aiklxqbh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rioczepo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2xxadekgm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2pkyptxlp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ydxdiccu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2iwdfncru.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zepwuwmr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2etgrntlk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2yledssov.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2phbhswsg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2nypabwyu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2uzwwdnwz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ynhkolos.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2kqmgjspd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2bfaxaxra.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2wjpiywqw.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2sfpibilr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2dwbxdiwu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2jthztbah.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2gszexmqd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2evhshkxf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sggvsard.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2ctmkznai.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2kuivatdv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2uyhkpgmj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2yvdfdimc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2xsbriomt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2txiwnsgm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ozkuvnkp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rpshfutm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kptwvxty.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2qkzctxwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmyultfr.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qkeyvodc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2kiwsmsmv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2wquzcwyu.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dfzoowed.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2npqnygdo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2ojwuwgur.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2honftqvu.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2bribyvlf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2iqqqqlyl.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nxfcbgix.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2dgywbblc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2dkqfdbun.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2mojbpjkr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2elrqgagw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2uzeywiuq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2rcjbuyjy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2uyspfekx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2atfyozhc.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2tqldxojy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2qyodeuyj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ojfieexb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dvfhezfb.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kfytjwju.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jslffjog.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dspuccnp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gnwiccsf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2kxdzbvoa.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ypinwmwj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ryzkxhms.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2bgpljehv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2vacxhgqs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2bjpqmzgb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lqfqeoah.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ksdnqykx.html


<!-- 参考信息 -->