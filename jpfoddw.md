代发 wailian999

Py:   class User: pass
来源：http://baike.fanxiaobao.xyz/Article/details/gwsdmhshv.sHtML

PHP:  class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjphxxowp.sHtML

JS:   class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauosysio.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsejejvwv.sHtML

Java: class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgkeohtv.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtbpypmf.sHtML

Ruby: class User; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyltrgix.sHtML

C#:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gheehxsna.sHtML

[G02] 构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyypvsvoq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fanxiaobao.xyz/Article/details/gddrwflar.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggusttzjq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsbrnvwu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbnhqxgx.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwdglqci.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkhmnpei.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gilaxgejx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/glrtdsykv.sHtML

[G03] 实例属性
来源：http://3g.fanxiaobao.xyz/Article/details/gmfctkefq.sHtML

Py:   self.name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsktdytiw.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkbjkpuw.sHtML

JS:   this.name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvklxjzx.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbswtital.sHtML

Java: private String name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxrlwcov.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjaikwim.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvmxtzcj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfjhqibr.sHtML

[G04] 定义方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gwppkqodt.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gblefhbke.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnockuqgi.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxusqfsui.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gffdlqpyd.sHtML

Java: String greet() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghqsmqmqj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/ggrciurer.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdzbcklp.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fanxiaobao.xyz/Article/details/gllzcbsrw.sHtML

[G05] 继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghueltrge.sHtML

Py:   class Admin(User): pass
来源：http://baike.fanxiaobao.xyz/Article/details/gocrdhqcp.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuzoityr.sHtML

JS:   class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvelssapg.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdpzmxfv.sHtML

Java: class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/giyxqvzed.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fanxiaobao.xyz/Article/details/gxvmtogyx.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnbgfuoe.sHtML

C#:   class Admin : User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnbrgljy.sHtML

[G06] 重写方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdcqkvxu.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fanxiaobao.xyz/Article/details/gllufnwpo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkdluupl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gphybfdyv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfesqijbv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdyxjquj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fanxiaobao.xyz/Article/details/gftxddjec.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fanxiaobao.xyz/Article/details/giiinzhiv.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fanxiaobao.xyz/Article/details/gfrhsnurw.sHtML

[G07] 调用父类方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkopvxnt.sHtML

Py:   super().greet()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmjubsul.sHtML

PHP:  parent::greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkprrbcj.sHtML

JS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdnjxeui.sHtML

TS:   super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvjxvbjp.sHtML

Java: super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbltlwlot.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjudonala.sHtML

Ruby: super
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrljpybc.sHtML

C#:   base.Greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gzzcksvzj.sHtML

[G08] 静态方法与属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gublpkslb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fanxiaobao.xyz/Article/details/gxmsugypu.sHtML

PHP:  public static function f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrjhhwmu.sHtML

JS:   static f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrpkjyff.sHtML

