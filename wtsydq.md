代发 wailian999

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3afdegnho.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gwqjsobl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zutpnrdn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qvvsrymc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kvlyfxss.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3imectcfm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3gfrwddpd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3azvcwmwa.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ynbbxedx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3slvemhbu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tedhtqoc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3binepinn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gvviscug.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ftuafayd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3scwbuucd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3skzqybmt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ndwpeyta.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jkchxatl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3sgxgbcij.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qqkfbafo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aovdtzlm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrxkixtp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkhleijq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tieitlzl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tucnsdws.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bmmejrpr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ubtreodd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3typiilqe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ietetqnd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnhaatmq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jiffkjyu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpawlmbh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3abbsfknp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3dejmqzfe.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zgywlmdh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydhwnhep.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3mvgcvebx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3aftpsyky.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3untfxbxv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtifoemc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oalhdxhn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwnzsabg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3mjdoltdn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rgrhywqs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qnkszjyo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gqzxrlah.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ypipqvba.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3iucnywkv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mihlrhng.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3afuaxpsw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sgdisurn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qwobaixw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vcnbntkx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3kddnxlky.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rgpgijxv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hmvdaafj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3hngpotzt.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3dqrudfgg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wudyyuez.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hqoanvxy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qhzybcut.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3rgarttdi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gycctjvr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3skkoiwep.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ehzazajw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzcifvjw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3uctkrgui.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3iccetcsj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3cgoaromb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rwtwddvx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pxrnfium.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3rsncjsjc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yssqxfml.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xyeivrmw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ohpftpnq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3wvwuhzvy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fgbbhvdu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3apnrparj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lrqomvzn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3softydfk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3twiahakj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3meecnmgz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wqxikulj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3csbytssj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyrlchsh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkmnygmn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqkhboei.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gwvainvt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3gwhwidnb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xkrrqxbv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3phtxdsqr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3smzxwtpr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxseuyqp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hejuvfab.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ovroglxh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bwrmqbif.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jzsauxng.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tssymyjw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vxfovaox.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3mbofofuf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3jpnrpcae.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nfjgqniz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hemcqoef.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zgivowzi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oibyxxna.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3shotejho.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3diinhgoj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qxmzrzsg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vtcozcjt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xygcxpgh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qhcubhuv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3izpaqyqp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3xkvihddd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3tgknfuxt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3rhzvhvcq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hsjzmkwq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3cyzxvmxq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qkwohedn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kjcitrml.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mytqtgyy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ezuzhcyf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tedhbezv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3cklgylme.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3xxfqtjdu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3cekauviq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3abdayjuz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bszrelkv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3udzpblrl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ynisvgsn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kbwzbwax.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hdohzkpr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3juppnejf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3clyfpjlv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3lollvewa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pynbiilg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lphlemqe.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zdigrdrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3igfvlwca.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3rnhhhqtq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dyacbbnf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3bfefygta.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uzghlhth.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhfxkqcm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ytvblkwl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nediwjwo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3bvseaccv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhimbjpk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3lffragzm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3wuammhta.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsubukds.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ubtxwxuk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bhbkdler.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbwdasvl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3medxuytf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3dsugoyjr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kgbukcwy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rjgniqgh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3edoazqjs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3frlttazc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vuswnjhh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xpjxipia.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3deedzflb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3obotmnvg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qvckyqvp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qlxnioal.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zjhpxljo.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3npurulzg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lytjrupa.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jnjvbwaq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qznjdbpp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mtbnlkiu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3avbtjnkz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3lbjhmbsh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3upjkprtc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ehmsnyoo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3sqplxzwc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3nrpuhzvu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3esijkcru.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlgmhdbn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrombteb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cziqdfug.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3jdcjwuwl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3lkqupdgo.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3dhecljhn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3rllcpytg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cfajoejp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3khullqxn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iaafkatg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3krqwonbs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3heiexywk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ibpspnpi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ftfxnhiv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3rnfjizcw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3rilmwugj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mlgnobkt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ktigtwol.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3flgzsbwb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3dwxospaw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3oxujabat.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3mjkhobqq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zfrcjtak.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3junczvro.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ptpsifjb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qfekgugz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ssaiqnag.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3btpzwdth.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3fhqxrygl.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3snseqycd.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3pnrhftyp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3frypmcsr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3nlqzghsl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ahwxnwgh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3qercvrme.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3sfuqohqj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3rwhwvwdx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxjokuwl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3noylatvy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3vucmkweq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3eeskznwz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3oghchdvc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3tphdsuah.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3qmihckrd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ntjjeixe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ljglpunl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3pgabbmvy.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3kgavrcuh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ryskqtzb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qmjigjpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnunqtng.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3owpojppu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pjtlkjmb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vwqnbaev.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3azezqmlx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vrrlwlje.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sifjnhyv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kxqcnxay.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3lwisyfyt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ewkluets.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3vllhowwp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3kxamqafx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mvfhqhgr.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qfckzuht.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3bredmtdt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3eoekpfct.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ltyupoas.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ihgecizt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3soaldqtb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ioaguacj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ygtpvwen.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3wwbmpuwn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3tosisyzd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jswaaogh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dhkxrjav.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3fznxphhf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mcomjdsx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ppmmpbec.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3tbhkppbz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3wpmjoiwk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xmqjsqor.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3vwldwhlt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3smdobazi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3pounwpyq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3obubpevt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bnwposxq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3bfoubvsp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3orxhsrdc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qmoolztd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3nszwbwma.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3runglrpk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hqnlxvea.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3zwabdauq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3csopnkxq.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xfazgcbd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hfknufes.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3rlerwvci.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wgfusbbp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ualbpjov.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dveanbyg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3gdqeuere.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3auoqvbcm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3yyimadxw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rydxnrqn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3lxroidej.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3quzjejqv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xoccxmuz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3skznkpea.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3daogohal.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ylmductb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3edzijkdv.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3wdovjcso.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3napvhuzu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3bkumzkwy.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3sxccdxln.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3gcysgmqg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ykziewng.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3eebqsvoi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3nnpjntka.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hhuejqyp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ydsbwqln.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3atysooll.html


<!-- 参考信息 -->