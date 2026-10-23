代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3azfqeczz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwicetbn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3cgqcphrw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ghrrdsas.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3nujuxacw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3hsgudizv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wetlsjwq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3unpvahhv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xwgynxxy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oopxaony.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hvhgnxxb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ttklxqbh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3yhutrjko.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3nqwcqnfr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3phzylydg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3uevtqufq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3avruhiis.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybnqoysv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3aimbmcyv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gigbasth.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3wntycawk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3yzwmusbk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrnmyiwt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3lpvockoo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wmaqvsqa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwonhhfk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3drekikbt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3fpthtljc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtlqcrwv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hwowthkm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3affomwsn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ldlxzdak.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3scjwihyj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3puzhityp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gbrgvytx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xpvdpowh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jekzadqv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hygzkfhj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3wnlxtkrc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zwyfdbrn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3itkiypsc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vwwpcgjn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3sfgzvnyr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ykxyaesd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ervyaubg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaqbwkrs.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3avpnpool.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nkkzzktw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qwokrxhs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3czkuzdig.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rvnnzxlh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uihrbkgv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3swjnyyjm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tevelcht.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3obuagjri.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bjtubxdv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ltkkxosh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3iloqrghk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kwamhvem.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3pbtxlsya.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ppukvwry.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ldjbzvqp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vrdiwpqe.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jatgbjky.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xfycovvl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3cscultca.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ppzftojx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3vlmkcfyy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3geqlnvfd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3swbvkcpu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rytcxzzy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3pbanjkrk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ysdmqbkg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uuwwgwbp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3abonhhqy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3usngexax.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qtdmxjnm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mmgujrdi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ochrpblr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3cxvyerjz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3kgqkgyaj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fngkkqnk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ycfahtlt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jfosusvm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qzbeivpx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pbczojqd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3mfahwtoi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hrmfkytc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3gvwiyvwk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3agsskmcp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ynezvasp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3bgwtfsxq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3dmhdiwqs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3jwgdvlgq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mtjckwyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acteqray.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3rdfdeizs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3isloryjc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wrihwsvr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3cvxhrhxg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3bskgapqw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mtaaqsyn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tetslcwq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ppmlfobq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3uvorcnvy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3kspfeieu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3kxwyzhfl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3uqicjity.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3eismmdga.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kwufglmo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uxxqaubh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3joefszyl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mopfkeje.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3aayfqhfh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3nmsjyrbn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zkmmduip.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lftkgmeb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3amoarams.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vzhkjclg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uvevzksv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mjlvpowh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zfqrkbik.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3oajfhpma.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ddtnyskt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sechnmrm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ttxukdsv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3mvnwnuvf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yfiyouln.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kzuqzbtu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvzcqhxk.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xaccpyqg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ibhgoppd.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3kzclmjvn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3pseumngr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ladauuvk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3zyogsild.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3dvmlamwu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3iobbwbnv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmfxtfmm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phiizpuz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3remvlejf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xtkpmbfc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3kgkloktx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ejocqlhl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ksdbyfaq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3seqbnynt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jyrtgsbu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cijpgtlz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3cygxcvpv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3dgjfucka.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3detzhfke.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3mgdtoxmp.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3caebeszr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3lpmkulrb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qqznrteh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oacdvssn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ftgtewgx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3mlspwcbb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3zooypjma.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pobpgdtf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3utjieiby.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lpipvwcb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3laphgghf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3orzupvkn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3rbequyyf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3rxqkdsjy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ivyyjoob.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3cmpgaeuz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3bvbsuean.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3kcfiqagl.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3btkearde.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3vjtxqjuf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bkndjgss.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3oijpsshz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ygvzrszs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvsdxmsq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3lkktgjie.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3agyzgtua.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ogjwxjuz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3xawgyovq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3xyncwhbs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3jdcygeyt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3kvkbyvxx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pxlpfjpu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3oapnwooe.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3tpsxkhiv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3subntvdx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xstwusxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdfvhonx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ulsmhqzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wplfowja.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wpxpqrkt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wmuuqikf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3acsyocdu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eiipeibz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3saqyxkuv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3gyobtwby.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3toevwknq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vxxloenn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pisddnrn.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3srphjine.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dmdcuxjc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ajxhwfsi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3fyxkhxho.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3xryaixqn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fzgyihop.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3rzxltyvf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nfmhzjfp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pyjtphin.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3riwwgwah.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3oahmblik.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3foyidclp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3btffjeib.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3njmvqmcq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3mzlgtjxf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3rzxdwggk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3achveojl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3olnnmtkk.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3dancbioy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvfncaqt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vknxjunf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uslxyikl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3allyjwfb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vbgrskec.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ybntughu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3vqwnlnjd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3lxxhldeg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3tgpjrkcs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kwgxonic.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gobrhpgc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3bzfeegtm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3msrymcgq.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ygxkheyo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3axsncwjb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3puhklxdr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3oqiwrovq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3tgnuhqox.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wewqreye.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ufxdvcij.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3iqxrsezg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ybwpcfry.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kmxglcjw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3wqhybfqv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3hlksyzur.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3szwtesag.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3nobfssdr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3iuywfhid.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3cxowcbzu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ltcnjrkc.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3xghdncbj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3sekkzaiz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3voptdeft.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3snmowrsg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3abuyyyvl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3roocmhet.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3dodtvbkd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3sdaenlfn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ournjmkc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3keaunhfg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3uhdhpksa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3fqdylemc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3vaxrygij.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3kcmxuhkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oabddqdc.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3jpxtmtsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjtpzmjx.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3pemhuvpw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3jrxedxjq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3vsiljxbt.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3effliyyd.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3bbkuroik.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3wljlsjxg.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3rirvdoto.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3emvjmiye.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3cfoxksby.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bgdzroxh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ogdndoyh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qsgxvebt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ivzgauyn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3axpcqhmn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3udivggfu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3xuprjaab.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3lwyhkuec.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3bgpfhwpi.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3dpznwubz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3yvpamtch.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3txotlmnl.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gkvdvmjb.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tsawceob.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tsfdgocw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qdqsffeq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3csajecjo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3qgkcbeka.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3qbzqcffe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mxrittej.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3dwsutbxz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3mjtuikok.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3kcvqxlqr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xrlzyleh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iokigfxk.html


<!-- 参考信息 -->