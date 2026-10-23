代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ynqfhrak.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xvalnwct.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vlzoctva.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3nyljkirs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eozbqzke.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3wygvzbot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3faalxuop.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3iftmwrwe.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xsvpzbli.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vhxnfxjx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyghxzlj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjpbnptt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3idyrdben.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3fldgfqeg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3pdrvzfkb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3btznhuem.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3dnysortt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3juwannps.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upfkjero.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qvnmwttm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3frglhmct.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ontxsfzc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3dwsiykiu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dixqvhsj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3owbduzeg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3cwbdajds.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gcwmzwkz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3quercjfb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tcpshwzp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mmqyiagj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ezwwepyb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3cmiysfih.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zcasliob.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ujeqqkxb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3skwdbutq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wsyagzop.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3olbqisvv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ipwjmqpk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tzougqeq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xnbswwxy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xlmjhvik.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dzuooosu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lghwrybj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nthnllsh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3cemxhjcq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbrudwkz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3irfnlxyp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bluomsdw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xmjeftlx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3dzgdihex.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ghhmifuc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wmhkcawt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xmszkfrj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wlolbrei.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmxmgdtq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vxissrbg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyjbfnhk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zyepoisu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vidovepo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nnwtyxma.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3lscnwzpg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3kcbobyih.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3scgpwflu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sizdqwjg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rtszbvpi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qssevyzo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hljjigne.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3nznbdxqr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3mesyhxrw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3pkhoakgo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rytsquvl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3zldymgng.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ybpdxetj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwpnfqyh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3orchvfkr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdejzivm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3qbsdlapt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ldofxbft.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbvzlqsh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3rtappovb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3bfcjuwfk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3onkkzpfu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3mhwavsub.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3euhutjmv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3scgwyrag.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xnnatxos.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qcuptgnw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pjdnpidn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3pkhaodbp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fcvhcgen.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tfeowhqm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3uxxwuiil.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qrngwdtn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ibcbofnc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3tpchxkgq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vlnctctg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3wiioazjl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3sfggnpon.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rjnwwubd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gsxtwgzo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bljxssbv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gougioiq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kzmirsgp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3msxlxkdu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3htdiulau.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qcbmlpbw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3numicghs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wtxrkpha.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xatpaoak.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qoofwonh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxygiory.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fzrgqerl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tzfqipsn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aktonuqf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dhblljoh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ohhrmbnv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3swglddbr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wfjpshum.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fxfptvqi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hezfejql.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uvwjpmar.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3jkkarzan.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xwqrzpnu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3cosvqafw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3aksspdnd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3lljjuyyw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gtaqpllt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qwkmsxoo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3buqnbkvh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3npebeuwf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3aihvsicy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3mhhtdhsb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nbkrygmk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tzvywlyo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bjknwzas.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3aeolehta.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xmhznrry.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3erejluvw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qxogeahu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3sjcbqklk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ahkdhqpu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cqwrsjfr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3yiwhffxe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jqrsbobm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3thzvtvhf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xzurpfcb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kjfdvtwq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ynnftelz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3cfavtpdq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3gqroogib.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bvtvmoam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmbdfnpm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wjzqbtde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fudosxnn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3rmbhyvdw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3tolymrrs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3iyjgdriu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3aplmoksm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wasnrrdy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3sgpqrjru.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3flcbfkhz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wrlyxfku.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3tnzxwjay.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3sftmcmvi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3bwgukgye.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bljaajqd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dnrekukv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cbkfwbmw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rzflqjyx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3gklvxrcc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3kmlakojh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnftpnxd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yijdprua.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3xzjvcedv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wqefxggd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hnvbdsar.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xclmlvbe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xpytoklj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3lguqjmbf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ymdpuglh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ddiyhphq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jebwmqqu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3eqyllajk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3moqfekpv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhjxfecu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3glalszie.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3igevovcq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3cxpxcgyl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3qgzpbbhl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3kyxrojql.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3nzwfnnik.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3eocfshjy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3zmugqljt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ihreqjli.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjzskuju.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxdknemg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qlmshayp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3pezuekdu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tijeqidb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ysfvvtmb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3mjplsjqs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3netkoxyc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3adpnygbr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xvurubpy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qerfuwhu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3smwafvga.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ezriiefe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pyngafgc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3jclkryur.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3kkraoiwf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rjmacswn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ksylpwgl.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xzisisqr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3jknfpypl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3dkfutziz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3fkjfxnpl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zxzacxaq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3txjfdkbn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3kazilhbd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3jcxkoxin.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ifbletqp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vfralcjg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3hmfkvkeg.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3uzmjrqfk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3cgpeqibu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3citzzoyz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3zxattmar.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3nyrzrwgc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3nnxdrtya.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3atpwdavt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3wwsetutz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkcytmwm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3gzamqczu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3nleowuur.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3oprpmkgb.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3vjtubpnr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3odfnrgpg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3iadehpgg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hytdfufh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dnqpsgrt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3aeopsfrw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3uezxvlym.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3yozmusen.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bmbvtjpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvglxfnk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iipsoeec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eimykxni.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vqsrycgb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ubtfyevi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zfutecgw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3axtyhjli.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3csgqexui.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3tcrmutxj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3lubzgicu.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qkdgggfs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3bbiswndk.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3bzyaqtmf.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yygetifc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3aenlyydx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3vozrnnyh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3pwkxphdf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sfjrhihb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3mwzrhztt.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3axjmyjkr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jnkqtgxs.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3yfjstkbc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3snygqctc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qdwimdky.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3tfyhnzwz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3eknpbblc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3pdyujcbp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3croleytx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3dtopgejs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ojxjpxqb.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3zirccknn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3hbrgjbwc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wnniuqyx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vinhotkb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zhnlftxd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3yreemrhz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3nerkunsw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qeiwvbki.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3wmfgsulp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3jgzarneq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3stwhekcf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ptrrcxut.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3kkvvaxyg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3stqvyjag.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3bliseohi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3uemfksuz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qdjaaaii.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3plxlfifx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3lpvfjphd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3azndyjff.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3igguufax.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3cqcmbnev.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bfbqawnd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xiztjtjo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ekvpshwd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3hpdygeme.html


<!-- 参考信息 -->