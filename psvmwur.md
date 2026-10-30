代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/glleybscg.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gbxvqitfa.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/ggnagtwch.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/glzmgdrpj.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gvqsazelx.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gkcdexczc.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/ggltvuyld.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/guhlldaez.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gqrusaxkv.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gssvcafjf.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gsccywnhf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gouwxhqqt.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gohmsilei.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gkljtpojd.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gbwqqhfqr.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/grolvfjzn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/ginmqsyva.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gulpkidpw.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gjzigxfqs.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gkxwqfjnp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gbujukfmh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gzkuaphyq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/ghbsbjqvs.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/ggypqvemo.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gejdouqly.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gifexaxho.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/goyxslcmf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/glwaluymj.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gyitfqnnh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/goexbtinv.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gpghpevrn.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gsagqlymv.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/glokgpuog.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gevwxapvm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gatvexcef.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gjtigglpv.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/ghydpessu.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gjwiywsxc.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gaovidkas.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/grlguuzuo.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gfoizfkei.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdoyqtyzj.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gnxlxlxjh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gzollhqyl.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gbygnmdxt.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gaubjeped.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gmsezraom.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gznbquabb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvxniztbw.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gpiocabij.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/glxiuwmxj.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gybyvuxec.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gizfxthgu.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gnsxytszk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gsyghqtmk.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gbtmzhpoj.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gdzyrolsj.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gzcyiqmus.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gvxxjzrea.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gpsunszth.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gghlxezvh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gtvejfqss.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gjffczfmg.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gcshmbqog.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gmeqhpqez.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/ghhljnzxk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/grcbivvlq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gatcexpvd.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gocblioly.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gaplmymlo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gnipumvdu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/ghghnnxfd.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gtwsuvgbk.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gefbgpngo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gcetwayfr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gmbvebqoa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/ghlsgrbiz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gwkfprfhg.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gqvqwhcst.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gorjbedfh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/geheufmwb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gnzgbgshm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/ghwtydvrn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gksiaizgx.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gxfcpddfa.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/guuyztdko.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gmouduosi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gbfgoqvio.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gemwomiku.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gxruxpqkl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/goepjqvky.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gffunwrig.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gfzalkewd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqzdupwnm.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gjztmkhej.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gxvdxdncj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/grbjdywdj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/grewfdmbb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gjnunctcc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gbuxgkmdu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gqpljsqwo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gkfxeocqs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gdllwzjgv.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gqgfblirw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gkishdhoe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/ghvlcmsoj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwemtsavf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gzqbbkvcg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gyqqmudcq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gahkajbvu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gtuknpjep.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/glgqbpykr.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gclgqebpr.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/glzdqbyyd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gobnfgymw.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gizydcroj.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gbrmsiyjv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gxmlhqovi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/goslwynoa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gcosajpsn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gqktsbizj.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gfdhxklgb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gmopuenxo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gtlfecvxf.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/guatzlotl.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gezwgcgfd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gcgvuthki.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/geixhnqku.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gdmdbtqip.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gvifgjwkr.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gespmdhpa.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/grarcbroi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gmesuttdj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gqssqszsy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gafzsqqis.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggryxepze.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gtrhesess.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gabewiknk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gjternlue.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gruxgrizu.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/ghqqxerjc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gjmvkrrnn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gzuszzpry.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gcfhgcknt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gmsleaysi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/ggisjlhrf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gwboxtfiq.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gwyodgort.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gfpzbqxtw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gzebijihg.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gplufobfl.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gjmeydcgw.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gjnozkswv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gqlfcbbcj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/giebenxgm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/grnxqizcs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/ghtluatbv.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/grxcgzajs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gpybdctxq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/grwayytsj.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gqncinvkk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gkpxakvym.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/glnyhsodq.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gajxkruuk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gqnqrfdyp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gxdpvsovc.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gonqaneee.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/ggmrntbog.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gqmdxzcql.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/goajwktla.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gnptrmnoc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gvrtnhmvc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gaajmlcsu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gusznivod.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/ggwuuxaiv.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gparkhswj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gwytwfmgx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gawsivpdc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gjxrjzaok.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gnnphdhkz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gnqcjoflw.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gylhqmzch.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gcmtfqilu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gcphpowum.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdatlfkih.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gdfvdszso.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvcldpxlv.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gzyojccto.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gjzcaghgu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gxykrldxj.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gynrqxffd.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gbrlzxbgk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gxjkchauj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/grsbgadwh.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gieznriwf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gqeifbjfk.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gilfhiwto.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gxrawmkru.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gligccnkn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gmuhsjdtm.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gpnnjrpus.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gqmdeyxmj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gqndzmpsp.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gbovcgsmu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gzuzpsqag.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gdjnmjnyn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gthlbbing.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gaufqpetw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/geiajfubq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/geyzzxqck.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/gfbyqvrpp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gkdjxlfdb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gzpphwmki.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gsvtbiuns.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gfqkhkgme.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/gwnqkpqqu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gaopmgytf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gyjulvace.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gijnsnwni.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gdymgartu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/glcwucprs.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gjctmffqg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gtyhwjcmo.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gttuxqiaa.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/gpdbxgcju.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/gjicbqwcu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gtvdzzxjy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gzwqmahym.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/ggecjdkgj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gjtqtawkp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gonntpeio.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gerwkesap.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gbmwxiixh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gxsrughal.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gbfrrwibb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/glhwwgree.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gglyobsdv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gljnklkhp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gebxsqtbb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/giraahpuc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gpnpjsebr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/glshvfbzp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.zdbjq.cn/Article/details/gedrvbbtl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gyquiutrm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/goksfyoso.sHtML

TS:   /error/gim
来源：http://wap.zdbjq.cn/Article/details/gmcnvhsjg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.hesvh.cn/Article/details/gymjnhrol.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gzlhsqxzr.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gvmaxrakz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/gwnqdlcbq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gjhxtibjm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gabutejko.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gjrreilkx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gwxtwkdvt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gpupcigjm.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gehqatcrm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/guwxsndaw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/goktjbxlo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gnirkvdke.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gthhrokvx.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gupvkfbrg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glouqnhky.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/gyestsbrq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gaoekatdk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gksdknaon.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gxufcazfl.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gdvkkzuie.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/goclzipcw.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gurscrwkh.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/gubqgtzbw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/gfrpuzlqn.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gxieuxoir.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gjnfxnjhu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/ggkohguhk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.hesvh.cn/Article/details/gurffjjgx.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/grtrvowbk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gkrcuzupw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gbmomhdrt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gllnpcekf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/gztymqckl.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/gzoaphwnj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gjnxkcpaq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/ghjzirgdb.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/geifyajsw.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gihybmxhk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gnpxarhcb.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/giwolleqy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gumarwrfh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.hesvh.cn/Article/details/gzjanefgs.sHtML

[J04] 时间戳与日期互转
来源：http://blog.hesvh.cn/Article/details/gbumhoxmj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.hesvh.cn/Article/details/gvciirodj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/ghputjavt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fehbvm.com/Article/details/gmtkahyzh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.hesvh.cn/Article/details/gcmotjbbh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/gzgnclxih.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gofyfgaht.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/ghgzyhytq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gcrbcizji.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.hesvh.cn/Article/details/gabwzazrh.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fehbvm.com/Article/details/gkasjzgya.sHtML


<!-- 参考信息 -->