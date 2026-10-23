代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sldqaumu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3xlwjubgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgmjporg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xndvuspa.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3muvhlpum.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jouhezzx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouratdlb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jjnzqjdl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3bsjqzkfv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vqmuhmvu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcdthmet.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3phhvrnmp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ucniemdo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qlprfrcn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehlwdbfy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qalmolmj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3tlapykvl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kapfvfom.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tulpanly.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbzidkai.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3drugjnos.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bfzftflt.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gnchczis.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ednuanhj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qsijkrhj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oopjvyhn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hecjewjk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ymohnmvu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lupxrfqt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ouefqbga.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3szubaykz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wgewfzln.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntywjhkl.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mibflxud.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gprokysy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3clwbtxdd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3edffcghv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3shnjerie.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3edgssjly.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rsrveolp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3oavpezmd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rwmrdhgs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfjugtoh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3antdjgss.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iihonmtl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fpywrikn.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3erqodncf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gtgzuaqp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3hteuzttj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ptlgvvxj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrqncxpt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yunxpuuq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhpcdafh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ejbycact.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wegarkxv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nzcnmhdn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3vucjqrze.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zwelyakl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3dbggruuj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3igdcikzt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bhrgrtuf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rdpfhogj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dygbkwob.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3pcwraotz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3agunsnko.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3owayftsw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ddfqcpcy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3gqmejbbx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnovtubp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qiiqtqli.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwzsdzvp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jdzzwdgx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3qcdeafdy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ibylnpfk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3fnzadxko.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3rwqtngyy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wxhlykkf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwdiojev.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3cajksyhb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsiojxct.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwalyybz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3lyrpssrz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hanxwjoy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ejmmtrka.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3imyivzww.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3twfofymx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nxidchne.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3kbklwagc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3azrrhpms.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3pivyzidr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3btxbnhml.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qzsncqyl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3omyspijh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bumffqae.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3kcxlbnon.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uvvqxwft.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtenvshj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ochqtwgg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgrjmmwr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ryuhcptp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3npqyjppv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3zytjqxkx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3usilezze.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dhfzxzkv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zgurejcq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zavrybvp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjzevbbh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmwiwjgc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pmhdhrbw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3acbmbkfz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vtycqkzs.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gclcxzgj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3digefdok.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ghmubibj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zcwjubkc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3juyjnwxo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ynzjuxjg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3uhxyriwm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3yyduijcr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ipryopsh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3sxuzxwij.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3bgujcbvq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ykzkqtci.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3svxrvujm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3elkoejat.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3khftqbay.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3miufjlbs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3dwzjvwtu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3mbsazrkg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3czzzowtq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3epzqwjtk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3njgenzdz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3abrhwqnf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oijtzqca.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vgxtnseq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tvzagfqu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3aaitfjmu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jhnebcuh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3wfnvrkjm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3fnobltuf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3pscpwaea.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uwuuoacn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pvxmpwsm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3zrxkfkyy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3kdmyhdbk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xlxleyma.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yswytawh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsenflaz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ixgtefrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fayazojp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mhqbvjqe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qxoffzug.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3apococbb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijkpzssr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3eixliyew.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrwiemqu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qdglucxq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hxtemskg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3suvhzfwg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rqvojyno.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ibpaivvz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3midtifvt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3otyeiwtl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lybsqpbp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ibkxjqtz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3aibiusjm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3uyadbrns.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hudimbij.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tlkaijks.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3dhaowaxv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3godgfngd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3noldnilu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jskxlfbh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3txhmdwmk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3adexihxp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3gmxsvdns.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3blbhqxzg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3xdcgneqi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3dodxzeuq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxheruko.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3metfnxga.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gznrwsci.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbrufewv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3wtmvzqqc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3kvjywfgq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3dtqppmgf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3muwjthuf.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ldeqhwov.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3unzqicwg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jfnwqubz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yanofytj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3plnqgwqh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3kobyksdz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3wrwgjiwo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iiudbvbk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3wkomkarg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3dsqelhel.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kizihwdu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3aibfxsmk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3svcpiuuz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3lvqadntb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3qtypuhrh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3jwmyrjur.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3regwuebe.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3llxgcvuj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3heoigwhz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sabqvjrw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lkxxqmys.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vugsbokn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3bpxofibi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3yoswtgas.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3uwwmjucp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3guhubplq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3hnmblpvo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3vvsaoouv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3msnzhsjs.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ylmmnqwk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zmkljnmk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3itaoquwb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3qxgecydt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3zesvatub.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3qdjndqpr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3jfcdxkks.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3minauaqw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mwltrdiq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3wzfijhgp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3xubmxpvg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ndpmixhq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3hqdkizbi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3wxyujhgv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3gvickmlv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3qshxlcgc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3itfljcdi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ddwwpjwf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3spsstayv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ydjkoxgr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3nybrgkcm.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3iefotzac.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3jqaocopt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tktqkyfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nungkuvs.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mgbxmgxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ppwhoexw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ribuwxzd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3muxfobqe.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ehbwatks.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qaytwtpx.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fofmaekh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3wuzfwwlw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3zkprxorq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3najheljp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3yjoaiezb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lsxiwtvn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwekijeb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3oczqbjcu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3oujobcli.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hnnqrwdo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ogasnpta.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3kwchanfb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3euyprnzn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wimrqyxd.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3rwsodjgj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3doemdcve.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3zxreyujs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3bkrhoxti.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vgnmeyfo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qacqkjhu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3vzhrznba.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tdegjole.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3kilztkzg.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rsfdrevb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3duqmnspg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3otvhrtls.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fqfmqouv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3tyiajeeh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3apisfnlu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3yxmislpi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3abweugtn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3kzovebtq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sagljbxl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3zbmfsgkk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bxhncrph.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3exfvhfvw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3speabtle.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3xechefuf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ugcdsevp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ivptdjmj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3beqosvcz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3qkuyvdqk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ptkhtgdb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3esitxncq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3uxrtzosp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3djddzxkd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ordnogdx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3jhvtedqy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3wpciscar.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3besbwgcr.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3btmohers.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3jucwijfo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3uqhygkxi.html


<!-- 参考信息 -->