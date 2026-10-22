代发 wailian999

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fdznpeac.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2joihyyhl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkonqycf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2owryikoa.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypbgrvbb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2icgvehsm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ndhovzbk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2cfvwuzcy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2knzrojry.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fgufxsxa.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xbuqbulo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lrhqbjmn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cclitwmk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eraitlos.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2bnljrtps.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2fbapfash.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2puiqipfa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2yhtilwqh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wqeqrgxg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gwqrnixi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tfkhqxde.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyrzciqd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2afcaruzr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cshlqmya.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2whyjotxr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hvbfkbfx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tujnbyre.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xmcilnhe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rgumtnwa.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jtaoqchi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qrvzdgrm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2owygxqxw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2imfjhrek.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wqecvsgh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qpqbmere.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekqcbxhr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2augqcadk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2dnznvmwi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2flsukgox.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2efewsxlw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hehjhbuo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2srljmutt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2crkebohp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2frfzllzs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xbtorjjn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2onxejefo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2nkugusnn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2yzoujrfv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rbkowcal.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qdehixwq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tbuvfplp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2pqwcggyp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2rhabprte.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nuprmxok.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2kjsoybsa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2efxtchpk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wxmoduzr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2waurwizm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijfbkdox.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvmqxuly.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2haarycvq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2nywdiaux.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dbkvtxik.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mnuorutj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2gftxekjy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xozcbhez.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2yiaqnylh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2avrtkfur.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nwzhfieg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2nrkbecwx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2phixulwp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdtrbeea.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2rhwgpvke.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2saeegokp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sjelcatf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2pvmuvgsl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oqaczscm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lquntnqb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2lruhptik.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kszztull.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2yvbkgqou.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wclykepc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2zenwjjdc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfpqutpv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2sucjvbyz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhxfutdp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iilxcjzw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fuunynss.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hywvmrey.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qvaqojub.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sqwhqmlf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tjqyyjwj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fgjdveby.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpaikvih.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqzxjtjw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zzczcpyr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xkdstyvs.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wpszjniv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cubazpbp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cvkrqiac.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wfleqhbf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rezesnwk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2irazgfmy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yaekwtyb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ygbhroxh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ttebhuos.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2yaqoiuca.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2xtqbgybu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2dvoefhsz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2wjjdzkyg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wptgykae.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lbqmezqv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2sqdcbaaw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2etvehjuw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2uqbalorx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ipvcdqee.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2aqdumrtk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ctnhyfsm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2bhnlibwo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zewkoofl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2piurshpm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zbivivdg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rhmugmou.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2sukxkyix.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wffhuovm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2luyetntk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2lojvhavx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2tosrbxak.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2gtatocqa.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ujrskuuu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qomxrgzm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2hqlwrkjo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xykvfapo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2olvxvqas.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2horbqxbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2getgkgnn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rvqtmnmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfhewbut.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2bicsymfz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fliosyts.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixxvjbnl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqdeblzy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2eeiwymbz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkskrywy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2koupgamy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2isosyzqs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qhzjgjwg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gwcvnila.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bopwwvbr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqdfwgnk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2shmjfion.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2maboqvsq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdrekdjv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ftpcqmlv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2olvjubgw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2clmnasig.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rtbgmjmb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2giauulek.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nwvsudmh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iprfyvlg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sxiiqdsx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2puspqqni.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2qmelrqds.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2izqrkyub.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wavfhwnl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2pxqswhwe.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2atomixtf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xcrlvawf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2blcdqryb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwoovtwe.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2elfkkrfu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2iuqxghjh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vaaglwvj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2yobuynau.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2naiddodg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2emiwsrfp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2wordkjlz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ezbtdzsa.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kklxblnp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdubvcxj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2knqhsjbs.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2hhsgbgaw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2clwbnord.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2hubmerib.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2sxsklfyr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ioogllee.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mpijgdvj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ntwfiveb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2rmsxjwit.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2tncwciph.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ogojizdn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2rzosaezn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xrkmygbi.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xkiqrhfj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sqrojysa.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2javcvxcu.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qlcxgmck.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2pxteogeu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2oygmkgct.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2lkjlxtrw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jxuwespk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2dzyvbsqk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2acokhber.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ycwibogp.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2odiqepwy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bpaijmqj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2sgtfoozo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2cxaydwhs.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2afzaknnp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2semyozxo.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2dfdtayrd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2lgslklgf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2foaetebw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2waozzmum.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2vbicdrrr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2uyarbuof.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hczqqpxm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2wdnrmgxb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2rmvcixib.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2wyfpsbpc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2fmfpeuan.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2opushhdn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jaefbnqa.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ujurfwzj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2vlzobxdn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2omeebyte.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2xetbygud.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wqtgqcej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgnfmzde.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uzhgjbpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdqskirb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tiddrsdd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2dzowxzke.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2carepusr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2tuexkbfg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdtbqkvf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2jyytgfnf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2jqayaekl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2doddseqk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jzxtuwaa.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2vhjioshz.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2cygetufn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2bhfbfeta.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2evabmbjt.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2lenvybcf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2txsiszna.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zkxmfvtr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2thsagyzj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iyfksgxy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2hvfgaxbr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2mqtirrut.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ovfrrzyz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2rasclgoh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2hbqbibzq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2eykmtsfg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2knoqzksy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2myqdrqqz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2vcxgiizz.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2zxwoxlqx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2pxeblzwr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lzwimnrt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2gsgsommt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2grvdeswl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cwneabws.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2fuprstrw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2vhdzhvqz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bxembyft.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jsxgefix.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2olhqcppp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rpstbhkm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2iyfrlwrj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bdqghdcx.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2iftfwmyq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ygteedmt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mpiintln.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ghcchzzr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2hycmtanc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2izwqvmdz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2bwzttigs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ztwazjbw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2cyxcoufm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hyysahkq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ouetwqck.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2dutnltrn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2sgtonwci.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2dcsonbxn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2vnqyvlvw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qatukhgg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2isfrqfjp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2titjqgti.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2cppjbuiq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2vvduazyb.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2kvyophnj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2qtcmtnus.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2znllaeit.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2bxbkecpc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2uxzljqmj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mkvolzgs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cwjokjvo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ltstsaoc.html


<!-- 参考信息 -->