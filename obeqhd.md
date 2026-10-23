代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ecksxmof.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3djuzjgcl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3pjnvcvlr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3etqfdvxh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vslzwjjh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ipiaqvsp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rkpmxedw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kejwjaxp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3dobgalty.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3adagpofb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fisfwmoj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3zfaqigpz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlpiappq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3lgzixmst.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dpvmvifk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qawpvhwd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3grxdgmxl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3jemxbyjm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ddyafrcu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ukqtlbfs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3oqjpaykw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ficpyoch.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3veqclzsr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3eazhxyxt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3dbkxvfwc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3jhmyhwvb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3nnsisopu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjsqlhxp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jtflohup.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hassgjoc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cilohtfw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vbbsxusw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xspnasyx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zsioypma.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ooxowjze.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dvrgazkz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rxeqrxjn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rabgbjyl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jlpexqrx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3eivtdrwa.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3afmuhgul.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xcmojlec.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bdevvzgu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3crdqatqi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wcjcqifb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3uayjepjl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dptjaflx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jxggarec.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnywlbdn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3isgmesux.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdahwkxi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdnipqny.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ldriyvli.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3quddfhbr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bgiukjfa.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rizrukyo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xfvkkuqv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3phnsyqql.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3arfnnhti.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3upughvli.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mcuixfrc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zbzbhfln.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3acyxvhfu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3uursmkdg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3wimmajef.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wovtujxb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3aafhdjwc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3infmeilw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xulpwolr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ctmwbajr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3xkenslsp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3bwyoaotw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ghhtgfpk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xvgivnop.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kcmoshus.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3nsesrrll.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3kvrpfbaz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iffqeeui.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vkivclui.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3szdylqyq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rtjbkboh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jgkopeck.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3jhqvlkdt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gunibwmg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zbsmsfiq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aocppzke.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tlweakrq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3byfbjuko.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3uwzupcru.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3uvermthe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mrocxqva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3samxvnfd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3mqryylty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tifrbjug.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3kcdezzkr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3snhinbea.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjtpykft.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uirenttv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bdmugzdm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3thkwvvss.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3plkfjjnd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3etcmvvwi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hovrrjvg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zsuetpil.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3wipoossx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zseosejh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wspqolnf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yscfwndu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3raabottj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3guemcafs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3geqkmxdb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cvyoovhz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lrasimah.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3kuabjnne.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bgimaooq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wcnymnct.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nfxxncfx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hqyjgzmj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qkqnefkd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ciodcptt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3awnjcccq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zvpdhkty.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ixkkiyhe.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqedpqbe.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcpzxboh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3yzmfgxie.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3akoyyjlb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3wsrsaxor.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3mybcqitr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3icwltxov.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3hmofjeis.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3cjxyabbb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3tfhgtkcr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bffuhnkl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iaojxarn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3kgpdwpew.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jjuikqxt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3dizmtthq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qodtplbr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3uunptpxv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3mjzglwlr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mtknurvc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gdwkaexk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jyzqzruw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3yhrfijpa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3csozflsj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3usznllxt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zcnfhgop.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ozmwlwpe.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3oihagkkr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xigeavae.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rakeaksp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bzzrmvbk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3vmqepusd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3iefcxyio.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3bvcxxsyk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dlosrduh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3kkhmtbqn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3euleohrs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3jrcffukk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3syvkikiq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3okzdjhaz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3arpvsnng.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3meusnfnc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ekzspgqo.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xxwsofck.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xqfuqaud.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3igmpefgz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xmjduiqf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3omiskvpe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3vtubiakc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3wmaiplwo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vucrudrc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3wuxrzkij.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3siovaxjz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3luvlwvqd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3qcvtzvhc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3mopiymsx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bbgnmzgn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3gkqdvggq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3lpcroxat.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ibpgkgvz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3vntsihcz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vtktcyui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ktliomnb.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3unehgiev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttygmyft.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ijfnzbcq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nwljjimz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dsxabxgf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3etsypjjm.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mwchtvio.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3xkzxxwwb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vmjjcthl.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3snarqqkv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3fadtlpkk.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3pbekledu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hbdmissi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ppgntghc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3gpmfnrzl.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qtdrudec.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aiuenytq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cckxsaxo.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jamfwhqs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zxxxuhhi.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3dfxwnfik.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nsudvedr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wkbheuzl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jxxhcwze.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qygepoty.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3gswjjagj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3axwdmrdh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3byipaxzv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3xsrnnfoo.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3guoeuwgu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3xeucnlla.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3klwufeof.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mdjkyeta.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pgggwwwb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bpldjjzl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3hjntnxor.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dizirzwc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tohlrqdq.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3rtjbnnmy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xcmxifru.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cwduuxdb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3widgskjf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3hvxrnefl.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3jfugtlkg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3aeggyzaf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xstvlalq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3acbhnqkx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3elreijzk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wpodyzhz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3tyarobtn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3qmwswvmu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3voapiiam.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3urptdrkx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3jjwjobyb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3saejebur.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3sddhdiue.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3kmxpyatj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3kccolqjv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3jthwcafe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3msjmpfll.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3wbwcwpgz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ivsyvund.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3olwrxjeh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ieiuxrxg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3cmwgmowv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3qvrjwwdu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3aukozhsc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ghdbpxea.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3yyfsbwkg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gkucnwjo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3mfeyxtxw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3sfgwnfgv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3fpnkfwko.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zzfairee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjabjgsp.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3uglgqbak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydqdwvzd.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pzydllll.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3bziakzpq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3xkrbevxv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tomkzwuz.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mpqopkom.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3blsnwexp.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ammcivde.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3slrjuudn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3xavdpxdz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gogvtqmu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wpnnerds.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3shzzgqao.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3hwuvhcdr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3cqykjnmu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3zjzrwhkp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3aurojtch.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xnydqeza.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3obvzminx.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3bvwglbnh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ppdknaxa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3bomqpfkh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hmjgskbu.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xjqmskrc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ykatnwop.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3aepxeqge.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3eebdhxvr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3khbzoqvw.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3qcnaszhm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xdghopai.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3zmprmgnh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nlmvupfz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3sendowsg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3abqlfvbd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3wqfmnjwt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3tdciolgz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3pqkzuids.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3gqujngvz.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3hujzpsaf.html


<!-- 参考信息 -->