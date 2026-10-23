代发 wailian999

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3whzajhtk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zofdmafi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmqitlon.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3qamfrslv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyyonvbd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3giriecke.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dupbgimd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nvgopczv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3takbwzqk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gfjmcxbn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mzjvofww.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fhtgmdgn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srypyoni.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynajedis.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vrxyccib.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3jydqnfcd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujrlckpz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dzfjdjra.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qaaosdwb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ggohhqyr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oigjdzlz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zqjablkc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3qzyqoyrn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3qayjljxn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3keshftvr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vbeqgkya.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rnsephtp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pfespoqn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qqmwpnnq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ujzlyyhv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3idobitnj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lynghmpi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3htdfeqvl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3unyumvmd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wfkwtnbq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3panngvhy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fiuidxnk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gcvzmihn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfczecaa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzumafyg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3urtftudi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ccwfvpyg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bpvjhwri.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3trtcsqui.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gkpgvngl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3rpipxfna.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmvwtkpk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjvoueum.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3phtdwhsa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ryaujzpm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hyojnpwo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gpimeehx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3cvckpnhj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3edtgzxlk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3pkcsdmmz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zhqkklfz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zxufhunx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ufsdmvia.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sxwfgsqr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3olpxfsxn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3wwhirhra.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3aywwvyld.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jjojirnd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ppjsoiwm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3sfwkkvyr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3thboydan.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3khdfuxkm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwqwkfei.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3idimbzvk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3frnavgll.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3elgmcqvo.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qzqxlsyj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3erifrmcr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xemjmfdv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3zhifpymf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngqybszb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kxjbbxsn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ltxrexwc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3azklgkpv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3vzzqceqz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jctlphdd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3pvavjeag.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qfalezvx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zzrtuywd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xipyfyma.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3mhcwnfwq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wsadiyru.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xwazwjsi.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3nwudifyq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3akreojyp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nzgpmdmy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cotyyiit.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3candbpsv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3iflsvilm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vaikvtng.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iltvlkkm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3tpvrogmo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnvwlcep.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ohjftdlp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xaqstbvb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xevvauwf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbenwhiu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3warzlgcd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkjalxxt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lxlqmwge.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jyzvrzyv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qpmbkizf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3oiuhvcdp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3nbgcfyma.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lygcanno.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qafetfdg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ntpjlviz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gpufglko.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3eipaffwl.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ynkfhlnf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3aefmyixu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ucjcgaux.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wlhyqeqs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mahyebgr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kypruppx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3faitsxsr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqalqflw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hpbcrvdi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3fmvsncnr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3cskjzdcm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ilgtzxek.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3wamdezpf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3byfmlqbx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ygxssrcx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3icfjwfvi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3rzncatkz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3lpplzdye.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xvvzaplw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3usnxwbfn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vdtzbnck.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3twbaqymr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3boxenqap.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lyppvsky.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3edmwyoal.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3notwhlff.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3dwiezbyg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3jegrbryk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ghuyrbhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfpexqtm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3pvnnanlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rlgtvqqa.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ytsupwyh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ilkhbbbb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzbqyglb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnruffij.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahnnixqk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3scoayzom.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3bhdmdenr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3nzbixdqd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3odhufoqc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3yktgnywi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3oqshlamb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nigmoatx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgvfnmgz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfaffulf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwttkycn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3kvzcdytz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ipmakmqe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lyiuspdv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3owtlxzne.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3nivackma.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nxaoblom.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kbwwohau.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wsmwiotu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hpiybjnf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3bufmducy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qvglajhj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kfkmeffq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3naqahhau.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hmtrlfgv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3stnbpgsv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mneibmzh.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvkkntta.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nqwaxqvn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3bmxglkoo.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3aevvwieg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvfibtnx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3wrsfgsyq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3irttnuji.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3uwvszoip.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hirgfxha.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytmpciww.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwnoosdo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3rtgjihjv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ymjlbdir.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3wknpxxeo.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3kmghdpdv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3zgewpefw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yeroqocw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ldvsbjms.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3nxrtvnbl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3obsinlux.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3pobabnnb.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3mlewupkv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3odiviwue.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3xeziehub.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3niflicxh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rbyzwfrp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tyvxoafo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cveuiqcx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3llxtpidi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3oyqcoank.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3wcwjjfyg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vqqushsz.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3dpsybgym.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3wpkyiwpy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3bychkodw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3kdfilsum.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3jjoetqud.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3rytwwwiq.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3tfwoipah.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3blvkmabv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xtkebesq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3qcspofll.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3utsskyol.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gnzfetae.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ndfwfegz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3bmylvsao.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3qidfrmmn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3fmlvelqb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3wbmozqcf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3tmrqcnom.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3orreqyns.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3jqyzkouk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3bgghkncr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fhzbbpgo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nhefrbxk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3xnrkpdeb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ennmvjmz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3xqkofsko.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rjvdstii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uthcwmdl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3erwnubil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lkzowzbi.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pfiinijc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dpgmlwyc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yqsurqtu.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3uqxutwmr.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jgfyedyt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3hrggzkjy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3nfypgqng.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rcyvjhqz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ydgyxdwd.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nxjycgsd.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3gbrsazyi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3olkjgffr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3abodnfed.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3vqqrvtrg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wgsmrxzj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lplavcwr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nzbhrzxv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xqkhvzzv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3omnvdyay.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwwaiejj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3jakglqym.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tvkgppho.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fwaodjeq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lenqgcbe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3mbujhodd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3zadbcvrm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3plhtpsvf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3tobztsnf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zqnlzgaz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3iaygsrob.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3qrragskh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pdbefnyx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3evcdifrb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gxoprsbz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3mflpcesp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3sramatcu.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3sctcfyqg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3lkvyfkuy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jwwskohq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ovnwkzkr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qewfyqkz.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ptztvkos.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3nhbjheve.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jaqzpqzt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3esybwszz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3mxmoytfc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ozuovcih.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3bobdukci.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3drafdqyk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bcaoyubo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nwrwyiyb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3kfxgmjlb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3kfkfrnvt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dohxvqdh.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3tthrxcyt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3vryrgeul.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3rxeupdiz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ngbhpxlt.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3xgopkwpw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3gtocqjqb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3xaybzzts.html


<!-- 参考信息 -->