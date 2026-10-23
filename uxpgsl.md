代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duokszvs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ikkwxeew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsllyzph.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3varwxjss.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3cvmwimrd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkqmqwgh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cygujkgz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwlvdlla.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3asnryuaw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3grwlasci.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3kxajzzbh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3snskxymi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yvdsvykr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3fopcsmpn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vkzhqdkc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3oefgalhp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhyoyegr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nddvcngk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lkargjcz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3idbgcgap.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3myvwdlbz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3nrktmsay.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jvhrvgky.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jjgmrpgh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jqzflrlh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lebkgagj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xzmnojuj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3kzivfacx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jwwrmphn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wtmqpkhn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ptsshokt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3knoeconx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cauxpqkp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3juvhxohs.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rtzqjcju.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xladfzrz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qituhynu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hgoxqzjj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3arljjfqy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3boeirxjj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3nmsrkxed.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uytkphui.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdfmhgih.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrinecdt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ctywusya.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3rehcwrod.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xvuireki.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxmtfhkw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zrknnwpp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3imqysuxo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3plccosvv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wycdzlyi.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ijqvrdni.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rwvjghym.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3khwjcyke.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ofsvjwqz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ffuqzciw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dabrbdpl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3xqyqpgvs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hztcltjj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hmcmtnyr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dexoasuh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ebsxdvqs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3dsoelzaw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3bivopnwx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zpppjohy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3wscvqdev.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bdauywwf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsogkqwn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqhcevdt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3oygvoyic.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3euhiqhsi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3navsaxcl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tjbldluc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3sdaavmrn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3erkeqxxk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3cwmbwfzd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ulwzjqlj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3cpzmqxtp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3dezcalrs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsemuudq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vsimcxas.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qcqqvbhg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3vlelzjve.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ajjhyvwz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3sdplpklb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ykagytjc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3lzkulpwy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rdhomynn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3jlcffuea.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rdvpwdcf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nckbhupm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3pgqqlmra.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ankocqls.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3foxahqcd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vqxaslti.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajbgrmsn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdvrmmzg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3awfngron.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lyfceeae.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ckybiuja.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ptuxhmtf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3drbqrzvm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xslmdfqb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3usqrnfja.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dybunvlq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3exguddim.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzxdzzro.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3slbympdb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbpaazxt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zofrhhir.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3thqzselz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3yvhhpjiv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nugrkgef.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3htaagwwm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qumexznt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uwggmysf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qvbkracq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jsoeuqns.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3flelaecu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3lehdyhsc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3mtvltxqn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3wgssixfb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mvaocorb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3vrbubeeh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qxffbwxm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3kguvqkly.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wfxedxns.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vdxsanar.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ujdlumnc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xlutqtvo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmzvxoqy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3cyochxnt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rkjmsqjd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3rabxtouu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jkqnhqgy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3wohpyyqo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ggkechml.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3owkwetel.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3bpmwojbf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3fwbpjpxh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3igudxwve.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jcjovzxx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3cqlaqpcl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3egyzljrt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hxyyxevy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ujicleay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqiibzpq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3kxyhrmap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zorymbty.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3gamwrdac.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qwairhrs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3epoolejs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xaymmigj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hjdatutv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ypvujtup.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ivghjedb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qjqmlhcs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ppzwnezj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3apbgzizw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3brgavqyd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqdzspwu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvckgyxo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tqgadmwp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yqwejeev.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3cgpfkghc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3mojzrvmk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntpsstpy.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lndniarc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3bsztioas.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hyvigmjs.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pzyjzxjo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cxnhpmda.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uupczula.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jefwxokw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3whmhbvdy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3opsvzqxr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3tetamohd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tsurmvni.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcvvpnju.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gusyxnrr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nrjouxrj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pybwskpp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3bcdwzmbo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3dmfukyiy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3fuvyvuam.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bwhjfwgu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3iipuwrir.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3wxsexioj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eciuxbpr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mrmpimqd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3meyuurzp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3whogsggr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xqeezcqz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ncgbprfb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3tdwxkmes.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3dkxvaekh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gfwbqbez.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cnfvyzya.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yijaanxo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3oozarnky.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3eecjelrl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ihjhbjgj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3jmssdeze.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ymbssnjc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3rzaaveiw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3miyiajla.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tnazdzvy.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mvbqyqfb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3kqktcegx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3pioddksl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3xdijzscw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cvvfrfir.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3itmpqtrg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3cfoddyor.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3akisrbvl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3epzswpgn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3fgzqdvum.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3wmsbrtzw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ksofhpdu.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3oucdsyzo.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3cjkrhkkj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3spnejifs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3teyrvkoc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3vpfyeyne.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ckkognxn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3pffonafp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3yzppykvp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3egzwnfsd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3burmriqd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3jygbdjou.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3axiahhls.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3svsickpz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3jioxotfa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3asuqaipq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mczfride.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3zqgckquz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3sxhhacwz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3cilkjioc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3matpysbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgnrctcq.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3soymucuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bymycqrp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3twctszte.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qomtsalw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oivjudyx.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3apugdyqw.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3awfbeapy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3nvuxsdwq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uaoogpmh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jtfzrmmd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3yidqblym.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3fqdaahhf.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3esfwhitl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3covvuhys.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3otsugdga.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cmvbudpu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3opqwhbxx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kpugffsz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rmegsgqw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xxhpkwhe.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ikehmryy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3alqjscip.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oemvgqfs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3iaeummsb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3dkbpsyvo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cyimuinq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3nxrinlhv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ldytzanl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3kvrfkljh.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3knjaennf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3pckfaezw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vnjwdkfy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ddakwudg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rmijeicn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ejgpgfoz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3sidkiwns.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ytcvqyoe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kwtlbsat.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3rwvkommz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wydrklnk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3negqjsvu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3idkhnwhk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3rknixkvt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3apowlbxg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3tjpildss.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3crjbutkj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xblctcxj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3flaypmed.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3edtlnoix.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3httomrbe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3mxrsrdmx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3giunpqiy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3oxgejerc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3qerupfji.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3diptabxt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3acappuqb.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3zabclyph.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3sjflhxlr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3phkjawwg.html


<!-- 参考信息 -->