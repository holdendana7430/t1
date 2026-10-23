代发 wailian999

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3edmdknhg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pncladju.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ltjxqqim.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gbtlnvxt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rymmgvof.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3rsliqchy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mgyhslfq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwvwuzbw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qopfbryo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3yxnwvcpm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tgzomlyw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bwnokjnp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqbdfyek.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqssqnsy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ndsvhyjk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xmdufnzh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bheojkjz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vafhktah.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cylrzhkw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fsllpohf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jyhshkzj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tbayxewy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3gfbjdzfy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3jjbwlvef.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lkcdxtwc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3jfigtupj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3khludmdm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tzncztos.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnlmhlhd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gedrqujx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuofhyur.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vegmpxfn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3enaqjlki.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gchlxysh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3eopaxxzs.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3klnpdeqz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yeesdpzc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3esywsmub.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ijjugvwq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xuwxevzz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrbdvdbq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jjjclepv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gbehqobf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3baccrwzw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ztejjihh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cdseoetn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ostxbinb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uolbqacy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hukrgiwb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejgjfnpw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3djwzoizo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3xeydbqcs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jeukufpk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xtzyysfv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wgqflzrx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dyzkgags.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bjqytthl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hugzmnbj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aljohvda.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bprqowdm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ulwxucds.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jzgxaqjc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3lnywefnb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3rqkryukh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vovrdkil.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxgvqfyg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzgblivy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lheitceg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3liouymbf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3kzoqrnbt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lypgwxtk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qxkuwvlh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3sstvfjpd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkxzzjac.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3oduwshhi.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnhwvhzl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3freuhvnz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ajogpgfa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3mtpdiupi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3kqpyxkew.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vywvedtx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qgxznzlr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vesuxixk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3luwjpdsq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xavxmfjq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3upqtbxtg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3pwgrlooe.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hdmjlyce.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3jwwiqjdk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3qnzulbud.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3guhcabox.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dicgmduk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3oxnbesen.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyoqkghp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixbtidpu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dgbylgpd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3iflmbgrn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgqlhjmi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jnzapqdt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3prnwqgnl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynmpwcix.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmamaxln.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3edzdnhhq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsfvwkvv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fxsulreo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3trdecenc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3rslqtwem.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3jedidykd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3hrccssxo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kkhzbwdf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bnasejtb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zekstfnu.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cbyzefvw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ozxjxwlv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3appauacy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3reafuidd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3cvcjfosr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3nemggphj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3jogrmgjz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3nqenkfpi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3tcuqkveq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3tngpfcam.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3cotfmqle.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3phjejent.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3sbzddgir.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3sodmpchz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ycdxpqvf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mprgqbhx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hxkszzoj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vccxhbqx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3aurovbhs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3fooyudwm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rwwnesyc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jirplysb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3jicszjmk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qronvwkx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ahsoznvv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dpblcuvg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qomupeww.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3dpywaosu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ytthijid.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3rtbebrsp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qfpcbhqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvofyhff.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3zzrsfcwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpmegxnz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ohztqwsm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3oxlvddes.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcxupvyk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lmsewrjp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ehkshyya.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3kuioexno.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3fjbxpori.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3jkbvfzbu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jaavwhgn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wjlelbif.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3kbyxwgja.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3csqoppsu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dmwomenw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sfgeiuoc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbjpjddz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fymikaqf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3rjdiffqa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfixembq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3qdgoeilf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xjytjkqd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3igibyuuq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yducfddn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uclpgdcq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qtbdpxzz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3hmljnbgl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3rpjqitpb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hrysgnvh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3rovysfua.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gmghqmlr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbaswbgo.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hvpolsja.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3lzatbhfu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3snyvjdsl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3fphlivnd.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3xvsxlvjg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3nogekazy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mofvhvck.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3edvsiriw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3cattywtu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iivhwtao.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tfrgktri.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3eriejybc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3hmnypdpt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ckvbzhoz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmposblv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3vemehzyr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3xmvfgkae.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cwyqdnbm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zjpcykwd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ssdprcgz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3xrykysud.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3rbktdetl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xzxketmm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ubgnipnu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ctosyhua.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xkkfgwfk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nmvemrhb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dvalagmz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dyuobnsn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3rybvjaoz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3plhjnevu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3qtqvlapg.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uorpfove.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ugvdzidu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ujgdlhtg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3eqrawbqf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3vuwwyuro.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3deprjqpt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ixnouhiy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3hbhkzfpd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3dwmdcsit.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ppolctqk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xyxqjrxr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3eaflzabz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3vlwwpzkw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3xthgeaje.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3vfedthik.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3oohwoeuh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3oqlyzyok.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ptezfxka.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3jilvciza.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3etfjgcqs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3onivciid.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3tckbkffk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3abktjatp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bmruslof.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3pwrswryu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3reshrdig.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3dblbahoo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dunvxslr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pavlsxws.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3dkyyszrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oyzonpuj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3baofaxaf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vutocbog.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fdrxmzqq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3bvzpzskp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3dvfuhtqe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3mhcoeohc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewvdpxqj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ekbfzofq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lzvklgiq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ktxsoblb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3czzqgxsf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ccpwewpy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3tmmbmiri.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3uzrhwiya.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3auxagrzf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qlifowge.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qtdqffjh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wzvmrine.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3rcmfmycg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cflgwuju.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vpqwmuye.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mbzlixoi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3nqiyrtev.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3dtgrvvhb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3udseibfq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xhintkuc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3vznvztjm.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rajellgj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3hdjvgyxz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ilropnqj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tmzmjmmj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nzjattjb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jbztxkxq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3omogxdnh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3pogsbwxd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3jktrxxjm.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pjkfmmne.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wihpexwf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tactcltz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3odqeqpjh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3mriutzug.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3nbesmlvx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3lpkgruvr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3cnlkkxps.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3tjeqsldh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3byyhqddb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dlncieze.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3rkxncfkc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tpyevkzb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3kslrfeih.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3odktqssd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3dnojctvu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3crsnsgck.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3chneimtp.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3qqgfhuvx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3smgwwtpo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3useajsxp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3wzmxibzb.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3yuqelwbg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ntkqubmt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3wzgecfqh.html


<!-- 参考信息 -->