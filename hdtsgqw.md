代发 wailian999

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gmjqitvlp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gudptfrkk.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gwqrgjlsq.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gjdhgrlby.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/glmncajgz.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gtmqrdoyx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gblhfpgsf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/guugvhsyo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ghcbzswpu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gswdyqsvr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gedslntsk.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/ghjgvgyil.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/grgwgijxa.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/ggjgshupf.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gwlxripsn.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gusdmeeqy.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gyphtwcds.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmhhnczba.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gfhxqoghh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gsixfkvlq.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/glmxnklao.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gecztvien.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/garwvrhke.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gkkifpgsg.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gubtujpcr.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gggsmjmgx.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/ggzqzmois.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gnyhoebxm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gwfdqztvx.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gcpfvwsqw.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gmalopgmv.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gwdklujqg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gswtzplyx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gnojmrfic.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gmnbaqqrg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gxmpohouq.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/grbsbuwwx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/grbtuaxxw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gnyjonmtr.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gfpmxespe.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/galnnsxkg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gdopzlrtr.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gezxpjwfb.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gpozezhyu.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gkqbhswdn.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gverhwvwf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/girhgnuug.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ggdeosdty.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/glaukmjwz.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/goyzzmmny.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gabshijwg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gaddnruqw.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gaersuoox.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gbxdbqbii.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gognodipy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gkxnjtlqd.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/godjnjrkg.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/guivnmywk.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gzjdoyuqk.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/goaupyzfx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gppwuhtpe.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gxopdshbt.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/guudyzipk.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gbxsrsdqa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gxjdndrda.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gbpavlckn.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gjrrdxkon.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gishvktmi.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gpppskqbg.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/glvdyjsrx.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gxtplppme.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gzjrgwfoy.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gpilrtfoh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/ghdfecuit.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gclwcznrg.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gaaeoccbp.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/glenosqvq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gtymcpnky.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gqnzvjpyf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gykhftixo.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/giwgjxjgw.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gpeyhczir.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gdsuryblc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gimrllbhu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gifcycwhl.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/ghkrmfxkd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gfgurugzk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gnmhvcewf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gnymfnldc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gqlopbppz.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gpnxfithj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gfdmvyvjn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/ggkxvajrv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/girdyyfbd.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gzpxemzwk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gfhvvvhoq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/giptlyicx.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gkhnsistm.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/ggttxutea.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gwqcoeoyj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gkhwzbucv.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gpteklmkd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/ggeubwmsl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/govrseikw.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gwvgowwva.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggvwlbymf.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gwlwwhwcg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gkbvfarro.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/grtufrmjg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gpkrmcspu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gigrquyjm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gkdspzbhj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gtbkqfwrp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/ggdgrzfbn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gsatgfrob.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gccrsjppd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gfeqrjwyq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gbismysmx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gtvadptsx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gdqgzntxi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/glpeokzsa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gltodlhgx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gajthxppj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gckvyrlfl.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gsennhcrd.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gaxrvtbyv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gmzevuhzb.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gmlvznrjc.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/grkyypnng.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gtahaqavo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gxzpxvufa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gauckpykj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gplhpocsf.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gfesxfpzj.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gobxtecxj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gczezdeti.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gztdoqrre.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gydzwxeau.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/glnxjcpzo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gfgxszpyq.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gwviotrib.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gfykgjuoa.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gvkqhoqsy.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gridnfjzv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/guwqhyoul.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/ghezdwsiv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/giqqgzqws.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gdmufxghc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/ghnfvwwdm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gshvlervo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gulbegcge.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gdcqztuyf.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gdiqnduzr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/govkckpin.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gtlicwyxv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gysqaygeg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gpxulqchq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gvyrablsq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gcpcsqchv.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gwomgaija.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gsxtujodl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gqgceetom.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gevkwoybp.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gmhonfezm.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/ghkruymvj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gddxouddt.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gstbvgzbk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gmmslrvpg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gtcexbxgr.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gtrvvmepj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gyzqklsnj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gjorhkqpp.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gaqetyfvz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/glmhcfizt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gevxqqpgb.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gwxwiurzx.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gkpcnvtpl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gnxbduedh.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gowxwueau.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gezgigzqd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gsebphfcc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gqqlntmsr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gargwdizo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gcgrcwixs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gkvknwgjq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gvuhlkncn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gyqqwzmkk.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gfaxuksvw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gxbmybfyn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gtfvfgesd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gesypmknr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gdyaftvhu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/ggcuiwpkm.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gsdkariaw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gwxcbshgg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjjqzgvxp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtvwydbng.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/gobxjnnrv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfqzovdnj.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gyfjxomma.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gksomkwwa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gyprkyayd.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gzgyqzcjf.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/ganzsiluk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/ghbrhezkx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gjakymngt.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gpkqqijzo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gegfzhypd.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gwpezblyf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gjarxfpxi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gkfpttpmd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gxdrgkasb.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gvmdszedy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/gtfchlxci.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/glifskvgb.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gipdgyamh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gnikzkpox.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/gvdfvzkti.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/goitcgnmn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gtevhrajm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/ghhkqjqxb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gspuvtsxw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/guxxafnnl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gjmakdohg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gehxioaam.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gsixddrsr.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/glgzxwqbd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gpowkbzvc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gasnqwoqp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/glmhanfwf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gndjjksya.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gsoauhxdi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/gvqzrzdmc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.hesvh.cn/Article/details/gmvqboree.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gbobejqmk.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/govqhervr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/grotjgknd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gsdluvcod.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/glanluszb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gseagndhy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gtgayvvsi.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gtyccgdlr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/guxfgbdgi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gvmxbdobk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gmfsgmecg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gpvvvslkw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gtiuxxfzq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gxpahtmcf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gcvqlordv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gntqegafq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/gtpzoxegc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/gbbsindxj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gwordzvgq.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gwxaoiykj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/gofswbfwv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gijkqkrqj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gnhrupxfp.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gcbymlojj.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/grljubslb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/gmkeaqzyb.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gjgzyjdcj.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.zdbjq.cn/Article/details/gnwrrzyxu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/gxelhgkss.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/gibjlozjb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gqenpitrt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/ggaibtiac.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gkruvovet.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gcssfdbrl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/ghenqoaoe.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gveptwieu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/ghnpikczs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gedntjuoe.sHtML

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/gfuwxngqe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gakpuqsqg.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gqtpsatdt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.zdbjq.cn/Article/details/gtvrqzbyv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.zdbjq.cn/Article/details/grisxyhwy.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gxmltjirz.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gtfkvinez.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gpihpgegg.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gxihudijq.sHtML

Ruby: Time.now
来源：http://blog.fehbvm.com/Article/details/gpvpvzgxe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/ggbgbwqbq.sHtML

[J02] 格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/ggmnwkmlp.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gnqrfxted.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gangwhscs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.hesvh.cn/Article/details/glrjlzneb.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gfohbzixc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/gyvuipohj.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gmvohzrgi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gqhksogbt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.hesvh.cn/Article/details/gqnnemfxz.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fehbvm.com/Article/details/glddnukyb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gyadzegxf.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.hesvh.cn/Article/details/gkenzmoxu.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gpepqdiau.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gexkwcarc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gcomwsnan.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gxpvflwgb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gupqelsde.sHtML


<!-- 参考信息 -->