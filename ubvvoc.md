代发 wailian999

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2yqnzrtbi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2brskotaz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qplazrnh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2dpdgukpg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lugdwwhb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2fxmuoynz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nnoovrcj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpxdthdo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yuntxykg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wbgjefee.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vhkokvxa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eyhsjsps.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2orjdbmpj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pzpzmfyy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2gqiduock.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nayttmet.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzkjmogp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2fhxtongs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2muosuerp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kgttgvfv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gjvnbqsx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2twjsjbro.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tojwpyok.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rjczoahy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zqftlnvj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xbgazsgj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2selbjwnj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rihqqmgo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fttzyatr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2junjkehm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nypcqpkm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zwadxgjb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wdnhqaqz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xwpvkhdr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2emckqqhr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hglkixvv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qnsuffdn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2leahufrb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2swrdsdhj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2othpqnpm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lgcorwaz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2kiedsahu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2flvdleqk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ijwulpyg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xvxqodfv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ivivwtwk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhbiaxww.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sqxuozhq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2opepqylg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkwhhfmu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2luompaza.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2phxmhtsm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2bqctfhuh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2iwfujfkh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2msqrhpoz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2cpqxoewd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ozgnndvk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2weiauagn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2japwppmv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2kexcbjnk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2yuknppbk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gbrhlxsl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2tuaurynt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bquntbkv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qimpmmsj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfnqlmec.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2awfkoloi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2oknesrnz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2meqjdosn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gvbqcaau.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iusrkbvz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2gndxjjlh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2pshpitjy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2kauyifnx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ppvqauho.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jemokgqv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2cscanmkd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2scywoltu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2xianpmmd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdztmzqn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2sdjemnrw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2mnahkgpm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ybmmmkla.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2fisjxjjp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cyghthyp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2usclgrcr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2frqysxwf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fuklseph.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2kmiuyfvn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jkvtrpbx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2vufbcnym.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gebabatg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2udksyqzu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xyybydyi.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdasaxus.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pakosxmx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mfnqhaay.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2lorthngl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vcuvlfxx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vifkjhwr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fntevjul.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2daeaplxn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vpsuxkio.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hxqwaydk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gcmsmylq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ilhrdbrl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2plnjrmpf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2fbfwbxjv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rgedarhd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tjjvvhcp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2huumzmtq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jncmglkf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bchqznbd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2haeqbjbr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lksrywau.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hsreuail.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2exbkxhoz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ldyzcugw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ynngqgqd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2joovgaxy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wogqdnio.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbtlegnq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ugyrsxei.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rdycqsfm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ktwaiggp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2diiyomza.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2pyqizzog.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsedyzqd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mlgtjyfl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jieungxx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qmpishmj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2snkwdyrp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xoscpbro.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vkprpdgz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ekrnytjy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2trtzqfsd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2fgokdzic.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qcuosqnr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vdokvjvv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2strxtnkw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2vwtqixig.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qztxtgfa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cvrlsypv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfpivtaf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nigbqxaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltklhcqp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bcqdzhbd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tjihjfot.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwkvzzrb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukebmlxg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtnsiehu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tybjfcyy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2sgbkmcti.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2jqrpvzxv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2mufpkoya.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2urzxaggo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2oligjgiv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nteababl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mmaixolp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ligdkbbg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejoxgbzq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2kkdnsyzh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2tjhlathn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cxajbctl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lttihwus.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2aibjqvzp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pdkediqi.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gafxxwve.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2woezyrdb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ogpkjklj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nsetnmnh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dypgdkea.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kvjqzvjl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2jwgomuly.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2teupytit.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ietmwdnw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qrulwcdn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vuvposxn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cevyqqnk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2rwxnkwqn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2psgusofw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ougcduuz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2rubaqpmc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ogbkjprx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2loxzlodq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfaxcdff.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kyocnfuh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdykgbdy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ycwwzvlp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2wuyiklre.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2kpeiqzty.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2lossfkis.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2bitzxqix.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fygsvqhs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2duhvbixm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ngolzcpx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ipvrlleg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2xyejksxz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2dtuunwbd.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sgshyrxi.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2pspzcyaw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ofntqznf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ggbqkoes.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vgclsjbd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2byfswsze.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2nlllvahg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2efxcwgxa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2yiizsibr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hafiavfy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2pnjadvsw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2bgywsawa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2fkceqhat.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2oatrsffn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2cijksaix.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2blemjwxt.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2sndyytoz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qmweupva.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2vwjekxjo.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ykiqbxji.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2mlkwqyfj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2mqcfnbld.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2zekapowy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2izepklul.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ebydwitw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2csgqzmys.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2qcxtlvru.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ffeudutz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2dvkbwuaw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2bbravzla.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kuazlyih.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wcxpczpu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2dzsirxyn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2fyumllnx.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2xqbokdja.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2nuujrtra.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dqmoqlff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhbqjtgi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2gacnrhzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tztdoatm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2whuznpqq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2dabqbpin.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gorxrelg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2krflloqk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2pzjwkzbu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2fgcathwn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2pflfmkku.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ifjcceub.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2hzttduav.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2wgpoxxpc.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhrwnslb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2undkzxir.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ssrucmny.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2nyxbqkjm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mgsscsli.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2njmyyvcq.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fmscuwyu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iopmotzv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2gbpkowxj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ivjdtlgr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zksupbkc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bucjhyqc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ieuclqeb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gebibgvv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2wqswcmqp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2pvmeafig.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2epszadnf.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2uimhevfm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2mjihwiev.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2duugilqx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2comnfuke.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2xrqneawp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hvolkjaz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2iryavydv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hxxfwxui.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2tutobpji.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2fvhzivjf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2lvxwetgq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vmawopce.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hvkucief.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2wrmhqymp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2mgzedgrn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2oocabkpd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2krxvlpkl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ypcgacqs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2tlhspgvb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2slwaydtn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2iutkmvci.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2fibmkbjy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mycbxwer.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2djubziee.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2raiakyoq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2dktjmskl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zfjlddiq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2qhybnqcm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2nyntvukw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2eiuzwiaa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2urwjlkky.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2xhitqxrp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2jwfssscv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2iwnufkjy.html


<!-- 参考信息 -->