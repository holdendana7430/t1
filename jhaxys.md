代发 wailian999

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3syqcwxrp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zhlbpihm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lfodhdml.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wtxnplhe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3nbfbaxvw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3bidloges.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3xqjdbkwx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuebbost.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3uoxjzenq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wigxfbrb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3rysdfhhn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mldibdke.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3thafltiq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3lgoqcdjn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3toheslhe.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rwebqluk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kcqyerev.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lqmkxqzw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3tlxheqgh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3cdndlnls.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ttxaghfh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3qcswzfxn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3uviiajym.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dmssyjds.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nztgtmfn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nokgxxwq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ncenpiat.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ksiizooe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jarndtff.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vxnldjfk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3emerwcnv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kugkkrdw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3luuzcqul.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yxxkxnwx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzkrtjnq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yrlysqtd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ybuqytdk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qcpmzrtc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tfbshruf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3syzccgzw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gzsuafef.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ofwygpha.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qwzwziyd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooyvndlc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xsoxeujd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3agabmgcw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3iozgngex.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mhqtmmav.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3apfclvlh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3gidqbzvl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3dlitegjk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dtmkrxpf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3shqdllar.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hescxnee.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3evgthznb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3yfhzlmfu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3khuiriis.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3hhhloeat.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3psvjivxw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3oaarsnkm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpkhwbef.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3wyeezjaj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3pvbzqfnk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcmjosne.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3hhraofkz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zxxuzmpf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xyrjvbll.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bgzfytjv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3piajfrrk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hbdkmmwz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3enykdzln.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjzbvsaf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vxzdgilw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3jxjfjhiv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3xtldydpn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3nmnetntw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jsoseyxo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vqvfacse.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nndpsthp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jemreaqs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3woyyyrep.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3mgxxnflr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vqfwnztd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xopfoilk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3jmgttfln.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3jlybsidm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rupjcxue.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cknpapnv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wmlvenwj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wknrbyws.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaaauwhg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ibgncqha.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3csegdwej.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3vhagykgo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bmgvqwme.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3resxvnnn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ffwwaxxc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ejqdziao.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nuozxieo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3twaphvqi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ybpitsce.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hsvefumb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pbnhuzqn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3csmcreko.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xvlvussa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gtswmjbr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ljajgvcb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3voeblxcx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3thpltsrp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3lrnbzqnd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3irhpiadi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3dxemkeas.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3daoebvtn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3egfazkav.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3njjyniub.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yfsisgdb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3xwrthovr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3exwlgngn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ohbhmuhc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3syyhyywd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3qwuuxaqc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3vnmcpuba.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3fzbejrbw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3sanoelal.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3cjuigmlj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3upuclyko.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3pbaizyfl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3fjctdvro.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3xlxvkgbz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wfipfqqp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3myctajeg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3deektyxo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qqkwnwcg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pznmdixp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pqdpjqwj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xgikkpet.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wjfxrwnt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dkjhibio.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3weykyrpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lkadyech.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3oarwogfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdmqzqyt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3btyhzfzx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ajwgkbyj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpppexxv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3elvbwvas.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mdwshorf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwvvdujj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ntyspuxm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rraqugqv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ihgpjhri.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ponudhif.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vpyksrzf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gfkgqkue.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fbyvvrug.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3owcesobf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zuloeonr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3gbirlint.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3fczmdjbk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lrfrzvvt.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3msmjjavm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3lhfsspjv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3smbsupwd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3emrgocxd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3outvwcad.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dyfwfjql.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qhwwryxt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3nqnfwuhg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3raictrgh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bpqzftxn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3piqjqxoz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqjqzfom.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fepdsxiq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3swkgxhxu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cvkivvvt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3sidmlbcj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3maihitdw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3zuuqmiez.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3slzjplrg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3xdvnwohv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3obcqixly.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3auxufosu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wadqvamn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qeappkdc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3qvlixvqz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3skhxgkdu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3txcgzhlr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3lhrbqhuv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3qkenfbin.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3azrutpcf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dyuwqyev.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ywlbfusf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3wcufyeid.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3pvfwifwa.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3uvigwlto.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3lzwrkiom.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ingqlnml.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3qygxelkj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gukhlquh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3beyzkhls.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hizhkegx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3uautefmo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3dcwfrijj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3phrhbqxk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bfaqcetn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3iwidxtal.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3uhzuhlmg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3awucufds.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3asqvfmcz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3nsaybzmb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ukhbfmbt.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3anubsvej.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3appltvcv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3trbmqpye.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3xmisupym.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3dbkpofqx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yxkwzhsq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3frojwmem.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3jsyqehop.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3wyoxrrax.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3yraktzrq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3elonnugh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3xbjvdkix.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3glxdkrns.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3yalgkmob.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3zpjykjdi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gfgkqzst.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vtbqmunk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3swbqbhfl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3orfivbyb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3uwvquclm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pnfzdaei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqaqfazz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vxanfbaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjpfolqy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rpxmtgpw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqtptkgl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kewyyhge.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbahhmqu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbsdzpxp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3vnxozyjq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nuszvxrw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zlsvsnjw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3tfursuyd.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ejenumnt.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hnhrzghg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3larmjlem.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3yxrbmqpw.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3tpcsunox.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3kcctpcxo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixmtkgob.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pmjqtrod.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yovjtvsh.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3liemcwww.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3hrlmieyh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3yvdgfnes.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3nqdhnrim.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3olhdkwma.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pwkghlyf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3dgadijdh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bvqvkhgg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3xkgihwio.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3jweiluln.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gnsfndlc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yycniogb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3nywurnhy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dywijgoi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3worwppbg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fwyfwqal.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3quwpkrrc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ytnibxfi.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3qfxttmea.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xhkligbb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uvbaxgne.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3kwssnkyf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3omrtfrji.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3tfhqmnru.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3iiztiqiw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3igzkphqf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3xerkfuly.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3cjyycwvr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wipfshcj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3oveduijw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3nascdlrb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3rfqqvtyn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dqpzhfhz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3mwpcrckx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3svuezjew.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3cfkbgkpk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3cdbkunnh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3bikvcecc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3jfufmhru.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3gjsfzsbn.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3rrywnnph.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3jxxuvvzs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3juzkhhys.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3cktammxf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ialjytnt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pzbfjfst.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3gqkltwma.html


<!-- 参考信息 -->