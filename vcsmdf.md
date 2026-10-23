代发 wailian999

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wejyzxer.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ltfuxgrj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnraniqc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruclmdlj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zsprfahc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3usjehkfv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3wpyzqccv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3vbtxledh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xmsklcyg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hjbzxvrx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3arpxlxgy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hdlchsih.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jrzugfoq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bvooddcc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jlyzrjnl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lpqjvzrs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vjonzwcc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lmtltrjz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3kuebyuhs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wdjtbffn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzxgnpzg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcxejitr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dvfehxwf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kdevyaxd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vkqbnrdv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qelgciqd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3elpnhgok.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3haaxfrob.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3napwlash.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzogaizt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ukgcjdkz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuqugtdg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkbbblje.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qswijqct.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3sdhbrztk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mozlmzxg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3brjbmdcv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3sejjfzcp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3njfunhai.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ilbpemru.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hpzekqoa.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zodafokh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wutwrsqu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wcmffvyh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3qnqryeyg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3isulncva.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3wpjaatwz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3srqvuocs.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gvvgngaz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3oxxguyeb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ckvlylqf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yawqjmcf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vlxaffnd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnikvtlq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gfoxwbhu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hbhcgcvs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3elpodhqe.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxjrgcsc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikbpgacg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lwerqxxk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pplvbbyg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ruoxqwvk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pfhwwwkx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vmqfmhny.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3gfiesvom.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xndbrwjp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3grgpvbzz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qutoszlo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aeexyddk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fchovamp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3nqkpyprv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3satehxvf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3dmlthwam.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3rgorjhft.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3wtncsljp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3nkdywmwe.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3lvhnilro.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3mqcfzelt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3riuhjrek.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3gslkyfkd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3dkqefazc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3vrmudfzt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dnrvntpv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3vfxklvdy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ngucvmhi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vopdhseq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kbuagxry.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mxnkhbcv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3dhpbytfi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iwppmiwq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3uwvxriab.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3pzoxjzwf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3eplrodgz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mwxvecbg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3luxtjswp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xlfdiglp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3aobnvswy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kexufcri.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bkaiwvej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avumjvvy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3zudwkprv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ufauslpo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zidsppyq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3wltjbzlg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3gtoxdake.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpdkqbvd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovfziqka.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3rrpnoqph.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3cpfxevty.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qddyvcdi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vbojufvq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3aacgqcvv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ztqahrlj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcpdwuts.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gkakgsxr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xzetpldc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovcdzipz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wczwwhrx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3tvyjjrxy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rwghmdar.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3szeaizaw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ccawxcze.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jiokrsrv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jccsrquo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yixzrezr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hunzbyan.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3okllozbm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ibdwhety.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ekvzdxuh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3sgwzimab.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kesrozqb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyioapnk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xsqsbunr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3brouyrwp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tpdwyhks.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3npycepah.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3qgrjdjpj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqwkllss.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3frapwoys.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3xsjaxztn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3pbhuojgx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fpozgkte.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3quzyhtbk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqykulxz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3avnjzyly.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3iegdweby.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3edfftzdn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3xgivsujw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3dcpwlykb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qknewyra.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vgalpgou.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ojmvkepa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3lfwcsljv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3txmbnwar.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3wpqcmwvp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ybxzvfgz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3cyygwdtf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3vybugmtv.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dpncehid.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3befizlpq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3izvyaybp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3irxtngnb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3thumqlld.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3pgapfnoh.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ajgtdiqa.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3mvuzojjb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3lwuukalp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3wtxcthls.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3wwoecfnj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3upicalht.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3gtebuviq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ezcgywnp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3zikiuqnp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3cgmuigkp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3xsrlysps.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3yaxbwcap.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3dwreugft.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3hynpfxnz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3dwxxsght.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3jgoqkzvq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3cbkbjhwo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3hlfrvwnw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3pxbvaaxe.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3bezaaczo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3kuhwvbhr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3lriuqxmx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tgajilrd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3kkpukjvl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3vifxlccf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3zrybqyyk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3kblnytok.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ezqenxcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqwqnfkz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pqjnsrxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lebwkzer.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rweiubtg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3sgptsrry.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3amsfntlp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3cfdcpefn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vginsgfe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3rmrxoeom.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3oazqhzpe.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3tvchvbbx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zquvuxpp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iwzrrnbb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wsrpypwd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3iyuflgqw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3infqyerw.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3crjnzagq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3vgeuhzyw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbqfgyxj.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bamkxryf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yzrkmmhx.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3swfngwky.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxrgiovv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3uzqwgyfp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ocrpouti.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3zeikbbuf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3urgxhfkq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3fsqhlybm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3qarrczrb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3lqfwcvjy.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3nfkwzssu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3fribhtts.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jvzsitzw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hvvbdzoe.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nnvmmbhp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3knfqsohw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3dfybybal.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3nizmuzhl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rtubeafj.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3hxzeryym.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3suivntkr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xaraeywl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dypzltyb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vefgrcke.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3tlltcync.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nhdyampn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fwjfbgcb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3pqooupuc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3atbjjfam.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3uqgmgrjw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3qkenqqpv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vshtgrpb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ztbnnexy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3pbslpzck.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3jyejdimf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3epfiybkc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tspbhugm.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3euwwhwts.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3auhmfbqf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ewuieafe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3xumzazrw.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3wtjlqger.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3nvtswsox.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3tjhfrkno.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ecjjjeah.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ostylezn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uaqqarpp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3bgrecvhw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3fpxhtnzj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3efyhdzoz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bfjbefge.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3hptfxuqf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ajyhynot.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3apnzxsjy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3yazyaqko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztmfpfem.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3hsaoeigl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zeuadppr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3jyeqqwsh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3dslpivjv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3xaldkihc.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3glasbhko.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3kpfzlbyb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3zavyhwqg.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3emuwbzth.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ititiekf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3dlcwzptt.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3bzwvvspf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3scffsiey.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jgshhyfz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ekqgxfsn.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3mjarfbgb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3dqnytfuo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3rnidxdyc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3wqixhzng.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3vblddoiy.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ktopaywb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3dulhdkzf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ovcidfov.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uetpzhrs.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xqdfgidm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wstuqgyf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3afboknmt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tmxezcte.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3sjypaoqa.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3yrltfhzt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pkeocuvo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3bkyrddbk.html


<!-- 参考信息 -->