代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zbrqorrt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3smjxnfgl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kldvrczf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3hjieepib.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3eaiunalj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3acmkjund.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajvcggzb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vflfxjxu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivzavueg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3werqjvzp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xvskhgik.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3krakfnlu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zshrlyeu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3frumfkvf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmcjxnom.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zudswsoo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mqjetkus.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pmtnrqlx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3cmeghklr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3cojsgkff.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3pugeulhy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zikifqyh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3aiqmrsgv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3enccjuvd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mwsgqxjk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mlofgact.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kykvnorw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3kkpqreez.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3pshwtrih.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3yrhcnxgr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3csigkeqc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3qvdhggho.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iclnldgw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3siduizqx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3wbgxdjap.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3byawntgj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3gnkohulx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3dfrcauhj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjyyvlpx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pmbxqgdy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3owesothh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3mmgqdrka.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wuzxtnhk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffwojdhf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rglvqurd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3vvyxorlc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rrjrditu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3gedktctj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3piwewuvx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3kybefzfv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rfkpussx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3lnoyyndq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ovhvyssu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3lgwetkii.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fswmmosi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3eidxones.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3uosicwmi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ewkmkeya.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ihworumq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxruanmb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3psfnnobx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3samhlxno.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3crcrvtwh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3etqjdvly.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3tvinoeeh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyttjdsh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kwlpyhdx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3frwwmbdc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yipkxcje.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajcaxssj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bsdahkap.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dgkasaab.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rnkwcvut.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3prpcstfv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3yceithlw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ocgedecg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qpjingnj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3quvlghgq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ivsjnsns.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gymbvdfm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3okmcokvg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fnpkotzy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3giksrawk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3pgwuposk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3zhlbtfjp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3kkjrzjck.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vvdaxikn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ucmngzdq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mvehenol.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3hhxuqdpz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vdsnwxbk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wfwugqrf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3qqfvijqh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3frdexxad.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3taupriah.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3doynbmew.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3lauyikid.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pbvpvhrp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cvhefmev.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3btjqrpmc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3rgyhgvby.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bwovzbak.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3xxqivvwf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mziguokm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vupbkvpo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lkchsihl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3izxegkxh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3hnyhcbgt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3yhfzjwen.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3aextbyjs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kouufedn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bucmvfro.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vvjkjbxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzaijlrd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3bfwubyob.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3xoyzxsrn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3twzoisqs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gewrwzta.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrhprxug.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjuqamda.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3fqmxsbpk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljmuxptt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wfwcevms.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3eqxkkhsv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3rrmbyrhn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcpdffzn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qsocfarh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3twmiksdy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwnwjlwt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3chcfzeyo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3piyrkrtn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqzsshuq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3osvawrry.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3uyrmgunh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hxdhngxq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vehvxebc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jehhhuff.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oemdjotk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3myocniwl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qlhucgwm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3szqjzfrl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bxbeynny.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3knwqoqrg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jmqdwwqm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qskwuqud.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3llbwbell.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqepeeld.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ewacimpu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3agfawbyj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3bxkvkjdb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3jqobcywj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dplfyknd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3foxoxlyz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfazuvmq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bsaltujo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3osqxtntl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qoyveuxy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3kkhttmcy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3soljecmv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3nilvfohu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wvurhfhf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3hsasngdq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nzyairbe.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3stakxuww.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3wggwcgji.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3txpbwnyd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3hrazzztp.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3klxvbanj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ranygget.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3jdnzwlhl.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vkeuknhf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mixbdyqx.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nhkimkda.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ewcunkji.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3cghemdsr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pvpsswax.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3umolopvm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3gqzeamza.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3gppvsxyi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3plgnyafr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3lbdpazyk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3kvwkgkbe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ugbxcenh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3lfvenbpd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3mebldppv.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3zyedffna.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3mlhkcllr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3qlgknrzi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3dkvlvugz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3xekuphtj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3mygkvrdw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3tadcsbtf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3gvzlbqqi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3trkbwdmk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3uiysedtn.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3tenyqgqv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3nmwjuuii.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3bghprpsl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zpkuirij.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3dipebygp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3eqwhrxcc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3qowwpiqp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3zoujikik.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oqsduhkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hneckpfe.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3jnbuxjri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqsyolhy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ntfdpvua.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ukdmpyvx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ynwibvcr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cbeitlqg.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3uosrbmrv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ebtoyuev.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kwdujmjx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ojbhiume.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tbtjydoq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3zvqhotsf.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3mqjczngn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3xdadxehy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ypxtcxcd.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gqxykajw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3udgvagkz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3dadcaxaz.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3frtcouhm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3owgxceav.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3flosqbhy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3fvdreazj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3vsmtvkxx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3gowvvkkz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3bgiwtacn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ubuumefm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3vsztmjfp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qptpsbfg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3umlaipzq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3hnxlrcjv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3srzrtknk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hvtbsmdj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3rsoldzim.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3tgmgupft.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dyjohplx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3eznwvtfb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3sxuytehp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kdtwruvg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3zvczsoky.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhxssigw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bdrcfxce.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jvdcacbn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3gbytdtuq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3tticfiyx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dqbdhbiw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nisppjwm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3sbkqmfdt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3qaxpwjba.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sjshbtlx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3xpmwqpxz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3lfnszllu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3zzlgmiji.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vteoswsi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3zeypxkdu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3gzsmcsfj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qckfrzcf.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ofgcetvr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3ovodxwes.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3svsibmpg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3gegizycq.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3haxywmmt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3lhlmdmbs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3qkoprwhl.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3bphmmrmw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3qfaxqqlp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3efvlnito.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3ynixdnwd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ebywfjiz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3acjqtfcc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3bgrrnalq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3fiijpihf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3khlooxho.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3lolthufn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3krwaheeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqiypbco.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ehlopppj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qiwzdokp.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3wbynhfts.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3fntinaiw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ljefllfq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3osyyfncv.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3pgxhwwli.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3watltgdg.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3xgnxtvam.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3adizujsh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3bfvpitot.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3uexqyokl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3rgbrptqb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3fwjbrnar.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3qtjkkbjg.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3mopjxwdi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3dojoodog.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3izwmeair.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3puqonyxq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3atzwdtnn.html


<!-- 参考信息 -->