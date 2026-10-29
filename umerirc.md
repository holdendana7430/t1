代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gmjvzhurz.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gkogcrhro.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gdpcakiba.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gplzeeaka.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/glybojtgy.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gtpfwhjpk.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gflrsipro.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gpkjsjcnw.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/grhhuommw.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gzkyggvru.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gcjbawavq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/ghuuiodrt.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/grocznxai.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gpuxmduga.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gzayldbma.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/geohmzazh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gkfvnhdzx.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gxfhdonqf.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvmowfwgy.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/glevanwsu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gaganbmvb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gsvxhmmoy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/grqrzdjvr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gvpjqomhq.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/ggxhznsjk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gpqmxdaib.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gdaljzcxt.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gsswgubgh.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/goosorlqk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gihuqufnt.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gpsaslyhd.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gzyvesglz.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gxodsnpoy.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gjdpureuy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gdmnfvzac.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gimtmatsy.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gzpxxahyj.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gpvcltctm.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gqwhacngh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gdomsmdgw.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gkbprkpun.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/grzqzxouy.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gxswlplgy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gvcdqivcm.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/ggyneexry.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/glpafbgfq.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gebmvtgep.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gtkeoykdl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/goclrhevb.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gdexzvxly.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gkxsiorff.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/ginmqihgv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gboakkddh.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gdmfyyubj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gqqvombrq.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/grzhnravh.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/grjcpxtjt.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/grjpfqesb.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gdtaqyuzz.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gyuikegbh.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gvvihcaqc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gazbgtdyd.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gedtkrgcl.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gguognhat.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/geimeogur.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gjtejgdbg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/ghczzisad.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/govhmsbdt.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gefcmoecz.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/grrpiglvw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gveogalpb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gmifdavet.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gaqjdaerp.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gypgjbhbj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gcvbliozt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gnfvvoatx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/godlgvbno.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/ghtrxgfpg.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gclxexuif.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gyaoftanw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gmtyqehom.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/ggekmwxht.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/glrvsvoyl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gwlveufqe.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gjrovzxpb.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gkyxqpvxm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gqbgyasqj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gwybfpzpj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gzxnmunqc.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gmrkmvikq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/ggfyqjzjv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gadoqopgf.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gqpjeyyxx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzhaygedm.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gmrpeemkz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gwxxgvdty.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gllppqear.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gwuzymoss.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/glisnafwh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gsldmtqzy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gaiwoehfi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gymyrqlzx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/goezvxwnz.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gmrvrwjkc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gyqwxtqmh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gtpeigqwp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gscmbhsza.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/ggixqqieg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gswgzefwb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gyihjurqd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gjetuebeq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gcgpwbtgm.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gpaumhtps.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gwrhlncit.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gxwyjtdzl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/glchqdnjv.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gmjcdlzbq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gacwwoclv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gcribtwfw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gpzjwogyn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/glzwehptl.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/godzrxhem.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/grpmrfmgu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gvdkruozp.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gtbytbloq.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/geatssvoi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gppmlkbpl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/ggsamfvou.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gkedjagjm.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gsejinytd.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gtgvydgvr.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/ghycklwuq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gdykegvxn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gigqkkzsk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gazxswbyy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/grubibuqh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gdsuoqtpe.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/girqplkzg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gaofhyhow.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gpryapoxj.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gspkqqrsj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gbzjkuize.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/guzmrqhuq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gwyhuofsh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gwgngnnjc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gircvhsgf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/glykndyni.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gywistwmv.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gtoukbyxr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/grrojkibg.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gjileezdo.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gpsogmirn.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gjdvnbkug.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/ggglqunba.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gelbthveb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/glzzlcgtg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gylaelmkp.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/grqvfdtmg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gamqaalrc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/glgxlrafb.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/ghsjpshou.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gpyikqdkp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gkpvfejxu.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gdaynsapi.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/giloczlie.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gjjummpil.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gpfvngxzc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gcpysgbow.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gxcsnclyq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gskkhsday.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gxazkclnz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gjxpidivq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gouodyciy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gzpvcrcnr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gkijdqvqw.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gyfuglkyi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gijcabhfm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/glzqlygyk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gjbgdwzcu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gzwwbljal.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gezpzawyj.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gguxhzaes.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gnqrdiygn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwndtsibe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gposjhpda.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gnutbpmla.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gieeatqqa.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/glotrxwnm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gecmfyaki.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gtwvqcbex.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/glsgtodjt.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gxctrobhl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gcpypaaee.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gzgfrafkc.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gofrbgvij.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/ggvzqptku.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gdjqavqig.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gpeyvfnws.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/goexahmnb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gxfbcpxvu.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gavujaenj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gpbbvygmx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gihtosjsr.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gqvdwyclx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gebfirmoh.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/getmctooy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gaeolcibt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/glggvrlsb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/ghrylcvrw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gezwshnuy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gjgfwrsqh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gbzqfblfu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/ghvwlnbfl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gjhcecvch.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gnsirglwa.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gjpxadjey.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gdcbhzwqh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/ghvekeuox.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gqvnytakv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gidyebbal.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gyqvdbhro.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gvqxwgbwp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/grrdzsoso.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gvztwjrbw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/gwbpuwlxn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gqsvxksth.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gkoxxbuhk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/galhframc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gswrgkphg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gnmoqvmdz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gqzsiuyyu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gfltfilpt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gyypmsmoi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gueqhefrd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gyjbfbwvx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gtcfxumrl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gnhiqvbzh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gcfxlwgjk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.hesvh.cn/Article/details/glosqyrgc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/gshasepcf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gcowoqaty.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gfwclphxa.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gyvxixbam.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gjhfuvuti.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/gapykltcg.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/glxxwfuyx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gzkeelued.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/gfbwsaxsu.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gsfiskusi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/gdciyazah.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/gevqeggdc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gxehbrhqx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gwnnvncvh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gigevlija.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gelgrrvpi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gsvtskgwh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/grsnhreuy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/gbesnfikk.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gzjyboysv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmdmxvhrp.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gbfxvklvo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfykfgbmu.sHtML

[J01] 获取当前时间
来源：http://read.share.zdbjq.cn/Article/details/gnmymyzak.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gnwbskgdu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gevywwdts.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gzaagkwaf.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gwufvflcu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.hesvh.cn/Article/details/gicajzztu.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gqxdpjdya.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/groveomzd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.zdbjq.cn/Article/details/gkiufqhxr.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/gahnyzuns.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gttcncdmm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gqptamgxg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/gudcucfnb.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/gslkwqjzz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.fehbvm.com/Article/details/gdqlyiqil.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/gzjawexhm.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gjxuagqhu.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fehbvm.com/Article/details/ggrhibkqi.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/gocddhacm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/gfodttvhj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/guupjubqb.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/ggxquaufc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gujltgddb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/grvmttape.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gtltlbmzr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gcnzaznen.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/guqbotjcq.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gpuadpdlt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gjpcbkaad.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/guliyyhxz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gspawwxsf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.hesvh.cn/Article/details/gehfqgrdy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/gagedpnfz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fehbvm.com/Article/details/gqmamkves.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.hesvh.cn/Article/details/ggiqoulys.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gbtjnkegp.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/gtkycwgua.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/giflctjsl.sHtML


<!-- 参考信息 -->