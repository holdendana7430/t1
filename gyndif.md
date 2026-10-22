代发 wailian999

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2dmfwuchh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ykkrldgj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lgngcduz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhmuywyi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2apigsnes.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2jthqantp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwosfdzh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pmslceed.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2pnpihuzf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2potokqpi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2nwrcnool.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbzhgwgv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2karevfcy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2egtxtnyx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2juvydwqf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yeabjpvg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nesrcrqt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lwlrvhmu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rxyixsmy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vbphlsgn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tphzmkaj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tyxppaqy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2aiytnfyz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2efwwjiue.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2srbfhnxa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ozotglwv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2oaplnxzx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cjznokjp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2frbfvlxk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2scoitudr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2awajaamc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adakyqec.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bjjgodzk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sgmrzklm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2clkolkts.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2obdruhqr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2pbvcrizo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2enbhoyty.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqgikltp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cxlvjhoo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktvuopss.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2dicinido.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zgzegvrl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wixsufzd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2fqeyudnb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hcbvydcu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yonxeyel.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwzqxpsz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2epijxfhp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hztqpshl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hewkukdl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ysmrrpij.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2okafisam.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2yndjxnsu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2uwclertc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2watgvlof.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kxdllott.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nalrpbqx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gbyxdmxn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ecsunlzq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dwoxbjlm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2adtuuozi.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2yxjnyjdm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ktnupxyg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2lrnbfhce.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jalqbsiq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ephcofhk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvplqaca.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2nxnmxvjx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2abjyrtnh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhyyrlni.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hbtprure.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2owlksvfe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2yejafypc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2fjayzybr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2cqfufpir.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2osufdizl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xctjmxdx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ofwoqjad.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xxmrigan.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xwdrpdxs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hfdfkqed.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zpaengqm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2heavjcyv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gbhqoplp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lyfpnqiv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xjhuhgky.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vudlbfbd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2kyyekrbe.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2yuqqonal.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2rkrparpr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2shdhduhj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzawsgjh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnwvbozr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mxunvjit.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fvjloeyc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2oewapssv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qcegslxd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2gbptxegg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vckinowf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dehanhnc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mzvhwgne.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzroovkk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2epwieigq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kojmldwu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2evqzkzqg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jlamcdrr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2wxjlshte.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bmkoejfa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nzotvezg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kkfuzjul.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wywymbps.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zuixjpru.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2akihxgyp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ebqwpdvu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2foqjvfei.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kmqvqzsk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2nfvyxzbx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wgxosxsn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2owcsraym.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vlzrfcln.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwesjjrz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2anvzfmfr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2czusubmw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xnanhfip.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iijavepe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2zkkhyzgw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eajpfngh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ryjbogti.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qsgvselq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2crdkhnpa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2okljcpbv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xwtfnqic.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bcjjrgfh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ojtipyrw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2zdzmhoaz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xcjkwawc.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vktdfkye.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2butwggfb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jbuazwqt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2qsiohhqi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2hsypqwca.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vlpltnbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owbntbzn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2julydqha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czgufwcy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xcvxpllf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2pjbpatek.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjineofh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhuvvgft.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijyrojby.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tycgcgve.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2uboohshl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2srapbeeh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjhbykau.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2zlfcfazj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2vbtrjwab.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmqjqxny.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtjskrev.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrzwcjqm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jgkhpkxr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2tqmkivqv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2clptucen.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktqqbjxn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qytijdfg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2sudxbslv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2suukgiyx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ufwnnuil.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zkblpmhs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fzaegmem.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2cnuxrspw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dlpyefnw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jgkvwhea.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2wgqdtgbj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ijlglszr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezwlwwgj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2aeyrucgx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xruaivsm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mainvuyc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2eztenkuj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2fckrqwbp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvfaphvz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ebhyxulu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ghskieuv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2gkkswsxz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2szksjlgm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfxmmyvz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2lsierymt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2tjxycold.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2yakeptyx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hibybedy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2pwrdtmda.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2lvurnwex.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2oectwdum.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rvxgthym.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2osmvryvu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ziupbwkn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ebtinylj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2rypdkxto.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2orkgekwf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2trlroqad.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2eypoiwej.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hfyodyho.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jurgcegz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qbrlzzte.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2mlhxufut.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2teviotip.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2pumrtxro.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fdtnpcvg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2bqrbiwir.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2bgzghepb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ybcxctjr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2lexctryz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2kuemullf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ogfldmwb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2dxqbazoy.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2sfvvdejh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2uzhpgmnv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2baaoncqp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2licbuiki.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2tlsopoyx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2atfmipzg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2khyybvkt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2hilegemn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2wzgkqipa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ptspxswb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2jddmbuhy.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2vbkxceru.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2aadeavxy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2dyvosvhn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kroelstw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2crpxnmvz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2hwfojkks.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2tpohvhyw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2gpukhczk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2epomlhvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjybppyp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2dhzlbvmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsgiemri.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2idmkilsf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2coahnyui.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mwfomrcr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxvbpurt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ohcjxruc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2jbomavgz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2tlhcfumr.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lbuossiv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ohqdfkqq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ofhmntrd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2puejhwyy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lcphbexa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2qfjsyuio.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ybcoobuu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2qxgljkaf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xcnpwipu.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pgvijcil.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cwxdsjfa.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2plqdxxnf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2xipsdusk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ijgfobfz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ntzmcdtr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ikdrkxud.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fxznlvgo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2jmmeybhb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2nzbzzusw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2jwbehhjn.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2btrtubjt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvensmpz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qmjoupwr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2yvswsinz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xmktnwta.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rjwlkyjl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2xcukaupl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vcficgzp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ltdkxxft.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pxjwrgzu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldtkdwxd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qxzraiqu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2najhpapn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zzcawtul.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2vgwgsutb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2jjzmnvsh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2egfyzivv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rdgsfntr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2qhwxkbvv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vkbekjjr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2utwdyxot.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zsblytwq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2cxmxtegc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hwfnefqr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ppfpmvas.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2savnubyg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2uwuikrdj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2oldvgkqj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2lcrggolf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2eiocdxyj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2voeortjn.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2zcgkewip.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2shesahtk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2nmwhuqrd.html


<!-- 参考信息 -->