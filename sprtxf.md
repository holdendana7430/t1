代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cpamstta.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jiplsvtc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pvzoraqn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gehmrcty.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3soolbudn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sphnodft.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwpmrkji.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3egpurmii.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3saufqwjl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3bmomuvil.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3gqfxcugv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3fuptdbdq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3lrcetcaw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jdozqibw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bhnhrumq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cygoywuc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3migeeino.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjfztlpa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3sfwcuszp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ccsqlkrg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3oglrgdga.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3bhfbxgqq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3mlqfztji.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lcnjbxom.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jxodidxk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lhihnadv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fomfmhqc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3krvwwxok.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xbmuxdzs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3sxswctmi.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xnlnmbvq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3pxjsksio.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ytreloxk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3yxtjfcis.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qeadckeo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofestuuj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3mwqxdfid.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3pyipjvut.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtoguhgd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ukapnlpd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vuqxeiso.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kxvbssni.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ipuxynaa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvpuxfhz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rybvhmeh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rdqzvzls.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3dthkfdry.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ttqqetjc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3yllkfjiq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hmcsebxu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xmgiigrj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mnbxrqme.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lyzvplnh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yzdkgjbe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3uiuhwpkr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mogeejce.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3wisuuwae.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3kbzdjvnz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3wevtixjq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyouvwsn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uqscreip.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3saimlrxq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3daqmjabo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3arnxnquk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3cbyznfwv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3tcluciwl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3csehwnve.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nnqpbxfo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jsqcvapo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rvwzsilg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cwmxvfgw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gfovbgfp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tqfyshzq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3avwyuoyz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qzwayzbk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3veszchvl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3bdxqifad.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gehfvhdr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3slugeffj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gfjqxukh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tevcoegy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3psrxjlrg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xeyhfdow.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3htiwlbnq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qgxbgmvu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3pcjwrbok.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3sybjythg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3fslxubiu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ltjlodir.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ltokwalk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3jfbkbcsl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3oyiyaisz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3zokmkwcv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sdrdtbnf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bfvsmmfi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3tlgdafpf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ohoptsfz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3sjgtxsdn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3lcxpdfwo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3foptgvrg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bslrbfyi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mmxxernb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3dhwbbkdl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ifrsrapg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3nwwanksx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3taobukxo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wmetarqy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dyilizkt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zkeuxbxu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3isycvexe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mltbuyem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnatpntx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kqcfepnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fckexnuc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3umkkqcen.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3npocmsfw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3dmxxgban.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kvpysgwx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hxuomiai.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gmtibaer.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3euwxttik.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bvqysogp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ntgnrzob.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3hjgjuyyg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3qldgwrxu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iidjtcgk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljjtncfq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nofajfmq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qjsmglxb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3sbmznruy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ukitebfu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cllnbnyo.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lejfmaeg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3veavpueq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hwfbhmnl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3burnqzhe.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wokivanq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3chqwkkiw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qepnkhkq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3hyrcgdpk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nboacsuh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3falbkiyl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3henybvlr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsyaraxz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxmgocpz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3sifddcir.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3uiuvnjgz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ovdatpeo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3apwgbgue.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3sxwnhyhd.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3byphiiml.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kxvbznek.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3drgpcpgb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzfwljca.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eebeqeyj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3sxsvdwaa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3xlwtfdnq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3prcglrgu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3cskmrbil.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3qrqieklp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ssqkneiw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3valdakya.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nihxzpza.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hwuaqhkp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qtatmfot.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3gaawygwr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3uuslqnqn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zzdkmwfr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3qwckqwtr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3izexkxlr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3khdyjlwq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iymvnjxa.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3emitwrre.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3qmqpuctj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3lrnxldkl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pdcsziki.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fnpgesok.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3jbqolseq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3cjhutvbn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3vcijmozc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3uusaibnd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3aqnxvown.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ttjtfjra.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3cakaxtpr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3dizfespb.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3htkozpfc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3wbpgqqth.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3fgegkabe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3wovphhci.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3xswzuxst.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3lcnnagbt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3kcarxupa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3daurjeix.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3hymufhsl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3svkdzcqx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3rrwdmvyx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3pnqugxcc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3yizbxowy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ugqjmszt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mjvdrlpd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3blbnvevh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3uoawsgam.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3zklqtcub.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rjllfypd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkarekjm.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3wfhlzoiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywbomyli.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fhhzlacb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3acyyhjdg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gsqwwzdn.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kkzqhius.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgzyisen.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3fgpjsymt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3suwysprr.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yhwrhelg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gudlcmlb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dfsbjzbi.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ippjirhr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3nhrmatnv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3fxluuirc.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3egzpmzxt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3wlwawkcw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqrbchww.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3cbfekbfe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vgvlwvsy.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3otnhjade.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ofnzugiy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ysakkrur.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3trjqjyfr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3opztrjpa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hlexfbzh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3hakoudrh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3hyhgdiya.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3meuuhiyt.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3pcawvuhp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sngyewnz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wuhqcuet.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jyyqdmks.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wvtcbhar.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3gknilghr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3aonbjpsp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xwgkybja.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3rmhalvzr.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xkcqtzck.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3sezedixn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3oqzisqjl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zndxppfe.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nxzzujhl.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3txuxoylm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ewgbsdrn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3avvqzpqr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3yxfihcci.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3lrbbvhym.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3easooayo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3zdntpkiu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3froqymee.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3hzxfszdi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rwadyqfz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ayklvzzh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3umyxfjog.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ztdkykhb.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3vsdbghdx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3yzqjtlgn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3zwtliqcu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3vnntzvxx.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3eynlleoh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3iqatmpqb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3nkqdeism.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3gtxdxycx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3sofjgobh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3egzxypoi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3dzqsjgub.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3mxsjjcyo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3oaaozovz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ruionvik.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qsqbgwjo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3yefqsduk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3bberdwzj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3blhleuor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tfwqzvzs.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3jihpyjcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqecbueh.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3vrmkrfqi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3skcqniao.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3bvllvaft.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mxkqikyf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gcvmcmzd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3mmazffgv.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3kymibllz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3gfagygdv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3uutzcpec.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3apxysphc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3abcibhpj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3kowikvbq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3hqzgbsfk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3mttzxaji.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3xwkblsau.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3dkrcajlh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wytdpsjf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3gpdrcdvk.html


<!-- 参考信息 -->