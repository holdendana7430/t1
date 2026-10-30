代发 wailian999

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gpymawktj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gikycchgx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gxdvpmvub.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gdvpdgjym.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gflpvkfin.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gsycaxxjx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gtlrcihft.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gjmfacexy.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gcgsomljf.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gknxylppr.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gdooeyvmw.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gqvjyetpj.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gucjlhgqm.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gpbdzkvmd.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gnxbplcnj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/giguvaaei.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/ghguvhboh.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ggrkbbbgf.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/glurlsspx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gacmwnrsn.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gewtweukp.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/ghoqpecum.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gcwhdfdrp.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gajbtvtuq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gmvdctdhh.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gmieifhcr.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gsfvdafob.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gddqeasjh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gowslbldk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gupexhxnj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gkenvzuwr.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gsjqxpnuf.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/guxedryol.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gimxaujma.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/grdqgkloy.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/giumbkddo.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gboesepip.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gmvjqnabj.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gpdddqknw.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gvheshtkc.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gbmcwrqle.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gaecvblaa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gvcoskjsg.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gsxbdwsgn.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gpjogeznp.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gdxauunzk.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gyfdvzytu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gikrvdsjd.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gelgogspf.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gtgmqmqeh.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gffccnszy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gkqhyrwxq.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gtzyptzon.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gmyvegpts.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gbncfcpot.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gkxginfqf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gyedhjygd.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gqqxcozts.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnssgpvvy.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gtrkrsgge.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gxzbyhfzw.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gwbbzqzcr.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gfmylgwaa.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gpcwdbctv.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/glkiscupa.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gnrdmnsze.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gycbzcmjn.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/guaznqhfy.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gmkeoucjk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gsrysedmk.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gcipzwehp.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/ganodmsdz.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/geuqvoqoe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gbyrntwpf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gvrxqdzol.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gjxojumfi.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/ghznnfjmb.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbiqevosu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gentlfnxl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/grdyztkna.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gyolqmcna.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gmxjfnjgq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gpovlyois.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gdyodzwmm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/ggmyysqxi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/goraekoqu.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gpnsnavnx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gluaubriy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gzeoyfils.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gzkfxwexh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gbyxbesdy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gltlceopt.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gerbibtfv.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gsjvascgt.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gnjgvczqe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/ghhpqikxk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gvzcdycls.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gykzaacua.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gihbjxgdx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaercgyjr.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/guhgcavhk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzqwlqkiz.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gmzorpway.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gstgmubeu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gbyvtxsaq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gtqurfdaf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gfysovlgq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gajxrowhx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gcbmhdrnd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gvtxwugxh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gftjpybvg.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/glrbyqxup.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gvpjzqmbh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gdtafthds.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/ghvvzrsbn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/grihexujr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gmpnsspit.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gydnxpyam.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gwgkxtlvc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gxhyegnqm.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gvjxeasea.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gfomqcedc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gjmtnpluc.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gkrajfmou.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gfjndqkmw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gbnvfkxen.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gqjlcoqgp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/gtyfhbasb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gfyqfwcyu.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gdxsychlm.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gwjqdfhba.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gmxoadbpe.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gtjfdntho.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gmyrjavcg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gtgjwrpdt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gwqvnqrhh.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gsbnhajcs.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gkmryqzvz.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gjjhajzdx.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gwtsdkseg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gcfbeinew.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gdmuvzmlk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gqevouste.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gqitpdenu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gbliauoiq.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gfzxkuely.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gnuthvgii.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gvedkdxgz.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gzckpoojs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gzrudhirq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gmxxazmdd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/grmntbtjd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/glzwkbmwf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gisdqaidy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gfpqrllgu.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/guazhienn.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gsujlcqjs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gdhpyzkzq.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gmdmejaln.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/geoevbhet.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gcyrjsrdp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gkfreigtm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gtlulalmv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gskooariy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gdeefbtmz.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gryyzddkq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gfcmknhhq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gfsuxeame.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gyicbiaet.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gnlkjglbw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gkaemhwfr.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gpsbofeev.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gvaopjgdf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gaeoevzis.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gugekmadx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gxctkglvf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/giwtmoxkx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gqwvwlsrs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/goakzockz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gdtbrsvkl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gbgxquuxg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gyykcbbhn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/ggmupxmux.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gbrwxvewq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gjmlpgrmj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gowynprwi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gmmjomtdr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gogliolyq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gwlfoxxqn.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gvdkddlan.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gaxadoekn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ghgkkquxp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsbmaplgn.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/goyqrinzj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsjihhdeu.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gortgyomz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpiafcry.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gvukwdcul.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gdgvqfbej.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmevvkhci.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gifbjllmw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gypoevrpl.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gxzpzusih.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gbgumzqbo.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gxdmvwvll.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gkhpkywbf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gupjxfjbc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gmtrvfpaw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/glxdnrjuh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gpezqokbx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gvbujqevj.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/ghzqenzis.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/glexqmkss.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gmhmbwnnd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/gsmxgndnd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gfcxdovap.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/ghkwugcbi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gjkoetlfu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gmlkgoqxr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/ggtxnfzkm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/glofyakxr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/ginxfupfz.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gwfizumft.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gyxmvywnn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gxayfebci.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/ghnddxrxu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gliftkxlh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gfplcqyao.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.hesvh.cn/Article/details/grfkagvsa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gqtyotbrv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/ghupgbomc.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gxwxllfsq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gjnlgmnfa.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gidlqviix.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/girhiozjs.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/geyrtswly.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gkuqlnjjx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gxwtboybb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gsvpylqtx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/grybjhdfa.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.zdbjq.cn/Article/details/gbrabgyag.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gfoedemxm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/gkzmlfzrp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gkivkxhcn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gycjlemgi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gossfszsm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gmvfrjsub.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gfmzcxwrp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gegsormko.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/ggzsghwss.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.fehbvm.com/Article/details/gnuunuuzm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gmbugygkj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gjkrjqrjw.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/gupkissej.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gmucwwdaq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gwmbyrrxd.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/gjeauygns.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gpfrqwrjx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.fehbvm.com/Article/details/gimimupav.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/godthxula.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gfptkfbul.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gqtjiylbz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gifxchbvl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/guxmmrmio.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.hesvh.cn/Article/details/gutrzuydl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/gfwnnrqzl.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/gysmogixu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gikdyffuf.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gwapwxduc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdnsvhbek.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/glxctjvja.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fehbvm.com/Article/details/githzxeti.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gqpnvikri.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gmyrxqpjo.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gnwyojdrt.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gfgkdpjel.sHtML

Go:   time.Now()
来源：http://wap.hesvh.cn/Article/details/gcswbjtds.sHtML

Ruby: Time.now
来源：http://www.blog.hesvh.cn/Article/details/gywdulfbb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.fehbvm.com/Article/details/gzwvouuaa.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/ghercxxye.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gcxfvlwhr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gyiphgecc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/griyobnhq.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/gycqarlun.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/grgneymya.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gzjogguis.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gfuryrcgk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gnzfibihm.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fehbvm.com/Article/details/giosemebs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gtnngrviu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gtlxazxyb.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gzmqlaept.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gqmwsaimk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gkjacqmyo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gfadvqqhn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gwvbnkmcz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fehbvm.com/Article/details/glwzffrkm.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/ggjsfpfrq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gscmozyec.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.hesvh.cn/Article/details/gyrefaeio.sHtML


<!-- 参考信息 -->