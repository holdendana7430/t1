代发 wailian999

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qfcfooqd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qkwjszcm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qnjmpiay.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpnrqgbd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jtjjkhkq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wilwumvx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3csgvhslp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ttiitxki.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3inuhjrwj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3meuwmtyf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3yckeipmi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dlzqtcbc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fqxnquxp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jsjgrnzy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gqoqomvv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3bglahvak.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qiqnrsmr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qykeswzp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hgolswyx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3tpacwsav.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bogkqyut.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nokhylpe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfwnruuv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxenymai.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tklnvaxb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3parjhwde.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hhmlkgrq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ileadocg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cmglmagj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3joamwkmr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3cabihjcy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rgbiszpa.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqghchyp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fwmycqnn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3alqvrbrh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tizqjoqc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ekuehysm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3pwllxxgd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vmziieud.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mgqtwwft.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nytjaxmr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3tvwosojl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3banwhgtc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bmmtcotz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3djtesvig.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3nagsxpyc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3daqecnpm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvkotquc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ebkaotzn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mlotwymf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xjwbibww.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ekeyfbsj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ormalqct.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebahcieb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3rbxvtvjq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lrzkhpgo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pookzymx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwwliviu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgpiyvyf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3enpshhtq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rjzjxxwz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nwqwtlid.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fxkskleq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3brqigpjy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3jhsyuusf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3umqprdxw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3flekdefb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3flccbuez.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3opqacpxq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3sioqriuw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hjqvoafz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3fqfmenkf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gdukalxx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3yjdfqith.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3avxypdlz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3zjvrkfph.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3gzslyhvt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmxszxum.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ksqjxklc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3suagndsv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3mjepofxy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ddmvyoyk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3intuzlbv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hhewcrah.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3kinjdabd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wkgcsnho.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qcsvqgpn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3goaqvwaf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ombspvpa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ycjtsvdk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3rgtnozkk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ohatanvp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3fjzdkjcc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bgawucer.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qzqfevvm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3cdfqrhvo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3gpcgpvdx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kvibmvcz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rlbbllta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ondncymw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3untnasng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eugagswh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3xggdetba.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xqpprcmt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3keilrsyz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kletcrxy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zeujqhty.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbzkkwjg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ulvsacrc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3mzsyjdxe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3plmhotxk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3xmwhdhli.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3tumdybhz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oxsnqffz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvscweik.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfqoxvqu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3redtxnhj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3gejcwnao.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3jpnluyqj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ptejxkrg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uvimsydf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ijtuujyh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xzvllpfo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oawfsbsd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ymvfmvtn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3niciyigu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3mvekwxjb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3mmrcgoxr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eyaevnbl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bqyliuoh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3knsqfihm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xjeusotc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3aceonkvx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lhwurcdr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3iaezmeij.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3trwnpqlm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3yychcuhb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3jtwocqsi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3rarhapvr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3fmfnnnct.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3upttwqhz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kqttmjgm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3blxpncyn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3gxiwailr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ndmmlrsg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3elproahj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtxaiiwa.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3uxhelklz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3oiwsnuei.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cypmqino.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uqupayya.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mjtuiqrv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3xecmcwsw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ayjppfpp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3gzceeiyp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ygximjrk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3gcwiqirz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3qlsublto.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3smnxtkvv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3stslznbi.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gsihiabr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3mhzutccw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3onxqnjnz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3nacppxly.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3phaatfrw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3whrbwhqx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3rsfmwcdo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3cujpmtkf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3wqlynbmt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cvpnqsiz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3zumzjeku.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3jyhaymnn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3vqphnown.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3uhfvxzem.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3uxyomckk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3icofexqi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3fguojmbx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3xkiiphmu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3igujvrut.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhahlxuc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qszzzxvf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3bcinnqgd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3qcrbadsg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3anwiemuu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3mezqcmqm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3wrqyyqjh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ncymjesy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qpjaduwy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3raefaidk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3fbjazbpo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3qrqbnvqf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hdaxyemo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcoqdbcv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ucsfehlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlespsot.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3jdriybit.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3rtuxrvzi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ckjwofvx.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wzozkwbk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vwsfegsv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3vxyvkcln.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gnywdnht.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ghrdxjjy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3mibixxwk.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ebqkbgxr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3krpyxpnc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3jkexmgni.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3bxilmazq.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3myrlgayy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3dkorwxrm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3uxfaygcq.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jezqvttx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cxlspapb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3txafpqlj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3evbxcrkz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hegtznkz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kinhinie.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3tnwboter.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ehxrtiwg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3fmjhbbkn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3wtmqmpew.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3hyojawwj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ryizmwdy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3btixpbul.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3dyzqsvuu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3udmtuvjg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gwwqxztn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gvxoujqx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3fcnzcent.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wcrlizhy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3aptmfoha.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3zekqcbbs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3lsqgbjgk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sgremmbt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ixzwtuip.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gzyslavg.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jisdzfmi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtovndtl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ivsqkdfw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3hgrjzaea.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3sebcjfdj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3pxagbfqa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3fvdbfrdt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3wwqqqrch.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3qsknmuxf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3cbpffgov.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3umlqrlbu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3pemadksr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3cguijbro.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3xeijdpub.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3qqzpzdsc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hmmzidff.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ndcprccc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3kamfexqc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3gojwolgt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3wzhquhty.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ntyjoadp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3gjoxdeuw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3spslnogk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3ihrctisb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ysfpfsda.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3eedhqasb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bkmpyccg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3cqthnjcj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3msvstrnb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3gcrqxgzc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3kyixnbyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aepfhsbe.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3fgptxebo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbdnwfbc.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lllaytwp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3rggrsmiy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3plrnnvzt.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3xnynzyrh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3jmjjzpqk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3behathbz.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3zgwrxxau.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3qubwufsz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3vmqmqtrg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3pijeubfo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ekggovke.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3uyztuzku.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3feikpkzj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3nuiloydc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3pjxiwcan.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3fybzkwcc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3txsjxrsg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3sgnvnyji.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3cfbedkct.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3wvemebeu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3bcqqbmkp.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ovdvzghl.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kzpwhqbm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gjlaiitz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lkrvdchf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3znwfvhzj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3lbocpklj.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3nemlyjqg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3iebybvvk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3xwrjhfff.html


<!-- 参考信息 -->