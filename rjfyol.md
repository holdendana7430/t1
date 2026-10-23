代发 wailian999

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3whjbsodc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3wtyuryva.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xyomhvpw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljldddyr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ysztscqf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xcblnxsz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tzuxmmxo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pofukdyw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3repfkanv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3teeydpvf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mgzgervz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3kbjonscz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qdfrxizs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3dqnmuonj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3catzoshe.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mqrohsaa.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mixnguzy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lpeqsdct.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wxykryja.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3pizeqcwb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gqggwvka.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fajhfmcl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hrwxqwoo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xiyctypb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejbjwrwv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ulmtraou.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcbefxfb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohibkbak.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qwdiqmpv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wcfynjgu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nwospsqa.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3bhechioh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3aeomvquy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqdkwisq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aeiwtwee.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yuibbyvx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ssextwww.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3docachda.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tbuyujwi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3whqcqrvc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hmhejcza.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xrqcfkzr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuinptbc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqfpwtpx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjbsshgb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3euzbolyu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ghipskow.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ugfffcng.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3dsiircao.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rzvadpoa.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vcnhtcon.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3xjvbygga.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mfigpdzh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tkxyhxuy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3chmnvopt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rowardvu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3yjnpncmb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gscdbrrk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ivgdtpqb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3nrbdsqty.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhrcjnzn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qjpwggkl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3hovbbozc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwohhuun.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vwuzfnkh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3rnpmryax.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kquymoeq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3hzxrnvfy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3irpqbnuz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpvfifkf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3oushhzzx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3bnwerapw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhgouxlw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3zeavcswd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hrieurjk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hogjilbi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ttuebyra.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3yrpzlcxr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gowexlhh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xgcgowru.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dxusshhd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vluvzgxk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3gbbnixzc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3egvdfytn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3iiahezrw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3tnyxkgek.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nkcduvss.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hvmthcpl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3thxxlbph.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rywvhtfl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bcxzwxqf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hiwpirqp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gunblzgw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jwfkxadv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ebdtlsse.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nhwlgqji.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxfmfggo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysnjczwp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnojhjgm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cppmkrhm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fuufdprd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3phldwcxl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3orzjnhdj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cuazllma.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fopqvvhj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yvfpdkwv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sgxujrwy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3isbzrolr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zisfefsw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3onznimhv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ustdizwy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3pkrgrpdc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3uxizysal.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3yspvvzpz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3grsmosao.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qitoahkh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rdattovx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3pbngwjtf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3emjppmvd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wjgjlmqf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3irprjgpk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3plajlcte.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3nrtmmgjh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3qrjqaxrm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3yohrpxpb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pgjblizg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3yfwoadeh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3smhpplfh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rkozxwlz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nhljeiam.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3irzzicxx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3kfuehmfu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ggwirbhs.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vsgwdwjo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zmwltnfi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3nasnmyde.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3egmbfvxe.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3igborirf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xufpcylo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkwjwplf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xvwozcks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olmqpuwa.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wrtixtnv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3fvvjfgxy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlfwumsr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3npclquxv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3idnbyfiu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xipceiol.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3eflaeiuk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3mhufhqlw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wzuwykkb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3rujqpflw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ceimtvvc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxzqizaq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wudefhny.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hlzhgxqz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fijjfefs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3zrtisfnm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3esyhogmr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3owozwkvy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lsldpkkq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3viqryijs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hudwbiqq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xjfskxih.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nsplopmr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qprsbons.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3fskmeeun.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3rpwjtzdu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hzymgqkv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3lwmgrqng.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3svcammbd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcosbxyt.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wsduhowv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3eeprwyyi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jfjvmjra.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3rvyqwwol.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3suxzjcvq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3uomxsvag.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3vjxoubkf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wnrwcesl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3quxeieaq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3seqjrfqj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ynongltv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3jantvwwr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3eiljexpg.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3bsrjravx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hgzvaytj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3axztpjqk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3boeexsrs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rdzaqyir.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uaijpppw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qqhgrvtj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3cywoysla.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3uzubglaq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3dcvtkhjf.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3doezqseo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3jlddgoct.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3qanjimdw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ccjgsowu.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ucyualxr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3smpynxju.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3hyynvgvr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3xtgqvtxx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3enkxvtgr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kqhhijqw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3nmnzpjic.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3udhxgmkp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3kvtawhbp.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3vitjslxk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zrkgllla.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3jydrczqm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3pkrgbikx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3tzswyqog.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ulujqbvc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3szydxpqz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3jjmlcadz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3gjoezqxw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3twvgwcvm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3qpwzoufw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3wtdysvao.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pwcigsgx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3nggiqxph.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3vrgkrvst.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3tsnqbdko.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3gmfevpjd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3zmtigbmx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3sqwcerjp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3nsusbxnh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3vtrvfzqw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3hwpddabd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3roksmaju.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gzgfjtzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkkvjlgi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3koutippc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fupeneqk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cbsrxvao.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kedjydrx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lseawjpd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xbqlbhbt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqdwszga.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3jrgumjgq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3tiwferrb.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fypqxmvm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3iackpzse.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3iucetuhg.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3szksdmcn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3elhahubi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3gvfjmjys.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rimrzqru.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3sgqhtwjy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jlbfswmx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3psfjetxc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hxsqettp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ytdcwizv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ahfmxmik.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3itaiqwfs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3umrhadeg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3uczfizyd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3udqqqfwa.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3wlxxommz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ufzhbilr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3gjobjiyk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xjbrfftu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3atezofqt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lyqjlyox.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3crjpxhuy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3razumzww.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3omplncla.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3uqtnregk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yugntkzv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jbuvghvp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3frurbjev.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3trszwmuz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3whzsxgzr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3pwjakgdo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jpatngnr.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3lanxkhot.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3pfjxxmdl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nohyesgx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3kkcqicnp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3tquxsdvh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3icgkftqk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3xbatkwbx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3yqmdgkkq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3nmrrkrkn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bxoykjqe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3qihyektd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ckpikgqn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sxbedihd.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ipowqcys.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3ddsxvljn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bkxrryac.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3faqaoxvt.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3rhconhnh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3yynfxxdr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3krhkctlg.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ksvaatts.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3tbpaynzz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3eugwmgkq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3feigfyeb.html


<!-- 参考信息 -->