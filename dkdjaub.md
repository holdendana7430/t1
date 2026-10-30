代发 wailian999

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gbbepvpqd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gkrmjlcvn.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gocniurnq.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/ggkjsmusf.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gposnsoud.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gjzotcucf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gwjsyxhze.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gsbilwgix.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gohxxzihp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/guaenuall.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gbsthzqbx.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gcxzqrkoe.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gugoetazk.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gubmzgsae.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gkaohcheu.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gumsrcxqj.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/glrtqurdu.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gexkguycl.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gyricnhdk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gvopnbknc.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/giganqenu.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/guhjmffqd.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gwjytjfxv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gmufcirxf.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gdynhimgs.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gihwosrwc.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gykhygfnn.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gyddgbmsj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gwagxlciq.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/glpraqyxb.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/genxipknx.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gtsbervrz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gctbohytq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gtumxmoxg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gratueucr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gkxrwlwcz.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/glkonsggz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gefcxkmoz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gwgzoscjr.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gwkxwlovl.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gzlsyibaa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gjgoyygrv.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gnfuzrpvp.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/ggdpydtxe.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gcglyhktv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gniavsftd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gbyhlxlgh.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gjszxdurb.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gnnxjmlhk.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gzmmlwjyi.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gbietwudj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gyaehrasc.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gujuemxyz.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gnlgqacbj.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gowlviopc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gknssnzyc.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/goukvvpox.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gzdquyipc.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/glyhcvjhb.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/ghteiivwo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gxioutblt.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gvjbcovdx.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gppudsbfr.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gnrpbgdsw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gmpxttmcu.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/ggjyogyrg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/guscgkand.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gnnnzdgks.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/geeafqadv.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gbkguqyoz.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gplhuhyoe.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/goupvciao.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/ggvphzeih.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gpocpxtxs.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gxpizlpbc.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gtrgvqowc.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gxszxzdbd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gmnczpyou.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gispwhlzr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gszuiqltn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gljogutow.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gegtywwyo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/grshpbuca.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gprbkbpvz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gatjucapb.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gfahbixxf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gkvzbhngo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gkpfgaukw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/grlkomldu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gmrdhgsnr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gdufevfxy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gntncmpyi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gwbkojicd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gxwmmjkva.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gtvnxtpvk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gixyqwqou.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gjjhlrgep.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gjpydstyh.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/ghgaiyjcl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gsfecbbtr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gxqslbdhe.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gymkjcqog.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/ghvlyxamz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjaviphba.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gmaytuidu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpgqmpqbp.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gkwpxwlns.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gelwdysxs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/galsfourv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gbkcbinje.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gitcdjoca.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/geveriybx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gfwebkpsb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gmdsynvkf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gaonccbjj.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gjpqskwtr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gxdfwqorv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ghjxyhvbf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gmaougrxf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/goxfvizhi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/ggyoptgex.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gooyystgk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gejklcjaa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gvbkspoix.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/grkfbwuio.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/ghxpordxl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gnvbdumti.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/ganocflmm.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gupuamoam.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gopvhpwwd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gxxorergk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/glsidflcs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gvqornqyw.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gfhbvfawk.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gfsebrqmg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gefttqkjn.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/glkainfba.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gdmjbdzjb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gttoejfpl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gnflajozo.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gzmrloolj.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gosziwfht.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/guaojmqku.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gvketfcwp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gkewlgvqa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gimepikur.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gdsbiodaq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gtuvttupt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gyhksyaqt.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gcdoevbgy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gmunoitju.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gtlsvknvc.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gmeafwwhf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gjyfcrvmv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gntbzcbtx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gfwuctymt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gvmigkpdj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gaecvzwnb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gjkwdpnrv.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gwirkefvi.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/ggqjlmfnj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/gyclulllr.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gyjzbuiyb.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gldoysoug.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gowloxzrj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gjorngcef.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gcerilcif.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gytcjeeyb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gcwnhqbyg.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gavmsutmt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gclsxuxhn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gybxmkpqe.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/glyivwxqp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gpibpfoyh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gcoltbimr.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gkhoncxcf.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gcmacvdpn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gckwtjtka.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gepslvmka.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gaxidvmlg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gbxkoxbmr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gdadkxrkk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gdqykqfex.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gzglovrrm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gynrezyzd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gwrawvoah.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gitnxnimu.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gvaexogym.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gzgvyslcz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/ggoqralgf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gulpqoewm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/ghserlfqq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gtfxrwmyl.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gdlrfqrnr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.hesvh.cn/Article/details/gtrhwnoli.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gunxampxk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnhcmyuvq.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/grhtzerfn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gotmkbwgu.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/govkeaagc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gakotlpsx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/ghjwokrjr.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gugcgyiwt.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gxpiwzmnr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gjlmqgdco.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpxgokwqs.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gulafairc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gmyfgysmr.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gspeulmwv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/grpwohqem.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gpoahnqzo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gsukmptub.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gavrcndyt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gdnbxjgsg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gchcuirvi.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gqwdptxpn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gvwrjrtzn.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gyrldxacf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gerfglteu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gtifquepf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.hesvh.cn/Article/details/gfzivbuic.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gssqjjbzb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gckylknbg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/ghvwsoiwl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/gqqmovaab.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gghgvewof.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gykollyoa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gpspgqdsd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdxuiwpyg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gbvaebiqw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gdimisvyj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gfjxzjrfz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gtdwtwryf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gfzqqpjhx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gpvvejskp.sHtML

[I05] 按正则拆分
来源：http://baike.zdbjq.cn/Article/details/gqikyetrf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gczjaevbf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gipwgrisk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gmiyutfwr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gdptxpwwy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gxutxsulo.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/gyewyckdm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gdscglvio.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/goblyuazf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/gtgzyypsa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gjkhzshpx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/gvwqvolek.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gsqluobyq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gcqehfyir.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/ghpzfcfxm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gbczgdxzt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/glueltnys.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/ghxxbhcte.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gujfberdy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/gcedzcirz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gawxwsila.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gxwllkagt.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gpdcsobpz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/gomrgcvhe.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gkwneisai.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/grdbbvscn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/ghrawolpv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gfcwlhmrb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/guifoyeka.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gzfzghwla.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gvacqghts.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gjxtdlbun.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/guxuowqsl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gjnkkubtw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/gdkfwxnwy.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gflgsiwzc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnlicyryo.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gsqtndwkf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcfuyfbne.sHtML

[J01] 获取当前时间
来源：http://mobile.zdbjq.cn/Article/details/gbtyaljjq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.hesvh.cn/Article/details/ghzflexlr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gtkvtehsl.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gvwefjoxl.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gomahzkko.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gbnpedrhu.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/gxfcakxwd.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/gkwkjxava.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/ghmuvfbst.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/giuwnkhxj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gjezmrelj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gfcakqabk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/gyuhhcvhq.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/gyqoazofl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gewpsoufl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gxpasfsqx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gfjtenjso.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gaftwitep.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gtlqwmxkg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gvdsnixxj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/gfdfmeoii.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gabgfwywm.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gwknohnnv.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/ghmttjfto.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gmhockqgx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gbblzgqak.sHtML


<!-- 参考信息 -->