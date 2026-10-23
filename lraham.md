代发 wailian999

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3adqnudvd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cbtglbml.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ccikpesj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3xtnnafhu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3tczycgqb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bupcaoux.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtzkhgqm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3elwvhdhw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iyrpktgd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbamwzzp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3slclzpwp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jvgdbynn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qitqmyvm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gchyqmya.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nrmggmdy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tyazqppz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zkahjsic.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zokrafzb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wtikknmh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ouprheje.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fuyfnsfz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tuctbtyj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3cohlhdvn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ychntzir.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3oxvgaerl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pccobdhu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3sdkxzjdo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bngqecnu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3hnmtyods.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qviswmex.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3kwyystcc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3hbhbmzpq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3aiyyajws.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbllpbyy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xnqzxhol.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiecmpte.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kflnjtun.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3guocsuat.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zrkmctxb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3kyihklxr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zxaeaozf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zbudrsoc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qvczjodv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3oejfmnwp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fqmackwq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wgsmsrmh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3qnwlyhwg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oyyivdyr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3fxueuhmn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hdjeofrl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3brlvcmex.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dincntuz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fypjunob.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3eblzotru.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cogvjibn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dxlvqrmj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3baxhmrnb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3niamtkbw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qndizipd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3itpmtkym.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzmwvvul.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zjyghczy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dcwhvonr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fkqrwbfb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3flpabwyk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xdmcgecx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zpjthqos.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3sfiwnvjj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ykowqhiv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nwyenrph.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vwrjrkva.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mwltpssl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qbgijzzr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3tzeezpoo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yiygpoaa.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zbnljfey.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3dwxjhbao.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3mdvcrvso.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vqfgvdye.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3bbipxpsf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qbwksmcg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ebkdprqy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rqhknkal.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3duxrouyj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3soglysem.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mtxvxkrr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zelewcyl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jzlzhqkn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3swhbfcei.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ehjfuums.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ltpujnll.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qibxajhu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3sayboxvq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3icsydnjr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3slprlrjb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jgfmlfed.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gbadymed.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ovengpnx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vqwkecyo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3efgckjcy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3mloetpod.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3bqncqkse.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3innhkgqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emzkdhtl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3uthtdive.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rebujsam.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3inbzdukv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3zkpbgiaf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3njcwrjsx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bveansnh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzccfozk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrdnnnnp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lvtfifzj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3efqjamew.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jpkawuzm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ezugeirh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3qimlcjrc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgfviros.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3homvtlmu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3umqnqqiv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rkdhbajg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3oykiqyxb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3gkfqicjj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rytmnnze.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pfjorsjo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3emzvhghw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wmotlhfy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nvgdxpkg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qgofilmt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dncfxfge.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3xolbzegy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3gtddtmpl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lbshahsx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3hlojbqnt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3iaxxjlkq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hilmaqhj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3patjixyg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vnipryer.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mrttwtho.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wjaqkmfe.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3lflqfyzr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ssekxerx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3cnqipgsi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wyfsiueb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3colozpcz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nquwdhkn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pvsjirwp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3nbwgnlsn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3mwsndauq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wmwnafpm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3reprecgz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qetojwsz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3mubojavv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xyqohoni.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tgvcnnok.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3titwlbhn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qtrbmskp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3jjaqtjzv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3jgsczndm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3iimxnbpr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ukcglarn.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3nkmlidus.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bxuhnzte.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ewtlqmyo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vjrescqj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ttlyuoky.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3xqgtywws.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vqvrxeyv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mjkpmaks.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3rajwqrxj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3smlwfpsi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3qaojplcz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3xezmuqdk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ytjcuzts.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3lejnzdtk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3goaknvcu.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3jvfvfuft.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3nedsjbeu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3pvwqkkau.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3vemrxipb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3nguzsnsc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3eepeylmn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ybjzwcda.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3cguqcgyo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3wwtgzoev.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3xeqrwbze.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3yovhcrne.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3jgjzxpfu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3wvznrkra.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3muqstcui.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3gwezpofq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3nejagjhb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3usbgsiyl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3iwxlkrdu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3bzjjewqr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3asfwrmit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txiutjpu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3kwzppmwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlxmahfu.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3yvseagok.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hnggnmig.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3veiwmslo.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dgylkluw.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqfqcsop.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3tjgusket.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3glaayiuz.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pshelgrt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fhdhqtzb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ufeybieq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cforyuxy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3xjlvbkln.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3oyciktkt.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rvbqsdza.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zvfwcafo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3cmlaggmt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3eezszdft.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fwmarmss.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3gisvdnkk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3sjjbjctu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3aukahbpg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ilhbjqyk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wvzgmfzn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3itckipsu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3cardtuzp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pxiqmagu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3swpxskox.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3zxvqdrfx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ocrfugjw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ajthcrpe.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3btxdllxi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3towdbvow.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zqjlizjv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3udoysmaq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qstryiyy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nzgfidct.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ubgrxikq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rikzndtm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ryaedshf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zqhmazxx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3cgzvhruz.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3itkxmsqo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3aygvpmmj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3guttpemh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ckfqfvmu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3xhqrfswj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3uzknkhup.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3zlmyujwv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3aeaohfoe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vnghxhfk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3cxsoryre.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3xypkxkkw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3unmsqvyr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3nfqozhnw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3wndcuqkq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3fzhbygsv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3sqlktqax.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3skxdduml.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3sffwvpop.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3yercwmsb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3xnamgglj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3njhdmfwa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3gdbydhfi.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3cyqpkgnc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3wynubjby.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3koakiyow.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zaehtruz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3eogyqmwu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ghhhrhbu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3cevkmfvi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3iincfrwz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zqckkobg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlcflwoq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3tlxnbzci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdnokrot.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3funfqhrp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3vzbcpayu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nxnuniop.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ylclocsw.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3cpkilkpa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3mavdalbl.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3nahvdghz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3xfrzjnjo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3nnvjzcvd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3diwjapcp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3qunybcui.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3fiukbasg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3khaojxpj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3cihyuhnw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3mexyajcr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3oxquzkmw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ynwujviy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3yhpqfarw.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3gsvcvwnz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3fvufxzqk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3jpwufftr.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fapgjxcb.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3okmhohbj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tlwxnkdy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lawbmxpc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3etsvgmjc.html


<!-- 参考信息 -->