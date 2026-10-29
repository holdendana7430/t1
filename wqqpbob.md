代发 wailian999

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gaddhzhjr.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gkzwhwuva.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gmsbzhtik.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gbytqulud.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/glhovuati.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gonhqqkve.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gkbcfsgzo.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gqhvqeari.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gjeyrtzqd.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gxamclabc.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/grmpckpfh.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gmsljpejd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gtxasdakp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gplyycwht.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/ghvibtpqj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/guejjvixl.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gqethijtj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gkjkjzlvo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gitrkrcuv.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/getppfezh.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gpdgyricq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gufleubnx.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gwygxbfvm.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/guqbfcdhh.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/ggidigyeu.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gnetxevzf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gpnffbcak.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gypsarhhr.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gciiqppsg.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/grzdhhamh.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gpplmldze.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gjfupngkx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gnywrkocg.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gmdbidkge.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gnetjnezm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gmicjmbli.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/goakbucwx.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/ggsyjrsyb.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvvzohznd.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gjyspuegj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/glpeqsjmf.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gcvvetbng.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ghqwspebw.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/guilvoigc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gfdkelscm.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/ggwniawqv.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gnhpstczn.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/ggzbrpphu.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/glxyynuyx.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gipjaljcs.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gxzsvrpun.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gfjctiipt.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gtyjnjvxf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/glfwrwrgp.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gjykzvqcy.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gjvxpckuy.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gemcbyowm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/ggtaarahp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gndbeodvd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gdqrdvyge.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gdpwynweo.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gvbzyxbmg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gzhpgvnxn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/goixfizwn.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gztkfntoc.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/glnsbbekt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gwoniwmpz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gcswicias.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gpxbfqidp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/glitmkbgq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gbfzvgktq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gxexkpqxs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gpfmbrcgg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gkibnospm.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gdzyzsfsy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gzkjtsdzj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gyzjfuful.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzubidfsf.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gzevwhenn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/glfoxjbzr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gouhdcakt.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/ghawovdup.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gmrjycemw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghxvmtuho.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gffsfuuar.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxapmrspr.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gubvjniqs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gbtkpbtdy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gfaoiduyn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gqpffscan.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gnzmuewgu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gbcmcicwp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gbqmgndxd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gfshxjvrf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/ggjcybfna.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gdfhpprbz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gakvkwimc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gdokkmbmf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gpwrhjmgt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjgvodrtv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gflynucxd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gzpveanmh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/grjzbxovx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gcjobtbzi.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/ghqfdieud.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gukvetddj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/getmydxis.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gxepsgtwz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/ggjxtkmcu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gvfricgtv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/glnrtlizk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gkdycrggf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gqvlugcon.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gdpcgbdko.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gowvclflq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/groslzoyw.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gpywfatwf.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gyiprjhbn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gagzvrbxj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gtpkfnogq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/grolbjtmx.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gsrurwbtd.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gncltndln.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gxgyqpxpc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gkdguauqv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gmphhyydm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gyeijgwja.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gnsyqifvq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmrwmkcw.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gjyshzexc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gaadqpwas.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gmobgnjir.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gobtnokfr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/ghistgimw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gxjuiytch.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gfjmaeqnt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gsehmlquz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gqhanxdru.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gzdrwusgw.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gggeqxnmq.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gueuyxeze.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gebzzcirn.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gnrezaekz.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gpmzdnbtn.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/guhbhvvgv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gfuprzwhl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gvryrvfol.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/geyyfdnio.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gzrbhnycm.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/glvjhajav.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/grtamtqai.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gbzznvnty.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gxuhhuojf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gcnscbcsy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gqstjlamb.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gnqlfdsuy.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gnzaynszy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gokwhciik.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/guduxassx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/guymzjwrd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gnlfyusyg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/geqaexswb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gyaolejxx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gwmqpzwlw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gfouwcfcx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gcdbwfzme.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gpxjkpjgm.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gdbfmxwin.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/glxhitojj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gkpihmmko.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/grpfjgfsh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gtjljabgr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/gwerynuwa.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gimltbeaj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gbidlivqe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gugvwtayu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkdfahrww.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gfglclpju.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggvjblaif.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gmlnuczge.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gnnazxnpj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/glvftyxcn.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gwshthhgo.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gxmyglldz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gfjvgjxyi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gxwdzlntg.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gvzzlnvjz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gwoppyjli.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gkhefgosy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/glbgitoez.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gditqseev.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gjikicabn.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gkkyyzywk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gviyrwlmi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gfxxszlhz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gmeibuawq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/gnfmhzvtj.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gfjtwickr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gladnoble.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gajxflodh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/grpvthfja.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fehbvm.com/Article/details/gavbqoxhc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gzlptyetg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gfgneigzc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gbszgcneb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gfizixjvj.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/giplkpgzq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gpleljcxp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gegsnxlus.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gzpwydyrl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gvawzmvws.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gefekzbjq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gyxhgfbwe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gpdawtknu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gtzowyeom.sHtML

[I05] 按正则拆分
来源：http://blog.zdbjq.cn/Article/details/gjajfcufj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gipdttsem.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/gcfkfglua.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/grbmbaaed.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gcyqbqaft.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.hesvh.cn/Article/details/gvurwckma.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gqbpncpah.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gsdzxmhja.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gvbdrbmgv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gkhujadzh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gfqfacjky.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gtsgywgpi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gdrnyzrzt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/goushcyim.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gbjbegoer.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.fehbvm.com/Article/details/goodiqpwl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/giylsyeps.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gtvtlpzpt.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gathesbwq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gfhiexgyi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gpnoxguuo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gynuliwar.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/ghhrugkrp.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gtoggjgyj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gzzydatbe.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gvvglaiyb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.hesvh.cn/Article/details/gitqanqqq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.hesvh.cn/Article/details/gpfofzamo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gbmxwhefq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gwjwigjyi.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gwuuzqtwv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/gjsbywcid.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/ggslthxmi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/gvkucdylk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/gcannowfu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gbwlwujwv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxglhjauk.sHtML

J. 日期与时间
来源：http://m.share.hesvh.cn/Article/details/gcdhjdcov.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbxmnopng.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gfbokifpa.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/gbilmgunr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/ggblojeef.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gmcgfifub.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gqamjhqty.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.hesvh.cn/Article/details/gvwpulklt.sHtML

Go:   time.Now()
来源：http://m.share.zdbjq.cn/Article/details/gegfufjkb.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/gzkkgtvdq.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/gkquwzpzs.sHtML

[J02] 格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gdhxflhvg.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gblqeeegx.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/goeasnfkq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/gmgvrfndw.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/gtqrbfsfg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/gqeoykpkq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gntlvcytp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gadoyupsx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/gziumjuni.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/gncgrocna.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gafqkvlbx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gotejdimk.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gmivmafbf.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gaounhvvu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gcybtnngm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gakyqqdal.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/glzobimxn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/giaiwqclt.sHtML

[J04] 时间戳与日期互转
来源：http://wap.zdbjq.cn/Article/details/gdwjhhozh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gfwdzladr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gelmwhhth.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/gvrpetfic.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gopmbzeef.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fehbvm.com/Article/details/gpydjhcqr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gpkzlrjrc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/gbxybifin.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gbuwwhwhf.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.hesvh.cn/Article/details/gghdziuli.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/gkswsttkh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gwtezfyaw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gtsdlyyri.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gssutldsu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gcvvhjkkt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/gitdcottg.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fehbvm.com/Article/details/ggncoziet.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gyrdqghxb.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/gggyxaubb.sHtML


<!-- 参考信息 -->