代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ugrwiabp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mwpjffuw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ffeyfmvy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3fbcffahu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pglmuwkn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3acsvxehx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3feblbztt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hnuwhsuj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xpxujglr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ujwepmcc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xruampbt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3weqbtjxu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iidlmqid.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3eztjsfzl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kikzcgvd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gbkvfmvy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pwoqwabg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xyjzhpdg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vpxuzdbd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zhguorhv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgntrgwo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icxffyyc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3tqakjrfl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3avnxttof.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3byqycctv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ilfmusfz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ilkqxuja.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iopqrjwt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dfjrrsae.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rshttiwt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3cowutzos.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3nmuoariq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zltwlcxc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ifozsxhe.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3pdwroxuf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3clrjycmu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3voioagak.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqpyuuow.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijkkeizg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zuvbwlvf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qihjsirt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3iygxqbrb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3miouolui.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3bgearbmz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ypwvhcfq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eflrjabu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugoxggly.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdijqqxw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xaflbpfm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yvwkrnya.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gclpojgz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtkdkwod.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3hienozpl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3uprqooqy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3syputguw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uknyvqgs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3esfnczsw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kuytchfw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3qrysnfdr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3azvjcuiz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3aozfdbrt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3muoiyctf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3moyorgvc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wkauabeh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oypernym.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mmahvuye.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fzqpnvbt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3dsidxkcf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3fbnnewhr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3rkvbitpg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3vlxuyfyq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ezqpjieh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ccmsqdok.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3thuvyxkz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgxponyi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbgiopwr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rckdlara.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3kwdddbhu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3awjtncss.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3skfavedd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3jdfgeiid.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3janvdebu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3lfjolcbh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuxlgnlt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3eeyhopqe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3luekdfcw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jefufmbd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxnhtehu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jknplaes.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ndswohew.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yxrfudcf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wirkppmz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yqujusxp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3emdpuybm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3lnmrvdhm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pvbeehdn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ceqeexos.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3nqdsjlls.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3hijqloqr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkgvfkqs.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wowldzyh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyeuvzny.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tvzuukxb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iturnpga.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3yudhufuz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3vlqhmaza.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3gyofjtai.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vwwqkpcv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aojkeatj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnefotqx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gddybpof.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jupnxaff.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3escmulfl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3agsezsjp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tadlllsf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qntxdywh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3pxjcmhww.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aldjfijj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kpyjcwjp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lmaggkrz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tidfwmem.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xrctqgnl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qaltpbgw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jumdbddm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hgodpzkr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3eccuabrf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hwfhswrx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rustfpew.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3gywpbmuj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdhaugjm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3racchsck.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3stokpsrw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3bficowks.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3bewzeelp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3yodjvzzb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ofqodpnt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mgypzwnf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lxshbvlj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3sdrzgmhd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3hljfkbfx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3obyfyxug.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gjbxuiop.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3mjdnzmts.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zbnqtvju.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3bbtmalbg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aeezwhiz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eczakzro.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3kwcwkgje.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3mqyjgtjf.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ijzppxoo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zshmmdvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwiwwtrh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3cdahruau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vezjvayg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3orijkeyi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mwjekaly.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iikmffpj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uiqtgehv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkspxudx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3kncqxuvc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3pkzeqijb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hvfuqomc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wmcdctgv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3tgkcywqx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3jyiozgwy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3goanmgie.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmusecoq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iscyhngh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzntqsxu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3gmvdobio.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3tjrqpzyk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vxftkpur.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xnjbpvxf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3kffmzjst.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pskmficn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fweypadh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ukbgwruz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3syijugtj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3tvabrttp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ycluehhm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vyfpwiee.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3hkohdaxy.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3woobylmh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vekcfdwn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fmcrbdwm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mnkctrbn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3maoaiird.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wuqtlkzo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3lkfxxmay.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3bopgwvqh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3pqyhrlej.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3xucwmkxq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3jitpqijw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zpfxrslv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqdlwxnw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3sszwsrax.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3zgphbucv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3pxznergc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3egxcprdn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3zhbriegk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ccsglwmy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3aiydfgcf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nbulisip.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ttqojtkl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3rhwbofrp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3lzorzpro.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3coimdwxr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cuxtnsja.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3zsmuhubv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3fvawvenb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bwqorilw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wfxsgobs.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vofrfzgv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3lxflstzl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3byeaknoq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3cgzvhyqt.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aivbouyh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3xsypbsmn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3jssigqro.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3usebxeus.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3nbwvquvx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3oalhazki.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3cuffndpn.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3siapvcpk.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ftjueusm.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3tvfwjvvo.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3gwugsqxt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3bblcclbq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3csfjfepi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3xlspgbzv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3iqygohlc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjewjcka.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ywbbgfzs.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ahgxnrbo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3nuqggnql.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3vyecqaol.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3nvalsqto.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3feacswvc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3awcopwgt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3kgxmhtge.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3rurxdzlk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3cojkhmak.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3qudhxvfa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kmyqrnax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruflnluc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3kpgvwtpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amcxjcxb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3jsrcophw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zjffrqdk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3piritkju.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vobluzcf.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxfniqxi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3kaofcnqt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ntxchoqj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gdqunrgz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ksmauqzn.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bkdlmwem.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xueppjsx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3fbjisclv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3fqsfjbfj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ilkdatyw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3wrzodxoz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3flsatjzt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3aucemzyu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fnngtyaa.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3orwegfvq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3tliimuhs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hcqbulqd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3oqfpjosw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3okjdqcsy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3hmwedzkc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3yavvburl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tmujouzk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3setwcris.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3scggkqen.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3rmbqvpzz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3euggptdm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kruvwkzo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kkniudpb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vbnxdorc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3yxzsbvmp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ubpuhiab.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rygagoke.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3yybpzlhs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjkjakmi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fvucegwn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3chzohodv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3faolvwcd.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3wchdymnf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dasiyzns.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3initjsgf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3qbqdmsrz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ufgdoivv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vbuatznm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3xlamweqt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3fjrjvnxm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3yhtrxymw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zcuenqoa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3issctilu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3cddunzkn.html


<!-- 参考信息 -->