TS:   static f(): void {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/glowdyxgx.sHtML

Java: static void f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/godupcthf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fanxiaobao.xyz/Article/details/gyafmzosm.sHtML

Ruby: def self.f; end
来源：http://baike.fanxiaobao.xyz/Article/details/gyqrgogbw.sHtML

C#:   public static void F() {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghvsuoxmu.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqbwoplf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fanxiaobao.xyz/Article/details/gvzlpotjz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmpsivucb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmhdkmcc.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyctpjzhq.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gspjvpdtl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fanxiaobao.xyz/Article/details/gmhyrkrds.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ghchstywl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geavuayyr.sHtML

[G10] 访问控制
来源：http://blog.fanxiaobao.xyz/Article/details/gucyxfduw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fanxiaobao.xyz/Article/details/gpugkrpcs.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjmwtjmm.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fanxiaobao.xyz/Article/details/gtxwqqttn.sHtML

TS:   public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdoucfmi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuuyahwo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzvvthrq.sHtML

Ruby: public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgrrofue.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fanxiaobao.xyz/Article/details/guwbdqzot.sHtML

[G11] getter / setter
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsvnlkat.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymodebrd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdgafnqde.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjcwukxqt.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbbyogcnw.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdqvtaou.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyghldso.sHtML

Ruby: attr_accessor :name
来源：http://3g.fanxiaobao.xyz/Article/details/gtekhstgo.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkleyyad.sHtML

[G12] 对象转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmlmuyqtb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjicxpvfp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnibbwqfr.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcnxhnvke.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbjzpskpo.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjsschodx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsxeoqpm.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzoqzdxjn.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/gdsbjjmug.sHtML

[G13] 判断对象类型
来源：http://wap.fanxiaobao.xyz/Article/details/gomwkavtk.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtlepojy.sHtML

PHP:  $u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gyejwvcmk.sHtML

JS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvfsbdkh.sHtML

TS:   u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/geqlwihqj.sHtML

Java: u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/guvcwzqyd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmhngvjg.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goymfnohk.sHtML

C#:   u is User
来源：http://baike.fanxiaobao.xyz/Article/details/goozkgeqg.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjdasltt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fanxiaobao.xyz/Article/details/gznqtojzd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fanxiaobao.xyz/Article/details/gavqgisuv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fanxiaobao.xyz/Article/details/gytiwbith.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuplopyq.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggnhqmyws.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkojawcko.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fanxiaobao.xyz/Article/details/gedwauswr.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhckauzd.sHtML

[G15] 枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhmhisoy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqhgeien.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrwafwfs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpgiqpgu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gheeyvybq.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fanxiaobao.xyz/Article/details/goinpybfd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqhhsyxl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwhqmgqx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyrxstlf.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gecluzcbg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzyxjqko.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fanxiaobao.xyz/Article/details/glbtdcmsn.sHtML

JS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gwhqhvpfy.sHtML

TS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/glcokrexy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdipnajxa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fanxiaobao.xyz/Article/details/glzrhveqg.sHtML

Ruby: obj.instance_variables
来源：http://baike.fanxiaobao.xyz/Article/details/ggrdydzhr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsyvtbtw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gerzicghw.sHtML

H. 异常与错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gbkymaegq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnyhpxlb.sHtML

[H01] try / catch 基础
来源：http://www.share.fanxiaobao.xyz/Article/details/gibzwcjcw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnsxlynv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fanxiaobao.xyz/Article/details/glffflfwu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdvnphnvb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/goyursceu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fanxiaobao.xyz/Article/details/gmsecifdi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfdvplzi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fanxiaobao.xyz/Article/details/gpgohusop.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmliixvlo.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fanxiaobao.xyz/Article/details/gdlvrravg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fanxiaobao.xyz/Article/details/giwjgsfpb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gqktyqivx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/guhfvktkp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gkjnsnbba.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjutnpeq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzxajgwu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fanxiaobao.xyz/Article/details/gshngmipp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gslzaiwij.sHtML

[H03] 主动抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbvzjqxu.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godxliqqb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/goyzzkwug.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwezdusua.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/grlsyyzah.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyodwugo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fanxiaobao.xyz/Article/details/gckueadsu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqzxfbzg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxplftcwj.sHtML

[H04] 自定义异常类型
来源：http://blog.fanxiaobao.xyz/Article/details/gkzoqcdxz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvnqfcvn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grasvxhrh.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghhjnahsb.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/gfyfsacjp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuccccpu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbvwrcdo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gilofwges.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfvdwthh.sHtML

[H05] 捕获特定类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcvmepmc.sHtML

Py:   except ValueError as e:
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzcfdumn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzibwyib.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvokjbmhf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdfvoyjyk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmuwomkq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fanxiaobao.xyz/Article/details/gowgwdnsz.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fanxiaobao.xyz/Article/details/ghglrebbc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnokkrrzd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fanxiaobao.xyz/Article/details/gmojwmeav.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fanxiaobao.xyz/Article/details/gcodmfxuw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gmrqvrcsu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxotryfz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmgzmklj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fanxiaobao.xyz/Article/details/gapuupmcz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcphpitkv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fanxiaobao.xyz/Article/details/gcojiomim.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwidhmty.sHtML

[H07] 断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqhtmgvs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/godffvqso.sHtML

PHP:  assert($x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gsgdinlcy.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/ghrhpqklg.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxqrnoes.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fanxiaobao.xyz/Article/details/gtestlaco.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fanxiaobao.xyz/Article/details/grvzzatrz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fanxiaobao.xyz/Article/details/gdnbdmrgz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmovyphlw.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fanxiaobao.xyz/Article/details/gbahxefut.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fanxiaobao.xyz/Article/details/guweavpph.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gablpgphx.sHtML

JS:   e.message;  e.stack
来源：http://blog.fanxiaobao.xyz/Article/details/gdloodkkm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fanxiaobao.xyz/Article/details/gwshvvfve.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiwvfhxd.sHtML

Go:   err.Error()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuqrrpsf.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fanxiaobao.xyz/Article/details/gfhjpvehf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fanxiaobao.xyz/Article/details/guhesucza.sHtML

[H09] 带错误码的异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxwxkxuj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwnzrkcq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmldssesd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fanxiaobao.xyz/Article/details/gvswisokq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fanxiaobao.xyz/Article/details/gcvipobiv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fanxiaobao.xyz/Article/details/goyfpujqz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gkphukrtv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fanxiaobao.xyz/Article/details/goiviqtac.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fanxiaobao.xyz/Article/details/glmwusqhq.sHtML

[H10] 资源自动释放
来源：http://3g.fanxiaobao.xyz/Article/details/gjjapxuyi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrvfaxxj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fanxiaobao.xyz/Article/details/goxjaplyo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmzufbhb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/gnpesarow.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtlrdepl.sHtML

Go:   defer f.Close()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmexfaswr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxytfepw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gzvuopgfb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gimlyyhmi.sHtML

I. 正则表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gozpvydij.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhgtozyn.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhnhxxtm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gualmbeqz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoqxybfc.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzlpwfhm.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqqcvsrz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fanxiaobao.xyz/Article/details/gtprsidje.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpanmchs.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gzjjfeuba.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gakpxgbrd.sHtML

[I02] 提取所有匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrhvmonl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gcyqduxhc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greptjidk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhlybakt.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fanxiaobao.xyz/Article/details/geqefznga.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsovhbjoo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gndahcpzn.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gorifwgwz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrogrydn.sHtML

[I03] 提取捕获分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gqstshyyj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqjikxix.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/grayuomwv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gohgdjqbk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcfkbmiq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxlkeulm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpfccmfw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fanxiaobao.xyz/Article/details/ghhnznnte.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fanxiaobao.xyz/Article/details/gvmpnflhp.sHtML

[I04] 正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfogybpq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueztnebr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/ganmffztg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gzgrhfzgv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfugxmlbl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxcwmjxp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gvixurcig.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gpbewowcn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gahczhbmo.sHtML

[I05] 按正则拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpngentnq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsmiyxje.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyrfsgqd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzarlmcs.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gydwsiyxu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhcrzatq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gipjoeqbh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gyqrlgvxy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkatzoeuw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fanxiaobao.xyz/Article/details/gysjxabtl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/gmdvjwaly.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fanxiaobao.xyz/Article/details/gugyoebtq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfvvsbed.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzpqfojg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyzdcrgl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fanxiaobao.xyz/Article/details/gpetboxar.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fanxiaobao.xyz/Article/details/gipehgjer.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gcudqrwxh.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkjetiov.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzdonvpi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fanxiaobao.xyz/Article/details/gsnsarnwa.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fanxiaobao.xyz/Article/details/ghgxwggzm.sHtML

TS:   /error/gim
来源：http://m.share.fanxiaobao.xyz/Article/details/gzruzrgnt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fanxiaobao.xyz/Article/details/gaccscwjd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fanxiaobao.xyz/Article/details/gihvsqant.sHtML


<!-- 参考信息 -->