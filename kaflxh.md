代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xissjitj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bixfghil.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3pqsolcjh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3okaxklgp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3rmjimkek.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zjryxpgm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3hutlqmly.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kngpjhvo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hznzbyyi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mzxtyyig.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ilcehvox.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qzywsgni.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3yfweylht.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3thwcdrwn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xajobmbj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rvyhgdmv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ewqygobk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtqbfcdr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zayzoukl.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3sbqzbpju.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3bpwcbwuw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3okxcluhs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkokfukk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3capjoiwp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3qenlynuo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3iadesgqn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zpitmjax.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hdvuwjoh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhftlsln.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zjyrstxn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3uwtdjsrj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hurbugxn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3snqpnclg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nosguiit.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3imzyxmpf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3osdieqmj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wjahkutb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3chtbcjpa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3rduriwyd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yctbdoiy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3pikhdwbu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3owughksa.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3twdirclv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fgwtlxkk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhijqwfx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yjulohnv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3txsziidt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wgyxefov.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jcldvgia.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtccxssa.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3sdrorawa.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ngujrshm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qozrbzgn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnqdaljg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhntwhtg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3onzgbzhh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qneapgjg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xebpmykm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gucoazjc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3pmonvyvk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ikthjbsj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3urcoipnf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xcfuresj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xngpskut.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xmendxnh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3cieqakpv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3aenaermk.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wwswifqm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xerzlyby.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3cgdpplwj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3nbskbrlz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xhisibnc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3vecqelyu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vntbfqpn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3esvfzewf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hmkssolb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qqtsxnyi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ssodbmzy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ahabdplf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ngeahiel.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jhjkebfz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dzqtlmda.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3iocugrcf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3sqfqhlvw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nnrvuumm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vfqcnxhf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3luqkerpe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vlbkjycj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ydfpgirq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hwejsrgv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nxewjlmj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ipupprry.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hqsjjgxh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hdngtyyd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rsaqtexj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgmrhqoc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3petlnksy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slvaselw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3eqsctjqd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ebftgdir.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3eiuiepgy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xeemoter.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ggpxyyfh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxfhzxlr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3deybltof.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3fxcsiahr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3walvzskr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3dspluqyo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3rwoavbtk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3stgqypnr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3orbxvlhw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnmbnfej.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3orsheilx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3umblwjhz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ebagfxcr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjuglypu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nufsqlxk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3jfdtndql.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ymgrzbdy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pdqpmeah.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lynhairb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zvporykl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jgoaqbjr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3jimbauga.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fldxylvf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3sltqfrhm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3firnpdch.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rzjlwtsr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3poiwvwvc.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gfonxkqf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xmhapkrj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ofehfyqi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3jxecoemd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3iskzbxki.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rttgbgti.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3jqluelry.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3beszddbk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ruodloro.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wnfmzfjr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyombvev.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3xeecfxca.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3mlurdrve.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3lgtybont.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ojkbwbst.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3inpyfono.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lgxbrkoj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yhssogpw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pplotzxp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ihanelbr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3rsrewzsm.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3vaedlmcc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3vqylpsrj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3zlyunsur.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3nrgackzz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pgjdujee.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kliydkta.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fbhavpao.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3lddxtfgg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3pxvsucwd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pretlode.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3serloigd.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3iobgxitt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3yahleuvk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3pvfixwzt.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3azifgkhk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uqsexmjf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3mandgcfx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3gxtenuxz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3pqveeosn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3qgcbqbaz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3nvmgdgpo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3klrlwxqq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3sqjgdhbe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3wzxjdusq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3slwnegxm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3khpeyvft.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3oaqjgmoa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3mofolmyt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3cwmnrfcx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3mkodjxaq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3lpaqbqni.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3brvxhuwr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3njjjtghj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rbychzaq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3tqzdqeva.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3dgailsqu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ztkzsojq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jgdxqdjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdmajxlz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3xcryvzlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtyufmnj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ddlnryyj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qppykdkm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pdbdzlzd.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3krgqugok.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cgmysteb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3xlwohcsl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3hwqqjuya.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bjniuomq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zdftnzhr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ukqremmt.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3toykktdc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3vfiwshbs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3wqesahob.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ewwmutct.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nmvmovil.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hdmgmipb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3csicwqsw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fybizblf.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3sldkzcam.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3iavvnrzv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3sdwvwvef.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kpqyqiwk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3otokewhg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3kilxuqwq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3rtjwjmfl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3fubvvhci.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3trebtlcs.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ndqdktzc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3oqlqwptp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3dwzfbigq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ekoiheii.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3qarhfjrm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pbfgppoz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3aywszbxy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3aieqedby.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3dffizkgj.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3arauveld.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3ceivzrej.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gfuluhmt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lfvwdpdw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jvauwjak.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3cdqpuzjh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3gwoxxnwx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3vkiekswz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3zpkckfdf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ijvrayot.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3uhumdzav.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3kpixsaey.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3dbkjdhkf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3oskpurlw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ryldsjkd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3tyztcbpc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3gfvozwma.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xghmrkwa.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3avgphqgw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3sanwuxek.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3qombznne.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3nhmeslxz.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3vevzjezy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ibtspfjj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3ekfyqyxr.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3jpzaqasb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3skoylmmf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eiytraon.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3psljsype.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3sbyfwgaz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3dagekjkb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3normwuse.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3liwhdrba.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3exrfzvsf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3aifisuyd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3negkqlvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obstyafn.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3fizppyqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btjtuwzr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3zkudtjpd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3fttskkxi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3bfixkvhn.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fofanblq.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3twakovms.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3mlxoexzm.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3pxpvvohs.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3inwnhwrc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3knykajbf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3vbkruqgw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3peengzyg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3yiddbyan.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ushcyejy.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3bttktylo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3afrgpyhu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3jdfqetxm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3voapcycv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3lessebfz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3mknrbman.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3gufgkqmd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3bldibkeo.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rqcztzfe.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fnsewldr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rfjdfdys.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mghlaiyw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lpkklszx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3iknwveyb.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3heqzfger.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3byugfexx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3uhysjipf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3htnkqhir.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3hkzxaocu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3dvfwgxsq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ugwgtkri.html


<!-- 参考信息 -->