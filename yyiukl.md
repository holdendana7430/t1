代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3yszakast.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3amfpjcvs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xipteaxn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jstapwaw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cgcgtkra.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nzdejqub.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sodjwuhg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qqfschpk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vgrjxruu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3spouqufm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3sutgyecy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3okjdxhot.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccovadfu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxazbopd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vmwazbcq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzmppusk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rashvgrc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vsiuiktq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ljsunjil.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jfwkohni.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3htldjkcd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3riqxxcct.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3lmetcldf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3souoawyr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3utezlmxw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3grospyjj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tzhklfxx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cohzstfx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zteaeddq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3nlluqjgp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vhdugszc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3wxfkocdr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3llfdfelj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3fnhkzdrw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3qjermrkh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zpjtcipi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3gvdnmeoq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3brnjjglv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3wkpqwoum.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpmlsdcj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lczeqbjl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yueeyftb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkrbcmgf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uxasajqt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3pkqfajad.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybymwmgz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vrakllcv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qviqblkg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hhfizanh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngzwbggc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rikxkljp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3owmkvawf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xefmgpxn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ytujxxpg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bfelxztz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tfupiwgd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3edkvlknm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3btswkkct.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tdksfmkh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sjereijm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vuwgohiv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ngcgoxaa.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3iswcyfkk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3nlgzoxfc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3gnierqsp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3twoobnuc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ygodzlfi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3evrgxlzp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mclkhgql.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3sedtiyzp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3lxeexusm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3pluhocso.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3khoekzhj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3avvfjmyw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bpkylkhu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3yvatggjl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3khkahcpf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lbqjeyck.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hmrbphei.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3fjhuhbkz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3zanzbjcs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sjrgaqqz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3prrqbyon.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lviijpbg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3dtgvfsym.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3mwbfckaa.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nfmdzifi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3wejzupli.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3goxqhkrt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3wkhkzepd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3anhuuzqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdikybgz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3juuxqqvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nepvsoev.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vymtrmvw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3dmjljusq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3cqgxkicv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3odgxgmmg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxhedqrj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbzhvknj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3psyuqumv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3viourpqr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3buzbyhtn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rdzcpmdx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3agvbqavr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ratnlyml.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cfxikymq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3todxceom.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3apgzquvv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3klomfqzs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3cgjcjhda.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hetqlizm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3viftubdo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3yqgjybuc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3afkbxajy.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nwcelpbn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tdbwiikh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dnxfzzae.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vworwqtw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3prprsris.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wwahbxek.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3psxtgsin.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ymfwdjtk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqymncef.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lgxcvexy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uyzwcyzs.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ylhdptzs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3etmhimss.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3nhgmrnri.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3dfflrwmk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3egnwcrgf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hvjobias.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3vycinjza.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fdqedvmb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3sxmcjuwq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3wiusevpx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3wljccbln.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3bglsptyv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3mvpgunql.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3suhzpkzb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3vyurdxko.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lfnupqad.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uehnqrqy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qbwvhtmd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3kfvcxmxf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3dzfjkgut.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3fcrvoitp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iusuxfei.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ugrdaior.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ioadetfi.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mgutrumh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3isaoafzf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fhlnxtwo.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3vyocnahx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3hnydnvof.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3elakhvyc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bvzwrkxv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3wqxwgfai.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3zlgvgufi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ikjgmadr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3vuhwewlu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3xiyhvawh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3qhvbvwnm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3apwsudgw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ofhgpcwe.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jastoyxo.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3adtflzjo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3mpprdmru.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3kfsrcrlj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3oltetvej.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3dbsjxbzh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3liggnxaz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3mevgwbhe.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3hyqccgdf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3lpnyjgtj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3jbiklqfq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3mhdpnzii.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3pocxujyh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lvdwylbg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rtnrijgi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3callylll.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3xjxmzbbh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3qzvrfpig.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qovdogqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdpbwfar.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xuucvgmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqshroct.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3awbadhoa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3bvbgmbkd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qrwlbyue.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ybbnmmvz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jtxdseez.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3oxkqngdq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qgamofsj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bamqqfap.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nzzkecud.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kusdwhyv.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hojlrrua.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3qkscppmt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3raetmuyh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ortzrvoq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gqrtttce.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3iljxkdlj.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kgryjsvl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zsljwhyn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3lrwafuvp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zciclfwf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3uykhlcsy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jzjlkiqm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3benovpsg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3fjvdbzdt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3nsmtjzwf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3jyxqjvvi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3scgtibnv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3syuwscxq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ztnzqmpa.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wvqgcxkp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fpnsvevr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3aiuuvxbj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3igzzbdso.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mjpdqwur.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3vsynpteg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3zhfpxlns.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3qttexeli.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pdycpjyz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tmpnihsq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3pksrfidr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wagatzdq.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3oqrykatb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ptjxrlje.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dsfndrbw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3fafomjdk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3bylipdzs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gmmqtmrv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3rjjvanjk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3pecltoih.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3oruiaapn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bfhiptbc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3yrwapgsh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3slftpzjb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hbtojxnp.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3zoesaujn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3aixatsmk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3qugtggew.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3qkwbtxzt.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3zdawayiy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3dooegfyo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3wtzdwqxi.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3qwsrprev.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3sxrmkxdk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wlnhgxvh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3kpcogpyg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3wcogwjsw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3jiupfdfw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mmdcqoed.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3yodqkbvq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3cthsbhwu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3jrhpnzte.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3leeplhdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuvjhtig.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3dfibpzay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dvbevdck.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jisbsicl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3xjgjmjgp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3fiillusn.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ybotvnsu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gakgukvf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gmfaqlkm.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3lgdttwue.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3xhdhkfoq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3fahfinmr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kgurebtx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3vrkgpwsr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3yijwopbm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3grivjtdb.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3jcbweirt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3xrerappg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3eycwgnqs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ulhybxuf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3phnnfzyt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3zlfzmnwa.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3qkzrhzdw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3rirbnmrp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3igfjfiki.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ibwerzew.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ruqhpjde.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kdjkotfn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bnbjhuoz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3jthmvcqm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3sadiidmy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lrybnvlz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3mejrriam.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ucpyhfiq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3hfuamppz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xiwsuoza.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3suucazgn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3fnmotgpn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lctbvpza.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3eoelavtd.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3onfkhpsf.html


<!-- 参考信息 -->