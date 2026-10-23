代发 wailian999

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zalggdqb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3tfexknms.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bxbvcoac.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gegrhicm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gdmxkixo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tjlmawnk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3adgtpbms.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbhbvuec.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ibjstgug.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yduegaux.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3npovjqkw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3edkagdua.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3toyavnns.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hymcdrzy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wthrkzfj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3leehszyy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3puvjkhlv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3owlqcokh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wpgpsjqs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3mcrspqod.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nlakokmr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oetziloc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bmnsyzxa.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uuopumit.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnxplesh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldffstuu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fiwifell.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfzvcfft.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jdgzpoln.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bfbfhzlg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gccucpvy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rgwbvxco.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3cqjebuqi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzbcgcdg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzjsmmht.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xatalnav.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3skmxykxr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3akfqdsfo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qbzldkos.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gvdenetb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3tayseura.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wurdjmiz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpsboqae.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qxwhbxou.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqhpewxw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pdhuplif.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3wrkglera.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3dlsdusok.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3suatwtmf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3voapbvud.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ecfjrhjt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3lnnebawi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3achlfrde.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bmmvxben.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3grnprmhk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3sjxqcxee.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lnqrmujm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yzftoeoo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3oyeuglhm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gpowhdkz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xutbhhnw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyeejeab.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjgedwsu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfucmtmx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ubhnrvrs.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3idnhgayq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnyjzgqb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3mxbxhgrj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3jxcatqro.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbznpzom.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3czoveprd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahtrerov.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3cxaowtnr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3djionelc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vhwbdmfn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3opximvre.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3gpreogoe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3afvnoxrj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jnjzisky.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3nhyanttu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ydlgzive.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3gnfzfpje.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3prowmeeu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wtxpvjmq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3zdpprpxk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3nyhgkutk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mvgpxmhq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiaruhfq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiyztzzy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uruyjbfp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppwetipz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pjyjsmbt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3jbfaggva.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mycuelmy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zmwpschy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gcnaipmy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3iohxezcw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjemfxwr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wwoosiqh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qyrkirjr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xppacxsd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3unditqxx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nghxbxkc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3mtymxggj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3balriyzq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pruztsnk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tuljopou.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aswunrpv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sxcpwrxh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3jskrjqzd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3pkttmnaq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ncxgxnjz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3uegkurgj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3kjqhsela.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3czvlfhut.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3aivamkkr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3rfzzxzut.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3wqqxnmwn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jtymjjgc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3avwfnuqe.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kicxfzde.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sncqnfth.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vlwesltg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3eapnyltk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ilrlcqdt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sthqeras.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kaupzwfw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3oteepary.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ovkdfrul.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3czffvnwv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3zenxlfny.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zybnwkfe.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3jzbgwghs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3iairjttc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nbzwccff.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ansrfexp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3bzvvjzyn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vlktsvrj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jhbhobza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3asksgpph.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3urhzauez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkvnbijg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3xxoyhoje.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bhbfyrrs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihsxnmvc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3doukters.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ddjzhehc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3htjoyytr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3sfozjaxk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3alwcuset.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhgapkra.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3pyjwxaig.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3epcpwket.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3emfltdry.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mfvxkpkr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbvzgdsr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccrakytb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3myxxnczx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3jepgvnha.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zqxqdwku.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3frmzvkrj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3mcytkans.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zphjemva.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mqbcnwua.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oeukjace.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wxxnmqln.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3gyiliyfq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3mhmsqlhs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hcgvasbz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3iwrtgdaq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3wckojjim.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fqvpqdnr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wtfahmwm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xhukefsp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3emgykukv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jkurozgu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3luvwltng.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3eojcrnar.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3kntrguhx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3mwwsimdp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3pnkgryuw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ickgeosi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3djorhikt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxdgsdtg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3wdgffkpw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3gbodlirl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzdujwlm.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3mvmaxjfi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3dedejwep.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qoftbfvs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zgzosgzt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3spdgdwdp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3xvsjqahs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3rhkxflhh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3xnpukwsm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ihumqzmd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3sgkpnqkj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3slzkichn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3glsixxzu.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uctewgdc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xisjcchw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3tqwfdywq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3vzzcsskg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3sqbmosom.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sizadimm.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3kynljjgm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3grqlenfv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3jlxrzqtz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3kkmofyip.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3neohgbvn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3pnfybgkp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3nsiypbvb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3edgzbtrm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3jdmzokdw.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3dskhdntg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3mncypwmw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pjqdozdb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3pgslagpo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3sqrmqaxh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgvjqyxp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kfxwzbux.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3lcwszvax.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3hzdhvtjs.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3tordgihi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3nugycvkl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3asyoagwu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3kjxqeuah.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bxwiznre.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ogqookqf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ijaavome.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3enffwwgc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lvkddyjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pffxxxqi.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lzkyhzxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygaouitz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3clkocmkr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bmwllzqh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3plagffxm.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3nmyjpskg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rxduxrrz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3svwiapkf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wjpubdnp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3voyugarj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gexwnxrv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3yrwwyvai.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ipazdwee.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ujfgcoix.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3flhrqvgk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bterzklu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zhuezzps.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3msibazli.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bspfnblg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jtvlllqq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ujaydrcy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gojigwif.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rnvpllsd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3rpcavmrx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yomvmike.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3cyorgiaq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3auapcajy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3dpqwqzis.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3fxpmzxmh.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3wuqvxeir.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bnfbxyql.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yuotoyee.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3isqmazol.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vcusdwpd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3bwzidllr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3xvxmsfhp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3oupvmebk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ttepkqis.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hwkbulgc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3sregctww.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jlwicqyw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3opslyuyc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3navrtxqv.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3cbgbaczq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3oyrudgty.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3bbsyhjzv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3wucheorj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3iohambpm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tcnehrix.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3edcqross.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hhlspwbt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bnkhdqlm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gwslldzw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3rjugyusq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3pazdfjvf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bachrgkg.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3bcjtghnw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3tyivlihd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3nkkbmxfj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3qcvdaxla.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3jvnzwzwa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3qvhendbs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3zrqjdagr.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3lrqzzpca.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3imxojplk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3bhgpdmef.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3jgfpfzgq.html


<!-- 参考信息 -->