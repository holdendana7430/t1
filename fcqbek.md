代发 wailian999

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jjcdegpc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hehyzvga.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhccwsad.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnfwfqao.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iregmsxf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lsqjyvff.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mbkjquzb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwtyhezz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3eqzdbsmk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3lszgcsre.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aozxafpe.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzsyjlex.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3djswdogw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbaoyjal.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3dujuseng.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3owbbhfkb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xyvhppef.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rrzbmrmc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jjtkkfxc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3nwvvmrmx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jfwphcqb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jcedqjvn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tybzbwjt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3elphbccn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3tnazglmx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rqfvayqa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ufkhbxjk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3esllaodt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxylxohs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mwtnyzdq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3jdeeyytg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3diliojqz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3skzhhdkn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3egxslwif.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ehphgqau.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3nsckrmzq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rzaehxxj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcrkmdim.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gqbwrlyr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3uacxdlkw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zaqwoclf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3owraimls.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fbhcbngd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3zzriyfyd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wvergrbk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3odklasok.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ywaoblim.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fdsvwgmj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jpnekjbq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3tcujuvoz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qcgemqpq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vnvbvsih.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3wqqzalhf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gloddcvn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3vqkqylxt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zfwepkwl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3akwommdf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3plzdeorv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nqlureni.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xltenqyb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3juclmlyw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3pkrbttnr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ulddkxfx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3eafwfpez.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlvnrvqz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cgwtftrw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhsagnme.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xracpoql.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qlxdpmfg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rznjonfn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wwzmywtu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lnnqessi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3yplnhaha.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3baslstsg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ikjdlwyz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3itdkxtep.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gioqplfc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3buoxzpvz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wtjamupc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ephwmyqn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ehzzufzl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3nqkesrlb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3eoqrcbwu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xgdofupg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3jzobpmor.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agyaffoq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3avmpqdmf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3poyuygwf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3shwvegqg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3weqejbcv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gltinoju.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooacznut.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3fafbdtoz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ncysdcob.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3xshuztmj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3esiqthpx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3xrngkvnv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mjnhctjd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qslyjxfk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rozewylb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3tldqfreu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vwlgnhxe.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xthlzeyi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3oqkhdgzp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tzrvsfmg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hpvaveff.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bsnywiqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqhnktsl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ghtwkkqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmkutjpq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3pxqdyrzh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bujjpzfk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhgmkvd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ncnrnrxp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ialpnhkh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3aiwmvvqd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3lbjqgfvs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3zgdhgrpo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3uoamsnzw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zqehvugq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vtimgdnj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbwntsrq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpbcpsow.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3llsqtmst.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mgwqycml.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3prbdneph.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3egkewhvy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cqsdruro.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ujemmgim.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3rnbjtciu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xyfofakr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nyedoezw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lekmxgva.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xghplwbd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bkqqmfeb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3tnolpnlv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kzizfynn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ulenfnts.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3maneefee.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dvirbpmh.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3elphqkcn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kqvajwoh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhlfvrtt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hnsggmhn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3lfbjrctm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfqtlptl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3zzhuidts.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3yhpsjmia.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3jddmezom.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kbqupyte.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mkajqxpc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ybfvhzaf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3hbtktxui.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ruxteybj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3veclddin.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3birpwhyu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3arhdhexr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ndznrqub.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3idnbxgck.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3urduvjsn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3acqujdqz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3zifrjvko.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ugwcjcnu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rwhakjlk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3krsbfhti.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3yrghhnec.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ggehjrmh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sffvctqz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3canzoivp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3eumfaivl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3kkqxrafa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3rabeklzq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3alrivlxz.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3gwfiiioj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3kzrgzlnj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3mgstsipe.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3yhypbrxt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3toqckscp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3yavdixlp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3roqembid.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ipvpsfiy.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3apncdlnp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3enohqtxv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3zhvrbpdn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3rxkfbqbb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3eateickp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3tjonkozp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3liliunzq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vyvwufpd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3flxpytix.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ybzetebs.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3jlzufjwk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3eitpkamb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3qmfgldbo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3iokdjqat.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qrslvfgf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3noozbiop.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ypwxmosk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3shbolavm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jyudewgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tucexyph.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lbzsxxrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyoejndw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ginslarp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3niybdlbf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3obhfrjuf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qnhvyuzu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tkbixzgr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3zfxyqbex.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3rytvyneg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yboxpzmm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3livvsqfx.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3zcuyabnz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3asfofoci.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jvfewfpl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3vzuvlcnm.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3jttrvzhr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3gkauvpks.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3pxhaflqr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cgbemhst.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nskztoli.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ybulxrgi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fpefwdbv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wfefbrkd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3xveowflm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3jacludxy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rkxrnyzs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3fdcjqxqb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3wjhqebhr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3wgggycyr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3qjoakddx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cypqeetb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xychquxe.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3macefwfr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lxtufsnl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3euajifeq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ttuodnzt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3amidjdis.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gsmnoddm.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rlwavvvx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gxvdikbz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eumummer.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3cawhwnmd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mfcdkafg.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3crxpxxgh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tjzjcfzd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tlajmtfi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3okfrehbw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3msrsfjxs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3yqlsntdr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ihpbkgqk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3xhbbobgu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3azvitfmf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tdytosys.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3gokqgvht.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3njyfoamw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ououqbgf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3uhjymlle.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3rjiqoluv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3kycmjcqw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3faffbdrc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3jdrvciex.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3lveixuyw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3cpioolae.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3xtgglchf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ulpzameg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3myvfhzdb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3oykahbag.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3vysmaupd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3tzargkdu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ynwegmjp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ldqnkdmm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3zuoghwwh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3rrvhebjo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3xjtbnuvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rvwjxcfs.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3yobdpdjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxbxvspq.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3okflpqts.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3nzgwebdj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3kzarpzys.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3bvnsyzbn.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3nggegzxu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tzmnrkir.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3tcvcozkj.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ravkllys.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3fhgbsewu.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gaiomggc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zjzcryjc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3wiasslbw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ehdieqse.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3vflzzcmu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ibcdbpwn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3vayqjgwt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rmlygfhs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3fuyxobkn.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3lbfipzrm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3xyipgltg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3rxmnyhdw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fqqnkwxq.html


<!-- 参考信息 -->