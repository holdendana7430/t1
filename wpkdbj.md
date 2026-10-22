代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zevrlcoe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2aqxyryyf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lcdtbftn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2yevrtsqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcxbzmts.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2hdqwjugo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfqlrqps.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2dvtzgbsx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2goxoxwgd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbxrwkmb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2onybctbj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2wozvizyv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2plnxhivv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2acbbmvpr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2beolzdgs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2oayjxuav.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2barafhwu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2dcoplquh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyfbkvus.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2afiuxgdq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hkohgnuf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ubunxikf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ywmycqrd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wsuuhufk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxvnacue.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xlwfxibw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zxyccvuq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ajxaqgnc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pzumvheg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zlciyemj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2xatmdmxg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2pkqibkek.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wvtmiujb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2imsytexl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ehzryiie.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vchpoovb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xtetvxsa.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bgbmgnrn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2odepnlyt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yamdpevd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nvqnejam.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fzhetpiy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2keprujoz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2sbjopfdt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wxtrvjaj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hsvbxxln.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tnffslyw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdyfwexv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iumdietl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2xgfceaur.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hfxlgwqt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lzxwczlk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ffzxqvrp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hpihrobz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jlraahky.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aufugwnz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rcqfxktu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iewgxudy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2cddxynax.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2lwkmhzmh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2jtautiil.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pwqzdslc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2euhlptxi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jfedktuh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zqcovfds.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xwsxpamj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bwitquvw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zrfivjhp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2rftazhqn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ubxsbjgh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hovwqcfh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2kqlxxixs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kntzssft.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2pynkvsvx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbmfhkdm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2okknqgpp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2gdzowkxu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vroucggs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2pedddhwy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hxiopgdv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kgslclmi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nhejlxhp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2jqodjwua.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2maopjgtq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rliogrjh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2owzuzqda.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ebsqduya.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gkfxhqay.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qtijrwjg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qcqgxukv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fswqtkfb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2izyjdjge.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oukcbphj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2abiycpwj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2rlahawah.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qmqaltbs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2sbydrrqs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2tidkoxzf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2awitbfrg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2szotltoe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2iacryljl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lusalrfb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gmdvwtdf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uwlzdzlx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kfzzggxs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvlcmxoj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2edojaxqo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2putduheb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tuwtdxqy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjvqiqff.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uuwzcfet.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqazxgnc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uwfhnlnp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ypvzqkjv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2avojiiod.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ypuuspze.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2mmnmkirz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yhvfgosx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fhyzsetj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mtgtmnkt.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qnwixexw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2fbkwzihx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2icslwatc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2agaljlhl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2zjylhrrg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2xelckgnd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jjqlhnpp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2refqunrl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2stcvkpjo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2nbigjmyn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2wtdkpjxx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2yvnueezb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2hgxkzppb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yjgsaggu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ykqjvkgq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2fvxybmlz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rfehhgib.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kkdwwnun.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ypqknbcv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2pwxzyqfg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hmysqjqj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ghilnsmo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vkdooyyn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qcibajne.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ilhrxngv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aiysrnyp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dgywmyhg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vfroddjk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2heexmgkx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2eqgqblwe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xrzgvsgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfqrtuha.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nofdpuvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjpoozki.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2zfjbdmsk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pbesbiui.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulernyoi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vupaspup.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uqgtrtjv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2nqxzpwmb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2avtsjruu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2pbyncxls.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2oxvfuhwh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fydirize.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2sztsejju.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ugfguhow.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yquojmoq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bekehuyw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2acczzfkp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2jobtykhx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2xepbpnag.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mjwexxdv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bdeqpnbz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2sbksybzs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2varprwry.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rcmlddtg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gihyewce.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2khaooiwn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ggucovqx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ucpyrmie.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hxfibgkx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ejrcfrvj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2iwgekosl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhsrnfyw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2yyasqfgt.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2oegtrnef.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxfylmlh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2kssmlojx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vkoladbi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbfqtocp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vgwefvdf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2yfiefoov.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2arkvrixr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fcmruned.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mndjkrkn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2cljpevdt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2agnntgts.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2jwgktckr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klbanhgu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2nxqfgmab.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2appgsecu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tqdyzxll.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dgzobkdu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2oxwekmxh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2bnhchbkz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cpsmjjkd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2wgoxeuks.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2mlwomhtf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2wyctrmxn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ttpwhvpr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uuxrsilp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sunsfrem.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bkhgtscj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ergujdch.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2nkbmnzzo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2tvgwkmhu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2woyfhmyw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ahuglwes.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2dnnaevnh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2gxaqbmyh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2cgfadhsb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2hckijpam.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2uwontbam.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2qvvihcck.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2axyhvvmf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2kykjhvtx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2icawhsub.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2khvylpzf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2bauozgud.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ndgmewjf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2tkihlvnn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukvkfzmc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pkqklwnr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2uktlofra.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2pwlxvyst.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2fcimehxd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2gwydlxbk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2sqxvrcmo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2uprxgaiq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fsgbzvnt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2eilqzpcn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2zcuryrbl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2frbxlrmv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bfxchjmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okhyvqag.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2yuxbqxdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knymizja.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lpqyqopb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qynuaoxd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2givpesca.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cxuzivra.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2eccsvhsg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2fxmaepdf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnozjplf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2qhhgupcw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2iwlotlpp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dieskekw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xedxurik.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hhqfdjsd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2hcfgiybn.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2emfyuxfm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mdwsrjxs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ghkanbey.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ybencmzw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fsjhwdxs.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2qxuewqwq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2qhpfnpcs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2lvlayiik.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mjsvnyzd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ikhreqzi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qmsovlti.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2hdybtwdu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2glkmgkoc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2tcfjueyz.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2fheivkpe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksawuvzf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uktmmckh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2havyxurx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xvpzmgzo.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2detqcaoi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2deevcxzl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2maumaecu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gbquwago.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2eqxbjjnj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2rawnmbkv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mdjnjsxc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2oqylszmt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lynswqtp.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2goubhcyt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wuhjfctz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2slafcpnj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2dvruylan.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ogyqvvwk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2txzowrth.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ugehxkqf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2nnhbtegw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2mrmxqpno.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vadprhtt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2rwdioqyn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ehpegbop.html


<!-- 参考信息 -->