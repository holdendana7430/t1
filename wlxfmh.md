代发 wailian999

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kuemjxdl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3dqdgunle.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shphwxcj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fgzradqi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3cnwpmlji.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxxhokmw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3khxktwsm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cpcjvnte.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfmgxlxn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hzccjuwb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bvaffrzn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ptefwcmp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3llinsdhp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xxahgxxe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3stclsxoy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xptbteij.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pnxmwqev.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oufuizag.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xhcbjnlk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zysggduf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpbfmtuf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ylrebxnr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lfxgrbhv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gpsikqqf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hhirbxru.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pankfepg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jzoozshx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3qjxrylyo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ardnloyl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ypucvvsy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oynpmufj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jujisrvs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hmdsdkky.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3quqwezum.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zkpriemh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3vmamaaxf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3dkysqmbg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3wonxzqip.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3docqeycw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlbxpwvz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jsanquan.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdxziuhl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wfqpjnxj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3wyfftcnb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3tchaaohv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3nfjogvvt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3huvibztz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3lqvloatg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sdqeyboq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dvsiwdwu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3incmygsn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jilsznat.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lfubsqxw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xfszejko.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3tqnaazxj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3mnkezgsi.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvjykuiy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjpaaifo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3msamedto.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzzrgebs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3fqzqoyrt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3tvpnemya.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3tnpolbyp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3nytmfbtb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3kerxvuzg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kjjzyqmh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3qtkisbwp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ofozpqig.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3quneuyob.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3efximojh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3enscqtxa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezmsijrx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3pkdrelyx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3izxsidkx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qaeslgpi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ypneumlt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bomkxhch.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3xmzjwyqe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kbuqyxot.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rwvogmis.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3yagqeczm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3vcctwaap.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gjgomyjd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rhyiudvc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgqtjgda.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3iqzgumut.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3prftpmps.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tebxxowd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cfcfousf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3emyvmsom.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kqifjfnn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ghfgktae.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwkxlmdf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3duafexlp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdwqfcem.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jsguynqo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nfnkdhch.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jtakczso.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oanweryy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gnpxoykd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3amaatopc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lhesuwug.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vktrjfrh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gqauygrg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jfdhribn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qmniuwig.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vwfnpmve.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ewiygmgp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fszciewg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3oyvgxyhl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3lfaqpszk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mpxgirod.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3twklhtlj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkerghbe.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qkfebxff.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3nzkekyhs.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3zpdhipsv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ixmdayds.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rdzcmrex.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kltizguv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zknayicb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ldufhreh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3lyaevpyu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lqwehzxx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3roztzjhf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ynqmdwad.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3uggskkrn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3knsxmlcj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3knfuibfn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tkicxpva.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bedbbevv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3puiefdel.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3dtmslzlr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dftkyqxt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dkhorwoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qlavxbhc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3cogdxmqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stxtocyw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3kyzvufsu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ubwhhvsz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlkyofqn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3axaiguup.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ojswuvqo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3zixslyta.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ogbfqybn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ivkuqzye.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qpzwujse.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3bumvzlvf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3dkmdmern.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycbforhw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tfvsmpth.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyrkktcg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mvsebemw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3gmgmrsux.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3aazkekrd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3brmbbvsn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hbyjtpab.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3qstmoaqg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3twxqrlbw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dwyiqguy.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lizwtbet.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3makzvpcq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3kiygmgax.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3nslsfjbc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zrnkuiuq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3hwyynczo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3iabzyand.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3iwxudhme.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vivgcxru.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qathjhan.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nzdxlesq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ufogncfj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3sjhgwkly.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3szjhbhop.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3jwialkql.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3lzdmplsg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3mrwaafrd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szosfvgf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ykqydakb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jegufjhg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zokwzlvq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3rbtxsdgv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3thxuhbds.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3tmdhzzff.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3crdsjprx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uvdgeosz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qezabvlk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3bjbaihxd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3rpoapeuc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3cpljhtal.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3dxlbimec.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3uqdjcrfx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3hsitoskr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3duxsclkb.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pqcmcjth.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sjxgvppe.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kloabqrt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3pcixoijo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3xkflveun.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3zmmzmrxp.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nhgucltk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3odvyyzmp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3lhlxsksy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ldbzpkls.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3gdyhndku.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3epizjvsf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3hmtukyko.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3lcfjpcky.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3wfynisuz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3twqcadnq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ggnvoylr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ntzhtmno.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pbbmmzxu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3eukkopvq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3psehqxmh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3zgeqfxac.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3vmuqjoip.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zawqguqh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3vklfiljf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3puusgrem.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3lujbjtqv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3vvbtxeuh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ojffyadq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jkrqidku.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ohxrfoqg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3txhubfty.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3sloztauk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vlltcebx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itjebaol.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rzukdkwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pcdevnew.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3iinddriy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pafvxciv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mdqbibcf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrzenwru.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xuxftmbh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3cypmpgep.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3phxgmewk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ydhshbdi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pwovgroe.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aeuvqqqd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbwneqqo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jxbgkdsg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3ztnisros.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3evhyhava.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nejcxtej.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3emismwva.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3smajmgtj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xyabqjeh.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3zlwsyfzy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3wmbwqjrj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3avvornow.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vedgaejt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3opqqoncp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ntnxxirb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3kwplewnr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oqisyaiq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3kxwjrwwi.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3adzyclrl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3rrtbiobw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jwxqixdf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vsqhlfck.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zvzmsfae.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3aqhoroip.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iiodelhr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3mhmwojsr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3jrcsbzkv.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3omodbccz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pzjynonj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3loxtuhrz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3mpxsibjg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jhjwteob.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3afdawgoi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3dpnjkamq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tceifsmm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ugaisnlz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3phahuxop.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rmnnqgts.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3xpilzhrc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3guofcajy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3pynoorrq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dcvhpsap.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3zrxyylgh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3klivvgpu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3teulzpae.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3vdvmbtvb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ocepgirl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3quseptcp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3noddyify.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ukbisfyf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3reaxozcv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3qzllvfxq.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3zsxugtgw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3hbwvmqgd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3sywcfffm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3bavpekkd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3amgeuzih.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ghxpphvq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zhvfpyuf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3wctvikvi.html


<!-- 参考信息 -->