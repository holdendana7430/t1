代发 wailian999

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwkujyfu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ceaazrsw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2kzggivzm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjotrqtj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gaceskjm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2wpvkmtgi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pdehfjpp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcxhgoiu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ceiueplw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkyieceq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2krqxbula.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fowmchpm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gqrmgwsu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2dlnwsytc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2cbsughqx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mjsdugqv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hrjauqzu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dtvlazlb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2almidojc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lspmbyff.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2lbhhzciu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2pfpctmzl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2aagtombp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mgsvsequ.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pdmjukum.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqqalbyr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnnclwrm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2asnyirjg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wwgyizhc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2odupdcyo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktlkorsw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2beaakgyi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ygeeypby.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2skllfbsx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fyaherio.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ojqkduir.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2cwqaesrh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ejgikvjr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cbfctpdj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2fkiowenx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2zzcttfpj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2drkorbhx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bnnbrrbg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xtezolrf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zvgbcayr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ukqzoqjr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2kcklcjcq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2khfsbjwz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2cqbymmyi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ucsouyhf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ibsxigbe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnstifut.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulxphpup.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmnanvne.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyupzcvo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tckujvch.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ysfxcmse.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucszrsqq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jvovsyzs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2utkioudu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ajopgaac.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pajnkhsm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixmtrtus.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2notppicf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ztgksduk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2comwlfni.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2idyjyccw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ykironad.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hopswagq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hqjgaxph.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2evqcmvdp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aaiepmne.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zjvjfgnw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2jaozguba.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2qfwzzsff.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2olnkdodw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ufoortyt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2sskviifz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ktbaqncq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vdauykgh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2sdnsnydq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zhwpjpco.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gxnvflju.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2wacathox.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2aegvsdml.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2cycnkphf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qivdirju.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2gpjheheg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2asmydatw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ujxcizqr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2azxyxfmd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2vwqfpqzf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2auliakvr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2iypjztjk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2otjixede.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2tcayartc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2wjftfoje.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ordovmmz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dqtkceow.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2wzqvouts.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2eghahdlf.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2kvhtcwuj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hgxxssxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvoqaqsw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2eejanvnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bimvflav.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gdrskjku.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2crzyhunq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2rlavhcsi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmyhwzfz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxkhanfb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlvihmma.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2nqishpty.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2fcqcyqhr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2oghvtlos.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2okhsyvfc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2vyjgtvrn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhsjrqio.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ujrgsnel.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjmqchgn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2czjkzxom.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2nkktqqwb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2iqodxvem.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pjwmmwxz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vmnbocwt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2llshwybq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2amhjgqdg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wuwedpet.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hmlghpxk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vyldyncd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2euezjguf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2zefopyga.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kmrqktcq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2shiukxfc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2evzwvjxj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2iorlzvkw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qbwnnuxf.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2diihxddl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vcummdbd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cqpluhrk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2lqqocrdh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2llxlhjcb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2tvplvcqr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qrpvqydw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2hxhzevnt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bebenynd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aenyzxrz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vubkamof.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2trahnbeb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2prxiowdw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azeugucd.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2umtzmrvt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qywfrrwn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ltddkbir.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2eexoibdo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2dmmhclcw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2cdkcwoik.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2vhovtygr.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2lptmelqz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tufiieto.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ecihjfbv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2utvjoqam.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vjgqedel.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2iowkxeae.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2slahresy.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2pkskgfcc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2jinexjwy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2rlnwzyui.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2marhsrhc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ldnpmpeo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2iclhslgj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2tcefhdjk.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2pgzxjcpt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nakumtrn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2gqdozmos.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2owfxxecy.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2mflsneus.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rtkdalqp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ddkltygo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2poafbxoi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2tzmzvmey.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2bpdtgslr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2sylgelop.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2hibpepns.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2dpjbvylc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2qpaocjzg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2bhsrmalg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2nxfocnty.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ktwigiho.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2boiovugv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bozxfehe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ikeumuhz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2suodigob.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2lvsupfqe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2bghmmpsk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2txytqkbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olklwzvk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sresbabj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqbittts.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mvxykecc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2uqpzkmhg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cenhugcv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xhtxadbc.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2abyonwfo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2xgflbgsj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngpapkkw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xwsywwqn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2dunbqvpv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uupnoidh.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dmcrjnyi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2wzgxzgrf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2czwbhtkb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ecxifntn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ozeclgpq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mbvsqwmg.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2uknnqnyf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ggwhnxtt.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2xdnkyotw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fbrkpseh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2kwqgaoat.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2xtmultpj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2woytekln.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2thrormvm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2wtsysicf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rvjequsf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2svvkxopu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kdziukgz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2jxsbqylm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2metlerhv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bmwxqahk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qraouhha.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hiwadgbz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2rvxsyzdm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ewikxqdf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sbqbqulj.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2cqkglgde.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2cobtukhx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ovuwviqm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vxjxfjie.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2yetyzkyv.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2onazdaab.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwofbowk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2aojbemye.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2igomexkp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2cqrdjrih.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zovhhjsq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2pvnqepfa.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vfgksmjw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2jrcuydpf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dyqpvlkx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2cluvqzxc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2nqrcuotz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pzaqwxxm.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2nqgbglun.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2zffqsbfm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2jnchahuz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2qlenopqw.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2tyctanyy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2isvvkudw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2zptcvuhl.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2kvcksoon.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2gdvlokdp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2mserrbct.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2mrjobxqm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2elmoecau.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2wdbnjftq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2edudqmts.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2agfizaxn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2dajbsshk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2zfnihawy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2chwfjzxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocpsxxib.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2qaxrgeos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hsdhoruf.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fuwtauaj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2inyzwhzy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2kgdnkyvi.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2vuiguagp.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2nmqstjcf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jdfmmhww.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2dxjqcgrk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2ogypayzc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2sucmrvye.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2emqfpwec.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2bkkpgjzp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2htbesubf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2acdtdmxh.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2eyqmjltg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2sqwdwlxo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2clgpdqxz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2cwsnluip.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2zxaleera.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2cfvuwsim.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2rzqvowmg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ymdfqgbj.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zzelyosa.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nfmfyxzh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2spljesix.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2toewxkfy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2imwhzscm.html


<!-- 参考信息 -->