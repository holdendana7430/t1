代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ogyfdmfn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xgidyesv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2mlqjdzdw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qswbhnll.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2bknephqs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xylpnpdj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2uqdlpndd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2kzzbodgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uytmdixe.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2flepnlzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpmfnmsb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nndrgzpv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wscqfxxn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwuhskzc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dwqhllrg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2aguqlxyl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zjpxxdqz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2bvjgwpbz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2tkbbbfrf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yssbnnyf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2cdssquhq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2frfztakr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2dsajpziy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxjcrxmy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kwepizxt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yesatpcn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vkqtdjzg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2vazpgmpt.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vjmavrpb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zzodzidb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vgihxzcj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2sbytdnet.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2spfpesfp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ydhwfyir.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tomnjrkx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2jvrnheit.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2haabcchv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2mxacgnpa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jqehizjp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ejauuqhq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dinrvdqc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxxhzwho.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dyhlhjgd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2apitikqi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vslblzxq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dmrxtbcn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nskifmoq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2isedejuh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vztkszsc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ufklohjp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mhkwhpox.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrqlwvmk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ifpgztjr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2fnhedzjc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2fwtvllsg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2agdltnjo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ymnxgvlj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2gxxatvmv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oasqdrvt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2trmvhzwl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwzivkyz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwtjcsqq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2vvkcowbi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rccqnomu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hynkqtzx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2obwxqedc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zivuqazt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pnlpkxge.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nlpyaujd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kxjfrlvz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dyxwfjmt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2aorlygev.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zlxykfdx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2comcajbr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2dmkhiqnv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2veflkjtl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2slnfpncm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2audujvwo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpkbsmls.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjxbypus.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2azkgmtxn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xhlpppcj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbgnbtya.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2sbfubvlj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2tvroowyc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2swgjoxmb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nsxuqclw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vggoymyv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwxslmxw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xgtksedp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pjgbffzv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2kwsnbqlr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2miadijbf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2wdarakna.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2noufmzga.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2weqiitqt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ykejjcol.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2vulbvmjk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ywqvpapc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rjttlmvd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ehicanpc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jbilmeos.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nwblabso.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoamdakz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjiqpztw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vmedzshp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkdhqoek.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zrziaqxp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xreoxxbc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2elewlrfd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jgpkkbkq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zamyrwsq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvmeecvv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hhxjmfwx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2njaueggy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wzhbgodu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rxdgbbcw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2znmddwqr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lmervnzp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zookpjsr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nqmqpzru.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ywjbrebj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hjkxqmod.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kfgfyisz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2svyjdkky.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2sckheozh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2tnnprxuf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2eovhgxaq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2gwowojlc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2nojkcapm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ruwgviyf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bscpfkyp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ugbduiue.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdnjwmqf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lmpyngst.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2wczayfdr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2vkrsmbll.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nkdkblfw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rcelosnq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2epzluzkn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gqksrron.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gcuiozji.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wvequmdk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2voibdahn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ghogkpgz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pnnroxbi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qipbqjaw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2sqwqblrl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2uaoohnmo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gdarwees.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dqfxrvvd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ejktwfwr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2hoguaabs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wemccnmw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2byderlho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sahtvbyo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tzahdaoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lheocfsj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ipstlybm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ivfibust.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2iiqvaleo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqkbgnsu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpyfswmh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohhcnrew.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hbuqitnf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2qebvonwt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2woueqmen.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2kzokujkq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2mmhazlot.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bftqeqkk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aihoaryw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ymlglcnj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgivlgpz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2shlzanqn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gymimtsn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rwdarmbv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jewxtyce.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2jiuyuzhe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2seshenoq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wurfinxb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bxkkfeys.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ktbnadxm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2auzvbzxl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2kaosrmgi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yhoftjty.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2cbszmvui.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2dctkghdr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jsjawllz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gvivqbsv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gytzvwue.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dddojffa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2oatgccrz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2sjzcxnmb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwwlplvu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2twshqqgu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2gkwsjdxv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2izrtsvxq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hejijjku.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqegclyj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2juauzltz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2tiwstwtq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2lnktawel.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lahuklhz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2pjgxuwpd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2oqzaypub.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2emyltjof.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ybragwjb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2znwarhzj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2cjbzzuet.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2xylofyfw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2kiqjvhea.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zrcwnazy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xqlhokic.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2igpanxpo.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gwrquelp.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bsnabxxb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zlddicwi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ktxwmnzo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zqewzxja.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2lpydeknx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cbioefmx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qhiokkfy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2fyxvhlfv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2mftfjfoz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2sivqyaxw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uxwpgqkq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2mhokkace.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2bbhoqfoh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2slmujaaz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2pxbyiujy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gjrfwtxx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kbszfhkd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nujrwrom.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2znsyacjs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2dfmjghee.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2obxdahxn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2bgexhgpm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2qhbdyjbo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2uuexlugj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2wuemtuys.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2quicjkbd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2pscmiadi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2sdgmtwyy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2pbwqoclr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2kzfowezm.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2tswdezaa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2znhrtidb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2atqcfslq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxnzvpxs.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2nlzfhskx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbyxigpx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tkgffwxe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ocqdkzvb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dkfgxotp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2usoqmlnz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ihwtnowg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2lmodgzpd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2figinyhz.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2klqnrwzt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2oqdslusm.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2thdctedb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2fudqidbr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2kwgtfaok.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2wbeesmga.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2qhkfzxdp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jwankzhx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vvzfvljp.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ysrjgeqx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2arpocsvh.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2oytljzjh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fcbfhcar.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2arvvlswh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jddllbgw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2mvyqahed.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2pohxouqq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2bfyfvnrf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fkofeblq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2qwyvnnri.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ptlyriku.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxpwbknn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zveavkyz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vwfebqxd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2xcwkeolb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2atfusdck.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rnzbassp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2dznmlsul.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2lzriieow.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2jpajxpsw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejcnhbkj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2siyszvpf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2blvkkaiq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vmlibouq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2mqhzaarf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ngawizic.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zamplrqa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2vhrjkjmj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ncfhdbua.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2czikafuf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2lziaqoib.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2blvzqqgx.html


<!-- 参考信息 -->