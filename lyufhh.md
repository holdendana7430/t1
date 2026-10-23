代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3qzvjcesz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3scttjnig.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zwijzwzd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3tihhjghk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3awxwlbym.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3pfbolfvb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rzuwepmr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3iwxweduo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dgmqkepd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3rmsgiyzn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3eqgdjzlf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rumilhuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svqscfwg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3cffkkptm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywpowlqv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ayudowih.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bookgbub.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3bwfxluhj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uaxxnpcb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3oynyrcvp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rslvfzzx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fdxomtfj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mbotpxok.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jisenblj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uayknjfz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3vqgsimvq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qecritim.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3stdchkis.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3xddrhwbt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bbcvbwtg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tzsdvqal.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yevtlhwi.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3orosthae.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3brczdqge.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ftfvuxqu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wtdvogku.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yzhqmiag.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lfcgpimz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ikxnthwe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pxkplliy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ribglwra.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3oatamnpg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3bsdnrumj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3eydjytgp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vijynzly.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tlhoabnv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dreyfgdc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgsyaprx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cnjkungt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vuaiyeya.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oafaxgyh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3qluyrrui.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wxdiqnlx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbowrmes.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hoyofiqc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oihggvjf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oetngdvp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3zvjgomzc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3udnyusyr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bnzcyvzu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ioeiwntb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gbyrggzf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3efmapdwp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3chcofjgi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hivlfswo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovckeydy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3bfaudxvo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ewzmhinx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3landebwq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vxnbqqaq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nsgftwvi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xlqvmxlo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ybxbksih.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rzudmlag.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vpqprfph.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3csyfxnad.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fsisbept.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3krskhqre.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3aprouuij.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3siyxgdqa.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3awksveqw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3abvrdfoa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbmrvhld.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qlznmxxf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3wlyonlit.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3diibjnyx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3uonlpmeh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3rdcflqwk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3kxihxtqd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3inugutob.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3frbyrams.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3qohtpzqz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3aljvgcok.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nwmwmjtq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fkphjblo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ncrwiwff.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fvyasbit.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xglajsay.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vqhlsooa.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3plfozdjs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3snllrkcr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3bvjhgcoq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vnnepotq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3njxdlbmv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3udiowixb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3uydgiihs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zvqpuvar.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngsfydua.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fgvgdiso.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wbqlvoxh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffemlnlq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ygyohvzp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3vogyxtwy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoajmxbv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qlelwdja.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3upjligro.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kvivzebn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3llwpflxs.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghqldocw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rjgjcgzn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3utekdiql.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3laehfbwh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ekybskkl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vjxsbgbd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3yelhwhmq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rynixcxz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3whxvfzoh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3haypwymq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ttqexlao.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3gzhrmksx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rsqnblea.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3dzlgiukq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3cvdpislf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3mtmkrnri.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3zjcasgwr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3nytnqhsj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3tnavnnjl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3skmvyfdw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ibjgkxmw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3xhbgwlvk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3eplknkjg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3vmhcnzck.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tfgmurap.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3wveauvrv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ukhljpxk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mvkqeumr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3lmwmecjr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3veticcvm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3svbkeaja.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ypjofyvi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3abaansyz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ecsivhgw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3fxyjnvqg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qyxgsrdi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jafmxcer.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3idkophhr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3egbsgsuo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3skklbozg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3darfntjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ryujtdmp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3mwnvydol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqfqealk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3eiajeodv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mgtjzjof.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3plstcvuh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ejempjoj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3odxgvdjg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pjvfdgbn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vmeokiif.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3xzfolhrp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3rowsjfvw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3yuuetubz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3lrxuumrf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jorbuqtw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3llvsclov.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jjcsxybn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxbfauly.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ervwkxzm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3cipngsod.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbfxjfia.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jpjcokfv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3edeeleet.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lkosjtlb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qwazeher.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3myrjppuu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kduhlayd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rkctztgw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ipeareqf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3domomals.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3vlxplqak.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3sqrcixkl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3stdqfwjt.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3anzscbux.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pqbofaeq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3eplitcff.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3uutolwnq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3zwwqwque.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3tnsqjxxo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3hcmfrkjr.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ymhmdsal.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3lrlumsij.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xkgmgsoj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oouqcqjp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3sesgaocf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3pnodatsn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3anzskish.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzwpgkjs.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3lrakpmed.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3lvqbgchb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sotzpogn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rtzbnlxp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3wdmeqvnk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3hvkodlio.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3lpljfigv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ytkcolaz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mtygieup.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3djabqqnw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3eenqylgl.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3euaehaig.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rountyqo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uovryxjt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3tasvzrwn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ubtththw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3bkuhrmmg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jfcgizin.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3jmjxobos.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ebiutbch.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3eftulczd.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3kzhodfbn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ypiatval.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3pxyzcqmk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3uqrkinwj.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3qrqbuiug.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3cqrqpfjw.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3tzzeirvr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3lfosezgk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3kbkgplwu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3nuijezmf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3nlqbclzb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dsnmzhwp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3jnxzgjzp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3bryithhb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3aesschie.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ujqccmuh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3fakyfpyn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3mrroqthn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3roduhthh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ofgulsri.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3fspoyekh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3dkdvjngh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3kfblzdkt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eavrbvew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxoznbdi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3jlzxfbwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilncweqx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bmiwodld.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3htepwnaa.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wkxecrss.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3oqlngpmt.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3wbjzitbl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3uazgxkat.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vaiwxwth.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ydnsqomu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ouzbglrx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3etfhaome.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bgmptkxe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3jfswggyp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3xsozqaeo.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3arfkpnan.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vezsbfnh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3lcspqghf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3dlgqhlmv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nozhqdkj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ryfozvan.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3bcfzucuf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3mwbtpbwk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iwkbtlfp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3hpllzfqm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3cdougjhs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3rkxeehsm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3frpibdbw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3gbhhkjwp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3avowubno.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nqeuarng.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zczzzmrj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3givaokkm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3yrslynab.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3hhiryikz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3xlfmxwes.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zchzhlzb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rhyaohzy.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fminlzwl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jpohrefk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cuayoclm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3piyjvfiz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3waiyfoqa.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3fuxadwqg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fpfhkvqi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3zaeluhuh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3cerskjay.html


<!-- 参考信息 -->