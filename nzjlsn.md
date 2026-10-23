代发 wailian999

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nbivsszr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qewwoakk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ddxzygar.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fyiivdsp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ettwuulr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3laumnvko.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3pvnjrjag.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cohdfjje.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3apoirfej.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3iavfqdfv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dnqdifwv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3klmaaaoh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yynzmdlw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xrsjkwox.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cvbmqlaw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3agbbwwhq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jvwoenlk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3abovicqp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3bdnknevm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xmcvxdoo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rishyeyt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tlvqgyxa.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pofxjwvm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bxlezjno.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ohjxsizv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tfrkskio.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fvlopztc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kmbexnhj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rqqcxgin.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hxqrohxs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vszgdvza.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cainefrb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3skobpmia.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gtftwygh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3nbjthoby.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwsqlwdv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3eugmkhrq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3npyeobjp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tdszislf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fluipcqf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lseknbfu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ygmzjsca.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ykylkzhe.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3krirgprz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3shlhnlcu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zmbiopuw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3plituwls.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kuzjquig.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vheyhjtm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uimanfua.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uyqwpyyv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bkwaurdm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3eipcgoel.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3wbnuvimo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3iaiwvksz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3mojkejfx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3osthijmu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhupetxy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ffqgzzmf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bncokloh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3defamlfo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3spzuzklu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3oeoouenu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yyogsyun.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3eowyrkni.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3nlkjwyrf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vtuwgnll.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3vhrjnstu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3dptgqajw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jbenpkzw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3tdaxyxmv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nngattxh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ibsszely.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ratexmph.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3whpzjukn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3myexbpkg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zdagxlfu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3oknfeodm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3crqofdyh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rhnxneyx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3sshfstsr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3nwbavene.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ezhshivx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3svvnkudp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fsdzdvif.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3adzbnwrt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uubmitxh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xvjwzkdp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ubybdkyx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmtcjwoe.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vsfdikdj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gimpnjod.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3sysgmnln.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rncnmjew.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bbwdrfqy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mijuglrn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kljzpgoy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3eskfvtik.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bwjfxqui.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3btbdoyww.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3qlplttuc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lqnpajte.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ibjtobqd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tyfdjhop.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fifnglco.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ngrpujck.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ihqlzswm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fnxscayg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3aerndojs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3docmirjd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ndwttpxd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3msdgfatc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ujivbupz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cswdzxjk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3gefrjoph.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ebfrfjhq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3sycxewou.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3omsrdgnx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3eouzefhd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3avdjhrhv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3hseoitsc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qqmnrkmc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cswurddw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ddwwsive.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3anopovmr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ohvxzscy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3yqhjzyva.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ffixdmqv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3bpokqbnm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3marcxmsy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zvsvekgb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3dekqaywj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3bcojdtbq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3wikbqupu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nsnbwfqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ztniolhn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3snifhzle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqspuapp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3uvwrfrsv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3dcbiqhco.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3eleermdf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3whvrszad.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mfokrpqp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwlokcnn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3aiydtgie.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3myzikfiz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3hnpssiri.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3tizxixsb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dcphminl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3czhytkub.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kvvnlqpg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfuwrysf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zisyqpbe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zjtzbmik.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ygobkugx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tetieknr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3bgevexbz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3nrxwxlub.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tfolpacr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gpyhnroh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rqtzzgzv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fldyfpbe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vrretkpr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ldklmcto.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3omhtrwni.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3nrpxnqgn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bbcjyydb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjqbqmlu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgmrpthg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3isnzcgis.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hqbueata.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3pldmghag.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3uibggkyv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcpekrvo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3leyxqmpp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3fdqnqvaa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3muuujmsd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3usqbwmjj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xocqcccz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iilatstl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3kucauzrc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ltydvhxu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ndfcsklf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3mlwmkipf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3nvlrdouk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xfvhrvzw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fehiolyy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hotzsran.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3diwdxpdc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hqlxuybh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3qrkzgmiv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3grssdszc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ffbcloms.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3rvqjmpdj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tcjbetul.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ytmhanul.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xruxcdux.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3xnpyolgx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3qnvytysm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3dtlcymrj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vcosjbgf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3tpfipqkf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ldvsiuqs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qxpjuixn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3zkpljfkn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vaunkggd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3gzmtyovh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kpzwazhz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3mjivotdr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3gqxfklma.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3wqivgsrm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3oacdaspo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3sboerwzq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3qsemnaex.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3pthmmuto.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxepjiex.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3onhqoojm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3otyobxio.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3uunfgeiz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3owpgbfwi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3lynugqtd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3kktrhvjy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3dxtfidmd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tmugeann.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3kjvwkxos.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3bwevlgsb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3lvbvdrqs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ietoqvnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsxijtsq.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3jrdnhqwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plhvwzmh.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tuhnusgx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehfbcazj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3azhpbrbh.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mpaasyml.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3sqxqrdhg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3gbcblyny.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jfelrtds.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3txukijdr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zimveqeq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3foffzlmx.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3sdhjhzdv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kysjjesa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3nbegtnpb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pvtqwbyc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bojtcgzx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fjnveynv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kufpkium.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3diybkjbb.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3swzdustd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3pmirugwt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3royvmqix.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3taajteus.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3riptlrav.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3utmdcepc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3yrtmlzmp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bjpzcyxb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3widuyfbk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ymnenoim.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqmfncsg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3slviiulc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3sachfyrv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rfogfytj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3xshgarpb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3gkuezuov.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rmsgjsyj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wuyebsdo.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ihfuybjz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gliowaqz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3eaprtjcz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ithelvdx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nevbuviy.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3ysmmjjzv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3keqiimxo.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dvxyfxmv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xxisrlrk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3hvfhwxmt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wxxdnpsf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3tzkucjyu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ocociqts.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vkjyfygk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kxsgmguv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ehjowzxf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3zwcchttm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3nfksqvwq.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3weofgoaz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3vzynnxtm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3refxappb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3hlqozxzr.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3pwipjjhx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3gmaivjpc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3nzctfaun.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3exegguhu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3lnmvyzya.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dutvqyjg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3zrxtyldo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3zlftqtdf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3fvkasyjm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qthhoqtg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3llvfppkq.html


<!-- 参考信息 -->