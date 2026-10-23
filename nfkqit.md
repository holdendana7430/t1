代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3jdurxaby.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mjvtcibp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3qjmroqgr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ukucwtfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rriljdvm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hhhbtmzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eshopojj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3kjpmshnt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xopphmlt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zjecygbc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3otathusi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3snjzhsyv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3itzsavbg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ehmbkjgq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3umsbvhqu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3husxklom.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wqyltfqv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3fdcvrnhc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ofidkruj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3whbuonkp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3oypfpzgy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3diywtrpx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kfriwdxy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cjwloxbb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gbkmohvf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qhdowkbk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jfyvbtsi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mtfkrksl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mufftkdo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3itydqsjs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wkifrtwk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3nvgdxpui.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tobmnkcj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bjpiazoh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wnqmovoe.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dacsltco.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttejwtdu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ymyypwdw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkwmadlk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3acskhnwn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3unteyawt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lhsvcclm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ywcrsmut.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ykpytgme.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dmvmgrwh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cwpbpqwj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rakjvmni.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ygfjaylc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ahlftdmj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3huwmwcqb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vivivhyh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3spzjlbsy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3yafztwya.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ukrfoctc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgkdsgbv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmxzmseb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aroxtkmj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfojgqff.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3yiteopmt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3wnnjxhlk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xamrcnrm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zicrpbbf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ngbxrnhv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3juonkyvf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vvuurjvp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pxiuhvdl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3paztbkfo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ljoqccsl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3adchgqdi.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tlnzoqhn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3zzllxrok.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rmjbgdrb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3zohwbrie.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3frzgxbll.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3hrogwynr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nowegwhm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ynbvgqja.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3siuszvwb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3wegoitks.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3uwkgwbsk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3jgpxuowv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3qjjstkyo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ryfnnxix.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3boyxypuq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jegpegek.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bydjvmhk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ekkycfyq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wglqtkvh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3tqdjjylw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qhtkqaxq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ugrfdczn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ycmhtwzt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qrysbtam.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3fpyqnyna.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fuyulukl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mpbkxvsi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fluonbsw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3wptotcou.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zermwdxj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3sytecqre.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bszbiygb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwvfbtai.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ckzywlcp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fwjuiwlu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wgnfifdq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ovmygbeu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eysowixg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lcuvphrs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgckyakb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xewglzvp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jutygflx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wqngiaya.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vpsdhbaa.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zimcwvlr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vsfangjt.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3swuifuja.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3jqrxzmgg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3optgncqh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qazsqsph.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nanarldh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vwkwjpzx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3sthgplef.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3pixjejkb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qllyyeza.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3oxznrehe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3vrvubixa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3znfeieqk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3crgypydu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3dgxgaqbj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdhajnxh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3yjdyfoyt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3kztzzcll.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nwavbjlz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3cxmvjjmh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nfixmjha.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3daikvirq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3aclmwvmr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3anfcnzmm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ykuktskm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lesxlzrh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ikzrlmzd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3svmtzxdg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3fwuvleeu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3flisekit.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3tugkqgmi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hkdgnpmh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ltioqsxd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3mmcgbpwv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vrtyvvvn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3beseomut.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zwnnclju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkkaxgwi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3yyjmyqkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mazjgdzl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3fqutmmyn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3aoolknwd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfvhgznv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lveqcyvo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvbrdvlf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3zxayolra.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lhiwotwo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3nysbrxrs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3esjbamnl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3jxedchwz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3fvvfwchx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3acypiszc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wfqovoba.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vitfioal.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eeiobdcl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tagprbyy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xjcgstpx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3slurxjll.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vcrrhpxq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3juxslmpi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3llvdncvz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hwkeaaom.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bpopywwh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cwlnjjtp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3lbzcocqu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3vbaovnrc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3japvxvbs.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3kyvqvggd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yzglslvf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ugtytfud.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dewerfzj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhdwkrbn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ziqiyjep.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3tjdhyjrq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zilihqct.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3gijjhxbi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jsgaiwpi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3zfrpfsox.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3pvtuwxku.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3litpwqgy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxagihsu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3zcncglty.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3neppwmhe.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wcrrahci.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxmvbque.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3fuwxespq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3vdzabisv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ybeoaqks.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zfgwcylz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hikxpfgw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mkmtrnjn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qejwngvd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3hdyxdfor.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3vubypxks.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3itafxyfa.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3zjtxqrye.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3akqibzyq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3govfwovn.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uckofhrt.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3poxaflxz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3qagpkcqg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3oxmfbocx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mkmymrfb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3kuprpmlu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3aohtyexc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3nfyasmzo.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3pwujocdr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jlauhlsd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3tdbodmkd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3lgxoaqog.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3rretaroy.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3yvdpiaoc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3pibllabm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3evqldjnf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3epczucxd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3rvgkmujj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3anmlohjl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3kkhdworl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ilgawgtb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xtretogf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3lopajmtm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3grkqxske.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3aenufqpc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3rsdxryjn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3gfatfdhi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3whaybquu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3effqvqfp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3lszrdrmi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3gpxptxyu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dqjknedn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3entcfnyy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3itxfhgpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzsllxnp.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3iknnscnv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ehdeodvr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qofumfcz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3itbpyzwj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqdtemcn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3tzxabnbs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3pboplosc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3iwnsbofc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3knplzjrm.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3lqyucmdf.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gsrrpesw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mcjfgzxv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3gdqxybnm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ionlscuf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jgnjhyfy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kxjnnpei.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kmzhubfq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rbfxfouo.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3gvxjdmsr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohgvrlux.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3tjccecom.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xpfhsvhq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ishquqxn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jgayoqwf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3cjbczteg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3etuiixdx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3tvvbqkmw.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ewjhwdyp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxobasor.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pddopspe.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3prlxmmgu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fbmnjgas.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dplufwro.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3glbbsjev.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3xdwszxtj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ynmrxgya.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3iyccdbgu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3dthnnpax.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3akdmtign.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3eiwivnmx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vqxsqpph.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3legmcgwc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ffrtplvz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fqclmzbz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3xefkjvbk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3cjsomfbi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3kzpordoj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3qiamiewj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3zbwsqrua.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3lajvahqh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3thmxcptl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3oeozkyfj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3nvxxhdor.html


<!-- 参考信息 -->