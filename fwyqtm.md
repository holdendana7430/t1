代发 wailian999

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zublrzti.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3teomamke.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nulytxbx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3obsoazdy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3khzbdcac.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3axymymtf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3yosizazl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ixvovzkr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3iehaggpy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3mknsrsdc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3sfbfzkkm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3daiopmwy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3evxobmel.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tzfmtvsa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ipfgpstv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fctclanr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3swtbxwqf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rcktchdf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ezryxgxi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ynvclxvr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3yvvngdtm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3lslcfsgs.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwpbqinz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kxjodzde.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ttftttkq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hdzymmum.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3jutnlidv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ogtqanpu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3krdadnqv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3yudzjxhl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3uxcwnsfu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hvmejddv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ghhsbpgh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gqlmoglz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ieyagjnf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3lomckmuf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3eyhactuh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3szwzaiql.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ezoazmbq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ixgppsmf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xkgfxtbe.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hsghsyff.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3lpzydohy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lrmacyqn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3gncjxgzn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3duvjkkoy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rgtnvmha.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fdmmjqjb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytukjffo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rnqlyztr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jyagvmfw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nuxztnwq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gmboggbu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3oilfdqiv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3tzejysoj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ebuxzuiu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3owccpdbp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qrjuetnv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oayolklz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3txbofksn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zectniiw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yucwroxd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bddrmoft.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qtpomzkk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hkqsywjs.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eqazfeui.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3juuqikzd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eqrrkyxk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bfhjfuvq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vbzaefak.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3gozohlkp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3bvjqoxkk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3qxjcwnru.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3nriezuxt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3vpfctnkb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3pscyrjyu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3pjmpvhma.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3euptkvst.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3eifqrugw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3dktgzsjw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ipnblnyy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nobaqgwq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jccgnzks.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3dkyunpce.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3vddajwkj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ulwiqotr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3tyzwzses.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xtyyfkiy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3pecvmxnb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pnbarmpm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3hrxrcmuj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3dwcijavd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3jyfzemem.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3phtvwtku.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cnnhlhei.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3lflprwlq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ltikhyzj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dodnwpsl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nbshexsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgfnhend.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nieiijxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlxzcubs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3owfcawvh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3iapzqjuh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3honjkqyq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ogsfsnps.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdpgdora.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3nulzsdpf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3cxxbobjv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lanzlpxj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fdyexwwk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ommjnkkv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3vvvbdoeh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3spstsxed.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3konyyvio.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgzqcqbk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnfaywgh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3cetpniyb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3reotlkbo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsorcvqk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kvknewiy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ltqhuvyg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gatvrasx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3titcklcw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3shzcnsbj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qsvuxaak.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ypajvdbt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3lspxkrku.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dsppvgrh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3nqayezqt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ggxdidzv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zajbdoez.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fknzxnxj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qpkeltvb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dzzyrarz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3xnpkzbkz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zygzeyoe.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3dyidoeuo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jcxlevwo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3byojkxzu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3qqmqrdlc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yteshzfv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfccazfl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjjiylaw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3utbiinij.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3svbwwpen.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvqtyrrs.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3aulwledm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3dbgnlnnu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3tdsxrxyn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ygmlmxgh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uthgixle.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3vkmfhvrh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3uvnrhdhh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3srgqtibz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ildqkqah.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3gouswfzm.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ndiiuwzo.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zgkjabug.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3izzrxwpm.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oielphjr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3gvqouiyq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3vzcwxrsw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vgsidupy.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3axkxkkjh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lengfkla.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3atmmlxol.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ehimmghl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ksvbtufn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3spxjyahu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3qawcrvko.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3lilgsleh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3egqbsilk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3gypoaazu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3miteyoud.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3gmwvjssz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tkoazmoy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3kfvqcnnz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3xblzhltm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkyigkge.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ggcivcyd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3laybcmmk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3prfsoinu.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3csvgkehr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3suxbkhbe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3upamnxvu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3bfxzocgq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zegbiiev.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3busqrwbr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3yvwytvlw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3wmmzelft.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rwbqxqno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnsrtthe.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ifmspwmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqxwyuul.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gidmepir.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vugbxwgl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yuakvixn.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dceldmrz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tndftxza.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3rfvqagrg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3fckxqdrw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tyvzzgma.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3epawkroj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kgyxmwbt.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3tuyhjxtq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vkvgdomb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3babvkfxr.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ssrnvrgq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxkpgngu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xazcsmwx.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3peshldqv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3miccsivz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3gcwgonyt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjlotlic.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3bdumbvkp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3jerzgybg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3zrxffmvx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3bzykbpvv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ulkajxrl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yynzqlgp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3qizdtkkp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3xavawcao.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3spnqahag.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3dxgzbepu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dretjewx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3gklkpowm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3dxlqroqx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xyzbifww.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hamxbfzd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3whijhvda.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qpnagckn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mupqfgxe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ostougeq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xsklexis.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jjxygdaf.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3mikrbdfb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3clhtecwf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nagdwnvy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3xxaynkoe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3rrzafrbz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hfverjyl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ogvowgds.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3evwvleoj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tusekavw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bctnxoja.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3omcuzibr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3emlsigst.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3olrtxixq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3nattvtiq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3hikminay.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3zttpkoxy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3egdlyonc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3itqivckd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3kcyruedm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3oybmhfdi.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3afpkitzc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3zrnjggvn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3rabaturk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3nkcodltf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3zgdkjyrd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pgziczve.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3npgxdirm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jwzdkpzq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3rhmsaetj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ohhgfrqm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3fhfpylne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3miytuhub.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3eoqafhit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3powyxbuk.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gabdpuwz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ngtdxfqq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3vuxgbmzy.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3syzserch.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hwbfheuk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3kmmgsgxf.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3hymxxpqz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3rmhaukkc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3saulceip.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3miztxxqq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3hsapoxnq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3tfxrcplu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3ibtxbgvl.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3bchqpcwp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3njztccqw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3tmqnpjob.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3cdqxgmdm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3kcwlmdsn.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3qkgquwqf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3boupkicv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3tcaqzhge.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xssvuwib.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hvafrlwu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tjsdhasq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qzcpfbyn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tjdeehlz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3hwniymvn.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3bpazfsps.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qzsprxhi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3kuergrlx.html


<!-- 参考信息 -->