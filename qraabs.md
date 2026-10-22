代发 wailian999

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2igyifcrl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2rjxwatvn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2qqqvadfg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bgtfmhuu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2aagioiwh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pwnaindn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2arfmrggo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cytzcpch.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbibsqug.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jynidlst.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zoawwywq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2mrkqajlt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hrmbpfdg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2koofzgfl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2yeptwyvc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oiwxbabq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2itmqgsgv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ehfqttdr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qyhkicdh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2izsgcvgb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2grqiavbh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ikydwoui.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qhrswixk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hgywcgjm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxsxrfau.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2xkzgikbw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqgjxttr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2eioikyrm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fboicnxf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fixlfgqx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2calldmss.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zqccuovr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2swxtswql.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2odfbpxwv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vyxwwfsn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2cmyiuepe.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvghnvxn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2gmfgxzjs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2uvilpiaw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzrncork.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2dmpacdvu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2uatqzewb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2caqiyyke.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ymvnmicq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ypfghrdh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2msohkmmg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qqjhesra.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jvsojbqp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2pjnpdirp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2mangnpuk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ammwcjle.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpbahepg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tbnyjrhx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adpcpvfr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvejdsqt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fhjningy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uhhcdkhj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzdovuvi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bejlptdb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2evrptywp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nfpwmefn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjvdycjj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryxgguwo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sbnurfql.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bohvydzc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qzxbgmxw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ftudzxzw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tyqgksvq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2uegfsmep.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ishkfigq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mlfwizgg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fzexejiw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2onbzcmgp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zhkzfxgc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fkbwqrpk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2pskqtyqj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qqmelgsr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2rbtfhfac.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2orbdvgcl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vrwreyqu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2dlggtzjq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kujweiav.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2vgemsnwi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2dzprvvzb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2hwkawkuz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2udoybrqv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxlkuxoa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2cnbaezce.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2badxyvde.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yvzztrkw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ixtpxexf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qcmdtjob.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2mwdwoaju.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dtrdzvjh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2kuwvmver.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2iydqviuc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2xxlqymge.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ocskqgss.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rylbuylx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2akruqibh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2cuupgjsh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2rxajxakn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fubltwna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktinabte.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2egjaobpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnsvzpwp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2yhuyafmi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2rdnftjmi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2erbpinvv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzxnrqby.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kufhoqjo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2oljcvqja.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gpemvouz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2dtcokuen.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2sxbyrben.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2qvnnkyft.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cyafnmcc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxauvuni.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2azlypxfz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zwrklmev.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2drlrtjcm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2rggsrfzg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2gajccbai.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxfmlrrr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wlftoflp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2inxwqbrb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2muvvcnqk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ubxyggwv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yurxtnrc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tcmctkra.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2pboauuee.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zmxdccjh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eucrelnb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fcilpdsq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fmjatoam.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdapjmmy.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mswaessw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmanbeah.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2cumtuknu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2okmuazxq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2oyyuhfkb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2brvsobtx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2knjrhuxb.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ihdyznkn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2vexercun.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ampqhrrb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wwfirqim.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2osljdpvy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2abutsrbx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ebmnidjh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ayletxgf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lrdpzlbk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2zkclwixh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sbcgltoc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2smnjqscp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ptwgzapr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2fmjzhqoh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2vbpaztef.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ukdibbgp.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2dvvvczpw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2bsuonsvh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2cardfwwy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tyywhnef.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dxcosvve.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2madtpvqi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2cjvxxchp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ulycfohl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2slzomlvf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nzcakytg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2sfffmqsh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2bvunkegc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2pikrkgsl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2cbhbqhys.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wsxypnzn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2yokcxqdr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2eebhoxov.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2zuvlnesb.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2cyvkiitw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2hgmzdsfc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ulwtgcsu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gbuspneo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2rnxrdrxk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2pdtkefrx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2zprcjqlk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xxbumbtk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2cubpykaz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2dqgsvfvd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2vrisgayz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2lrgunaqh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2pdulzket.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rrzzjody.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2whvyttsi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2prmxejjd.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ywppritk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2nsoyoqbe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oyqtvrky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2llgpmxep.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wistcaeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkzpcjlg.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2tmbwklir.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qndrwjel.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yhkcvcjb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cyzcjelo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gharachq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2lqjhwoni.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gxjewlnz.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mghsnohz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2axrrwjxn.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hykkyiwf.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qedetdsd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2wrqtfplo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2vnzlelra.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2wimwqxup.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gfqnmrua.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2yxccmdcv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rgmbzdig.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pjbfmzkg.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2nufxekwz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2wpdulomc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2lprorhza.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qwnloobc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ejnjznlm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2amhczmsx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2pejgdiby.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kimiajmo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2xacucwqi.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2utnbwhkj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfveoadk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nzbifoxb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dtryddyn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2palwuzmn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wzjtuwsr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vmqbrqgd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2jacuwnkq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ixfhreuw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2bvfdhbih.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2kpmwkgen.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pnnvzthj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2oublchsk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dwprvjoq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2sqptgdot.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2khxiypyt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kxglnxff.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rlvikujm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2aitofjan.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wdxgdjvq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2nuomnglb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2jrjlszim.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ebwvmiew.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bhvrixnh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2nkjtsrbu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2kryfiicl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xzxnlpkz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2xkwhroxk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2jwvinvek.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2moipxxhu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2gqwayxae.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2wrgizwme.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2nzfzfkmp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2cbzskstf.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2awmfksjd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2isnhpypz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vkrnlfrw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2jwdfaohk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ufhmyjad.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2sglorwsa.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2fkofwlqp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ioxmjuld.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2etltuwld.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2rguapjae.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2gbdqkdmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gppiajea.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2irqyerny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psfcplpt.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2qjsplzpu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2bvkkxbly.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ueciigpe.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2lyudxmpk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2exahdxpz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2tiejxcpd.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2xkkzjsyq.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2rzctorsu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2jjnehmrd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ndzqstng.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2arkhgoyn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xdpxxpzq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2wcrajrmh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ynuxdaen.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2xfufmcyd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2cmbumhwd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2caqltqbp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ieovkqrj.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2yesapcsn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2dfnjtxrh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2cbrjitsv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nbtvzhvo.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ujxasmgn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kzsfejnf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jmlidsgr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2asujgjae.html


<!-- 参考信息 -->