代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2unchgmgh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgyplmio.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2karvxuhv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jadqcqno.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tffevozu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2bkibqjho.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2uatfjggb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2saseetru.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2axpezhos.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xtebwkxt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2biqnpoul.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vvbaesks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvnxsqhb.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2gurlnvds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcwxucqi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2klvyvteg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2retfnllo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzzkjnoc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wiyigddo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ikcekpqt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hayhajlw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2elhfalae.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jewixart.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnqxtgoz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zzzrfzxo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2klgjzwgk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2puzksawz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xbbjfwxs.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fznqiuzi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gsxfaiej.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qmrktccd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ljawiojw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nzdczpqf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gwxwrktv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qyqsbvhn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2iootmsnv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ccamqhfb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2clvtbsjk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jafxenuw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qlllbnlb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bqfrgjtm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cqukmsxn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2grqmbmti.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mrlrbagd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dujzcxrr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blmsmdhl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2twgebyhf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhvfxzos.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2unartrpf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yaghqkbn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2aasobdcp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2qxynebfd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2gvtyenxt.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xytfjhkc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ojewgeeq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qablshyg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzxfdoij.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2owjqvlfj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ulhqmawo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgpwwpvu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2oameftuk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2sitdundf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ssispnzs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgsjkfmv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lduortka.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oqocjttg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2nigsnmbs.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hoeebyts.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2txhbcqyt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2sasrhhby.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qcttufge.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zaocabwr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zkhguvmv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qploynzz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2udeyftrx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qjlyhecw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ntjmeuus.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hjuymgmi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2icbmxlok.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jhpxwwmp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmeecfjc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2zygsppom.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ytdyqxhs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2tgyxitje.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2eeyepsrq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2iiykyhbk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2zaivkcqa.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2gkroskzn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2gkqwtlxa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajhosbml.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qwnjbuuu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2viqzeunq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2njvwcxbo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2usenrtvh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fesabcmo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2blsxyggk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jzcadqdn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jlxcwuov.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2volqatmo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2btaqxyvr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2npdlrdyl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ypnxyucf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ipsfcqdl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qwnyuomd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nfwipsjk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2pvxngcbn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2rusphuzc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vrxbsdhk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umnkinux.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bghfedds.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlpetunp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pdbflegk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hlmltqel.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wixfkqwr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2seibilgg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2adqjwjpc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2imaewceh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zqxctxzf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocmcquyt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwbzvosr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pmfoaauy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ubdoqjmc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rftqwkfw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2nfslleci.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wcumbszf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xokektdm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ukjizfpn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fhlgowwh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2okudpjnq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2oszwazqt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2fqqszvjd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2nqwllfpd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2dxszewtc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2cuctgxwm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vbouvjin.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2xlxmicvf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2lyulbwqb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2cvjjmyqc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2vffswunq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2elniowvk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ipalsxqh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2sogigcru.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xvkyqkmx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwnlvlev.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mbgmnpnw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kxcvdsrp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ezrzteqm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2svuialbb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2zjcecyuq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gwxrpwwn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2cbtvandw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ojwbisdd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2kqoctnrj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zoxtczsq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uitualvb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2istjmfls.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2rgpeqdga.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2beyoskly.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dpdqyzux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfqqiznv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wjfqfbka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsmvilxe.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2dpdgzzsr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2nvcrbbol.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2iystjpxi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ozzqzpyj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2snijhifk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2hqbgwktr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2yrngzwcq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kpfsoinz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajuexbvj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2scwaoidf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2enwgvdzy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2owhpatgm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2majtqcil.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogcxwpun.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zleqhoon.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2cznrduwd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kkafasyh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfizepqa.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xvcyjfrt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2bhowskkp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rkbitiox.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ynqgsdyc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fcyrkylp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sgniveoh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2kkwmgfnm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hmmyscsi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2spifjslq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2vlcastpd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2gkxkkroy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2otuffnzo.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2keadnafw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jzyrwnpq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cuvvoxva.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2uijojynz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ttwrzfka.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdcgpqev.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ghnhnhaf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2bpeuyfmr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2amlojelc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qqyzbyeb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kirgtbyd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2zucblugc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ryibjokn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2chhtjuzs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2qxcktdnw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ucpabuti.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2pozbdrur.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tdfgdmcu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ylommkag.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tjoorjht.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xpytnjxh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2yeglborr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2lkevxbox.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2unkppfhp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2trobjocw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2qrgmzluf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ylqnyniy.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ttedwnaj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bwueqcbf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2wooirxkh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2sigpthxw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2unrfbvrq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kwwoaaou.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2olrarnvi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2alwsoeyk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2lgmukbnl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2cgrkdvfo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2elwpiaif.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ityqmqrw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2zkdikpuk.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2mhdyocrx.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2qhnzfxjf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2juojvaff.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ohyysbsy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ohxcedlv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2xkegriaw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bgqijblh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ktirkuvy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2guiznenc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2mhojrkar.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xmvtxdqe.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2gcfbfogi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2euoovlqr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2yaqqlfwk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xhmtxxjo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xrvjjeet.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2aouorsgq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2wxbevdsr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2gsazgbrg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qmdhuavk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtxjpral.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dcjjrdbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyfprlwn.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2bqmltpiz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tuzckcir.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xrmemkpl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojxofuoh.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2yfyqrzed.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2kurvyzsp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2njwwimwg.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2obrphqzf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zkzlrcle.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2wbszzwod.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nyoaxmrm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2esrculmv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2zvvttwsl.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2sldwcvms.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gyygpgcl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2giqwoabr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lcnxjjrj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mltbumqk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2rggiaeqz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2zdsuxtng.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2mkqdcifr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2euiennbf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2edtrtbbe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2fmyjooox.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2bghjodbw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2duxrnldj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2fjxbqajl.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2cuwcxsoq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dnaqfyvm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lbvopzmz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gdqukzop.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ckrplfas.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2igzwmjue.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2zbynikrn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sudehlit.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2sgybeebj.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2cvfigugo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2idhejilc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gycbyldr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2khzgnmtp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kspcxfzs.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2xppcghwf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ivlmatpu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2guzftwmh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2jmidahmn.html


<!-- 参考信息 -->