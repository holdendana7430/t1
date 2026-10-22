代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ciuyorgz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jamtqggw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqboveme.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vsefgdfa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2sgqymdkc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjdcdiwc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ilhhqmvd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2plyvlyly.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ueqknldp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2yzpzrfst.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ovqpbffd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2weplvyjj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qgvobmuk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2oclcpers.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lgdypnrv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hakkosfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knqwjfdk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ofpoqjtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2forojqsv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2crplogfp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2yyqwbjag.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2hwkxdncj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywjcoudp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bcaeanui.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zqmrmpbo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tqdktbzs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2tpzpqiiq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ncgqyhux.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2raiwfqax.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2fyevvnof.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2kiaywusn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpdjhhyc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xhphiqrd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2phuywmio.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2xhzioqhd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uprcrlxx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmwfccgw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ibjdnikc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fwqxetaq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pvjpfnbb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jautwwrr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2tfpdhbuk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2oglhkuge.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dpvcqdrz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jgdlxold.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2draagmkq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2awcjtzle.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sfavnlmx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgoiqjqh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qluphhwn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2trvoiivz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzcuiuue.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gaaadhnu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tjhplwig.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jiitvoih.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tdpkfisl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fmcilfbk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcyzeivu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2asenbwij.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uvkgnshj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnybqxyk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2frgaskzg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vteokfgq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2naifzczv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2hkrwuzxf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2snujohtm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsizxwqw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aecmxbyc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvnhgugn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xklwrrzv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2guxsrywa.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wwajyspb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2obqehneo.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2llodwhyx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fsvjjcqh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2yioaeeci.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qmfyjxqq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cbromhag.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tqzpxlqp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2atalfjxl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2bnmzmipr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2grmvddzg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bkxivyyd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wqhqpyht.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vuyhabnc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2xhvszceh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2poyvstyu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2oapxwfoz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2twuytsea.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2arpphzry.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsakyoqd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ogmgwrsn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2eitvdebk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2btbqxczu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2pbxhsysz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2loftclev.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlwsjucr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uopbfkdb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ahqsqyjs.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2csmteifb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ijjadclx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qszastva.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2etcghnfv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2rxjaevxr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ttbceuup.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2mftgilqb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hatjcovr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rhcalviz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2smwrvefp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jkklwyej.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2yklagivy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2axnhjaxq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2oixtilgw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2quyjltqd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uyaamnuw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xuaaukav.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2fozzsusl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yhxwclvi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2fkoxmxxi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jyshemdx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hvhfnmpr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhsohmtl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjiwqpwo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xnzbeuqk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pziqnyif.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tzppxipb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ofizunav.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ropdaigr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2feerisvl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jigsjghi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pbmcetzp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uurdifwh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uwystohx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tyxceshq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xqezwbge.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qsegnhcv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fhypeljs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2czrybrjp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2drcvntja.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vmvjcynr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2dlvhmefs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmihcgel.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lddriolt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2idicrzfb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2fjmlbgdz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qgzywdyk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vsdyxjje.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcawkxnz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2crfibubf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2iiysdyvt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2fwhdpjol.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2spkjqjwv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2dlexztcf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2syzdadph.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rpmcsbhr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qajypbal.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tkdtwgym.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wfntustk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pbzalduo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2groowzwy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2heehiyot.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2kotuzhce.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zvritkij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytuipvch.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2iodvqnce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsukgsas.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xwppwxsf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bbbeqhdf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuvgrjcg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lguisvzw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hipsrkno.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jwudscpf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2eooijska.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ksquqooc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qktvmatb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2dsziraaz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2akqxtkrk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qrzakbtg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nzemearq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2adrknzwn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ipirmqap.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xevwanaw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ddljzwuw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wxtwzhgq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wiwdzupk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wvuhflqh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uftluyel.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hqkpegsb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2flalvbdz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sjmnskwc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2iuqxdhdo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2edvmcysq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qkxdkovw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xbximdhu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rfjuecwt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwtwwkcq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbgmulhp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xlhradjs.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fdkvgwui.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2nyplasuj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2jxqsdfwz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2janinatu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cjdumwpn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2euqkwtcs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2mwyvufif.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2psupbpfr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zqxglsfz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2voyntzpv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qlamtqct.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2wkarctad.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ovopxoyh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2rzkpvtnh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ejeclhlb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hoaihcsl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qbzhviph.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2etbkzcjq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zwjdmdix.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2vokkpjmw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2vjwevdip.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2quykerzn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2pyawcaqb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uoswmzqq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ubtwzugs.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xvgxqnjz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bdpxuhnv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2mnordqgd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2jaanotzs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2otibdhuv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fwdqmtcn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2svmsbclz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2huiuetop.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ftsmtcpc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2mglukljg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rmkgtnnv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hptnjwyb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2bjeqoemz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2fnwxxxqr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2oynywoew.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2qhjerzey.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ourdcvci.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bupbausl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2dnfcexir.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2hhqasptm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvxsrvwt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2yvmcstvg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2tsadevzw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2zwzhhqux.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2oflxghbt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2weuvbbkl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2wkpkhfdo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2oovdrxhc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fxibpdnr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2cpckwihx.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2bppstjvi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2lopbtwwg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ueetktux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcskljnk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2lmtalnyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jflhlyez.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zhrnplgb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nexhzhbf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xjjibuvh.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2crzdqohm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2avmohvme.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2hqywuwbn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oergoopj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2dpdvmyiw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2rvldnfnx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xfdaqsgq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tnwgrlkr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2npnrwivo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2bdfoltdo.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2sttbewqc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jcsyrkpn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rvrsfkjw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jqiaszfm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uknawvmz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2iedysdhn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgaazumy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2dzecccgy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2bnzljfgz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2daqteehp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2akltbkao.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2erfiqeap.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2lfoduqis.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2jwzoeszf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2flgnaijs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jrxwqnma.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zvicgffc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2kxrjojjj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zxyhiitt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2obcobxxs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kywpvdqa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2otzhtszi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2debsmfpj.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fdluhrmn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hfxrzqag.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2molhsdeo.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2aukqkhgj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gfmpgxlt.html


<!-- 参考信息 -->