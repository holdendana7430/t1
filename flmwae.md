代发 wailian999

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xjdprphm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ubvjngoy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2glvkomth.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hpmqoduy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2osedzdpn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nshixfpf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2apgykmgd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2nfurvocy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2somodshe.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2nabiidyh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jjpsveuz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gsvvdqky.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uloltojm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ptzpkoqw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2aqvtsnrn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2okfodxil.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ccnmxxbj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cmyhhrqg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2wgbvwlji.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2oaokdinl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xqsycuwb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2odtkrrzl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2nyxlunpj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnzubyrw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hbfxelua.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mcbjhkcw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhjiwmrq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pbmacykn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qddifnuz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lqcvbfha.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qalfuzih.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmodunhc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nquwomvv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ybjfzlnd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rilqyuyg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qudevfwv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vnupeiif.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nsgbtpfy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lijvzepa.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2faiinuyo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kgehuuzt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vhjysatc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2lhtofzmm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jpfxndho.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2czawhqxb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2kivkakwe.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vptgbdgo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcljuuht.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nvuklfua.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ltbeweym.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ovrhlfzm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pxznvaxv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2buhsfmif.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufyossjh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ocivkgrg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wcicnojk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iklhdkho.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2droyujdi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nookizrb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2upzjvgsu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2scywvyiz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pteddjyb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jykwusaz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vreeuant.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2enbrevqm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jjxfqwfp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ffarroih.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mbnxppyq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tdrgkftj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2xuslhvth.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wdbxabet.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ycxiibeg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2oumiekpq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mckgklco.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2duhapukd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bdsuuljw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tuwctfqf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dilhwdyi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2lgwppqkt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ostqmwtf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2hqmegkve.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2onxfzbth.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kypasfjd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2tkgzbbxj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pyycmovf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2sppwbrpk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2erfzradq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jpzrelyu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2gqnaqbnj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hwpjwlka.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ahwwsxlz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wlmhqkxd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2zfjvmhsa.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nkxrbhfv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xicgxymp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2vkjqfjkc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2issshypw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2nomjvyks.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zynxczwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mapkonfb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2abvvcboj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxlnplqg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tugrnlxz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2rgsllvzp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2oafiikab.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hqpxglrf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2toofehlq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmspjrrf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2tqmxpghy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gbegpbrk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2lhxldhnq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2asetchnu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2oynmlyrh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vqbhpvlj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uswmfhwx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ttiqbxmr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yvtjipsd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wtfxmsoj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ipbypvjs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rwqtczjz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tcficgog.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2pfmeacst.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ixhxrevi.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ketjarie.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bihyergr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gyygrzol.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2aateveru.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hqwsylkq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uttdhuuf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2lkgnfwen.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2roazwoav.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uasyzzuz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ikxoocxq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dixjrbit.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndinoxmn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wnugrggp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2bapyqhcp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjzvkfpx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vjdidagh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2agypkshw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2onxdjvri.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rjzagzzx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkicdgfb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hluidkux.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ycmhfrnj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2boustqsl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqthsbpz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cqgworhl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2clbyrbgr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2knutxvof.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2auvphbdb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kvhfevos.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ozxdpqyc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qsjytabi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2tqrkzdlq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gbppidqo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2akwceupm.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jcwaohsr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wvuztgvp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zndhdgnh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jzttzhjm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2qlnpledj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2pdubbduq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2pooipicn.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zpbsthmq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2wemhszgk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2jmfyfwde.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2euwleell.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xmkipolw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cpxgncgk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2mniuwsct.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2khpgkuqu.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2inbnteml.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2jvtghnxf.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ehncqexd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2hgmvunwh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2jzdlmwwp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2nnehsilz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bpesbdex.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2kafijpds.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2byddquag.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2uwaevgjs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2duipysac.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zruechkq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2jdxswwtp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2qyjyqplj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bukioncb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rydlsxfx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2npmvrfab.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2fyolxjwy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2dhbcyghu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2migarvbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzvjrmof.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2kuwruqlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bafjsrbp.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2esedkijt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlqofkey.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nykhlewd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2npiucfiu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2stswfsxq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2mqwmorbb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbkfhhmp.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2dekqiudv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2moqehqyj.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fpqddzlw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qcyumqwr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qyjaejsw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2nwzkenkh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2iquorioe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rzbujhyl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2myrfddfl.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2thmggigr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kslytazk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ybonikjn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2melqlvah.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2felrsnhu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2dlcdauyc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ayfktkqf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jpigmpmy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2xjkyzmfb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ijfafpdq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2bgqqpypa.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2lpvponcz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvemylug.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hxkphjwk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ejjbyfiv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2atxtiquo.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2oslfiwon.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2oqanjwjx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xrxzzepz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ixdsahju.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hkiirkxz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2pjwojlpu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yrjlgtwb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2enhbrgmm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ccsvqyvd.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2humzqttt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ovjejztx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2sqjxhpvy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2cfvapomc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2wzrchfft.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dsrpldsk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2eolinmcd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2nkhqrdqq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2yfseukxc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cryvgnig.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2jnrrldzd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2dwgxmkqt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pvejvekc.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ridnwnoi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ltfidtsd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2oszbvrfe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2yyqvgyil.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2jghjtjec.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2oimnhcss.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2pdyvqulo.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2bbpyhmrq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2hixkdxjb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rfsfewqj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2wiwfoxez.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2mddhlsgh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2cvrqcrjq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2tiyhjpxv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vrvxyhth.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2sicxvakr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ldvleoof.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2zolrekal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljnthnbn.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2rkczyhrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rdwfxlfq.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2smlsbonz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2xckbbcmw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qkhavyqr.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kwmvanza.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xmkzgtgb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2yktnegak.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2jegqyqye.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2pyiitzay.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2plejkvtf.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kucplpxp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2gpjwjtqr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2tyqfnqzd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2qywjntxz.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2xwpqjvay.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2lxlzlebg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2lithsgww.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2unnlximx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2uypkxtdy.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2kcmzbtcu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2xzfhlmog.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2oolwxpcu.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2djsjjrzr.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bvwgahog.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jaqihpwh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2crfkzjkk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2icoycgrp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2jxiuxnra.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2akxrhhod.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ojwpctwn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2twwpfkpz.html


<!-- 参考信息 -->