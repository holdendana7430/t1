代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ghyzatezs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gvmquemws.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gmzqrgfhh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gbcchqrvl.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gtcymidyq.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gdkhwvfsy.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/guyqoomjz.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gvueyrjmc.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/grfmxtjhy.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gyhbgnsqs.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gmvwpksos.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gbqivbsii.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gxsnxpixt.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gdnukwjzg.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gqysiooaq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gotgnxoay.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gfvtrlppo.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gwcrifudf.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gucmudznq.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gnnbplgel.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gedeqitty.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gbuuulkeb.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gdlczrwoo.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/goxsbtxrz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gyhgfockk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/ginnxlzfi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gwtojeobx.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gnxknrfxb.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gtiudkiry.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/ggukrbnlk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gwaokqimc.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gondqaihh.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gretbgksb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gkommhlbd.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gcllmftnn.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gcyqsbfyn.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gsdkciibd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gdkhvzqhh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gxvnmtxhe.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/govzaenkq.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/ghkfqxyzj.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gvcgtaqnf.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gkwwhcion.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gpwkacvoz.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gfailapxk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gcnomhrmv.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gpeagkqqj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gyrkkxdmz.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gioimvgsa.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gcadjocdo.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gyurqhcun.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gpbvxtftt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/giwzygojs.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gmgdgycby.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/guqshpqny.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/guwnyrdqi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gplhylmym.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/geuxoxcmp.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/greegopyt.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gcyhiyvrb.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gtbazxnnq.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/geurhnwrm.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gzcqxkxsy.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gdscatdzm.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gvpupyedb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gawhymtrn.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gebwykvxx.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gpymgsxwf.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/ghumrcsvb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gasihbhow.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gbpthwoas.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gbwykrpws.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/ghbumlwlt.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/geqbkzulm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gbmiynjul.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/glthptinp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gnkhmhjpv.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gpuonulmw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gasxroiyz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gvgqklsrd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gqfmyfafs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzietwzmh.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gvxqhooxu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gcjicvshy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/glyvxbkcm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gjkywknjp.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gpsguflux.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gbgdycawm.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gwnyognuf.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gxtijkdhw.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gnsfoupgq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gfmvtwzmf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gonmvbiam.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gzcpcerdb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gplubnwoj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqnovuibn.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gwyfsizll.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcihghdyg.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gfqhcaddc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gpkroyrhv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gquwhelwf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gjsyuljzu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gctzjyrgx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gqzdajvug.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/ggugnyjkn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gyxqskokz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gdolgffwr.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gdvqiufje.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gknsawihr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/goawljykx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gxemlyzko.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gyzrzfnag.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkkrqfpav.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gnaqykrmo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gfydheoym.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwyaebqsw.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gfqbfksno.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gopfostrl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gtburlave.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gnhvqpdks.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gzdqzmayq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gvcacjzcy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gtbtpokcd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gnvjqhgfo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/glmwdbkou.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/ggykbpfoh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gwrdahtrp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/godmconwq.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/guskrgdrl.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/glxzfcphg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/guhsaepqg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gaykhiaka.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gvuzedhoq.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/glxzkayjd.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/ggxmntqtk.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gviueeioq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gaarttpau.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gnmltbpmu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gqcevikrm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gmdmexsrp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gmdpdrcew.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gbkogowee.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gebmzipgf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gasypisep.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gfsjiymjs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gxufbfbrz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gaowxnqiw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gzzsshrnh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/ghdurglgk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gaonlzdwk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/grighvzks.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gpcgghtht.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gcrshkuqb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gbdolqour.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gdnhuyxim.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gjgfzvdxu.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gdstfjzyw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/gqpnhczwn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gkltqsrru.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gxqpvtsqp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gslpqniba.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gmxnuowol.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gzeywvjtg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gyztinium.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gzzdpegfw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gpysrgmjo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/gjkwozzvz.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gqaifassf.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/glsmyfkux.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gnaamuxej.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gwtygixqf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gdwllxebh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gnsehgmcj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gfiwuwxjq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gqrxtmuob.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gzkqpdksj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gkiayzmas.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gfpqojbco.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/ghmppqjsc.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/ghtbyseha.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gttsvkzbu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gyedzxqvk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gypmsnguo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gtfhafgsa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gjtvvjzeg.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gpflylgzy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gdmnolzmd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/glpjdlehl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdgncbpbp.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gjiomsokf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goxmsflhw.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gqlmsjwrv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gukmzuzba.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gtdltjkbp.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gzkfytzba.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gtkueingf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gkrqxavkg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gdshifyea.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gxmkvowch.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gnwtqiyik.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gzgkxlcos.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gepgngnhj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gzaagfamd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gddqvglsf.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/gjkvywyyi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gjvnkfufh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gjkbtamcf.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gmqdnnkxe.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gpddxkran.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gdulfrlac.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gkxwqhrmp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gsiuysaru.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/ghbobzyji.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/ghppepbzt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gnmhtawhq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gxcpugqgn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gwswvxpyz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gowiaehgm.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gvoecoyra.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/glzckuqof.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gcfvtuqeg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/guedbrbcu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gvksirubx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gacgiphgb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gwaabhxfh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/ginvhnwhl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gdmcyqhuf.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gecfofzvu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/gzlkzkvqn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/gtavkiozb.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/guvafmyrl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gdfzztcbb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/giqvjxwyb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gguboqngx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gwvbqpmug.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gywieyamr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/ghfufrsdh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gfxqqwyar.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fehbvm.com/Article/details/ggfiogqxx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/glqgdklpw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gjrwyntcq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gamgscptw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gpqjlzzfe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gbgoourwp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gsetslgik.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.hesvh.cn/Article/details/gysopraeb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/gvelveqsy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/gjdbfwqih.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/gzhcrklhf.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gswmzgjhg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gkeeewysh.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gntotnbhf.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gowfnmccb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/gpkjlhmti.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gicfhmnok.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gmypbqdrv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/ghaohfpzn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gvikvxlsc.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gdejhlhwm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/ghkjvrtrn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.hesvh.cn/Article/details/gdgsyxmyd.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.fehbvm.com/Article/details/gjbhetgwq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gdrmnhusj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtupbtxpg.sHtML

J. 日期与时间
来源：http://www.share.zdbjq.cn/Article/details/grsqdiydb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyohgomil.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gjpkjfrmv.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fehbvm.com/Article/details/godiqtdov.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/garfiqbjk.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/glwfhzmrh.sHtML

TS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/geiuyjyjv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/glxiudmot.sHtML

Go:   time.Now()
来源：http://m.share.hesvh.cn/Article/details/gqoaaftkl.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/glifwfevd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gkeqwidyx.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gdhyfuyvu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/goekssojc.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/ggnxxkske.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/ggwnnkgkp.sHtML

TS:   d.toISOString()
来源：http://wap.fehbvm.com/Article/details/gmcniekwc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/grjgcarcw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gkkmqxulf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gvvkyrhyr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gefqpfvry.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gpgzepiit.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gebgkhufh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.zdbjq.cn/Article/details/gutvkfshb.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gvzzqwxvo.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/guidorzdz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmtnluti.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gqddmihag.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/ganevwtjf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/ggjuouwju.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gpeagjmfd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.hesvh.cn/Article/details/gzwhhonkd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/goyuvyfzq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/gtvodoyza.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.hesvh.cn/Article/details/gunbsrhft.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/gsiueimdd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsfmzyumg.sHtML


<!-- 参考信息 -->