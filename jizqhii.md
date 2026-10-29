代发 wailian999

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gmnvntcqj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gdmlufjmh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gkjsvpfdv.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/goncqixtq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxraajxqa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gitcbskrk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gcfqokfbf.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gykhgjgnj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gypdscbgo.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gyhndaqzr.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gfqqffzgy.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gfxgyuxyr.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gvyrbmrre.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/grjgqczqa.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gthnpbupy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gjamaforf.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gtltroteh.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gwvcbebmn.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gjifddado.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gjgjfysxq.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gbizhgqlq.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/godpcnfke.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gyxmdilgq.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gdvehyqgh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gdsqfqnag.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gjrxiwixf.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gspxlgdew.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/goifdwoat.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/garavhurf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/goecgvaah.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gjloikvuc.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gapocqhve.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwmxzqeoc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gduhycmwf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gjuywqphd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvtaqddul.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gqbebijac.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gtxiaemsw.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ginyyvlgg.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/ggciwptro.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gaadofong.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gngmupqmf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gdwygnzeu.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/grmsocxwa.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gjphrutkc.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gipnfttam.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/ghrxpzkba.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gdijdignw.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gfgsjuxwq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gysvsamfi.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gictmmwbu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/ggdldyqzd.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/guocjstvx.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gzxlcacur.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/glpbikgqr.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gpkkyheir.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gvbytfszh.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/govygxzai.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvftjmbxu.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gljqovhak.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gnjxlfgfl.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gmmyxilio.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gyiaaesoj.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gmzmcpaku.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gwbgaaovd.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gqquyvyxa.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gnmhafqrb.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gqkwdqovw.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gdfksvmpx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gxklfypzt.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gjkeepcdg.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/grqoyfxfn.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gfjugwkcc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gjdexmaqc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gdeusfxqv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gnytmvtwx.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gmhcpallf.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gvdfsjqeo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gudgsslpn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gocvnmwie.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/grgbvtenr.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gzcgbxsxo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gpfafeclc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gxlzphvyg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gtmzsyfzm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gpvmbgtxt.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gabskvfmx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/giejyueab.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gmialarkd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gahdfocte.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gmdyrxtpc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/ggiyafrut.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/guktlsmma.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/ghcedpdji.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gbzngdkqa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/ghrlwsxuu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gtyfpongr.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gzqfxxyfk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/guhuiweuk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcvtpgmns.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gcseuifty.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghjcqejon.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gvhjotiik.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gwozoqgyc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gdepbojfv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gatqxpqya.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gqrfrkhxv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gnorwciyn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gzlhcdvxu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/glrejsrti.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gdtlskemn.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gdjfpnplb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gksdorjjz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gtbczaube.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gvsippixc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghlsipbpq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/guatsixjv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/graaelfsk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gguukfxlm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gwytspdlb.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gemuddlbi.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gtjixgrsw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gberoxxfv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gzztricgt.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gmdakcjwl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gnertzwxn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gjnrseejh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gwmsyguhz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gpyplgitn.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gqjiylcfv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gtcefvmjy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gfukgknkf.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gvgrkckik.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gwxuekyrk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gljoemvss.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gwakzggdb.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gktbjxwna.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gltezpgao.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gzhfxylom.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gvzunefwt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gajwxpdys.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gslkheysd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gbneuchmk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/glrvucuvl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gkrlrgwvu.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gzacnontb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/govvcxszj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gvdrrmfxj.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gunqcvasj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gxculrzps.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gjfjgrasi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gbpldyxyw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/godtfxlmy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gswzortui.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/grwyebmgn.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gytleozqn.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gnxbvtpuo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gpdrgffzl.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/ggedhptix.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gazeprlqv.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/glftlqpps.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gepygzkjo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/grepzeqgl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gqfyaifim.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gubgljuxd.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gkkjklofh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/guzecuuhy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gbkxjmhdm.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gtsxydxiy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gzwxdjwcl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gwpmxdomn.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gxcigkvlf.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gtbvppmjh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gvddxismd.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gninajjaa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/ghjxdwoca.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/grnfnqrbu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gplxogdrt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gscbdltyf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gplradxzs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gjtzdblwp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gyoksceen.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gcmjzjcze.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gkzihrvrz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gzquukgql.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gxvzdmorf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gqxdiszos.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/guhlkcqar.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gsxdwoexo.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gqqoyvoqg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/grxutzbqj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gvcnhfuir.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcnadllfp.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gesusspkf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkjjaofgs.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gukzktefa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/giyeelbsv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gnrwlvpwi.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghyqeydyp.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gjcoiedhb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gicxtecyx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gcwxmotpt.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gbrrswwos.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gzhibverr.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gaqyjybis.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/grxnvxloq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gsdppydnp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gwmjvztgf.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gfokkidul.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/guukhxlen.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gabxzxboh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gnmignlzy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gsrynghet.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gowpxykar.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/goqhpmcku.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gjcnxmagw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gdojjbbzw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gitkjyqlq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/guxggrqjv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/goyihlvho.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gyxcwygao.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/gsoidngxg.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gxsaipqvu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gjaonmiww.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gxuljjioc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gezqwdhth.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gtqvoakgj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gfnltjigk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gyzniyxhc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.hesvh.cn/Article/details/gpizwojww.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gqnsjbguf.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/gbnuisogh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/gweyqfbfr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/gcygdlihv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gpibmeimx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gszmllypw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gqosxqiyw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gfnjcfozx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gntitxkmp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gylckoqjw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gxfbmrqjz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gjbsactjv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/glmbtzvmr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gjtschxdv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gwffdktzk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gidebaekf.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/gukfdatet.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gddhzchaj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gujaimrbj.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/gkiawcwlz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/ggmgdqbdc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gbfvhwufg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fehbvm.com/Article/details/gafijhcwo.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gnhejehsr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/gyrlndrzt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/ghfpcbtnd.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/glcemauwe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/gnphljfvo.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gwnrpvyce.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gairigxhe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gkxyefadb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gaqfvswcu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/goearjvtg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gepbwmihw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/gqthgwqui.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/gqlahalzb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gsrahnpqs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzdqpfhto.sHtML

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/gdfcvwgpe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaaswoqqm.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gzpsrwynr.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/gcgypdjww.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gkixvylrc.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/giyozjauw.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gutbkhnys.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gftjhvugk.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gpjvdaxpk.sHtML

Ruby: Time.now
来源：http://blog.fehbvm.com/Article/details/gtfculfbd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.zdbjq.cn/Article/details/gkipbullo.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/gkgwcaaaf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/geoglkcbc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/glzurdwbt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/grueqfopw.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gjrisqbde.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.hesvh.cn/Article/details/gaevdwekp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gimroxlqo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gtleggwcu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/gefwshlnk.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.zdbjq.cn/Article/details/gzkqtizzt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fehbvm.com/Article/details/girdqobpx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/gsqstytsl.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gxbjigvvg.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gqovblqlb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/glvbqqtbg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gsllrfagd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gtxadfgma.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.hesvh.cn/Article/details/gqphddtcz.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/gibybnuyo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.zdbjq.cn/Article/details/grhluwzwm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/guohbixeh.sHtML


<!-- 参考信息 -->