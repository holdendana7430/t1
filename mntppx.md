代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2yvqzkyyc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkjmbrbh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ckstgupz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2loaxchpc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qyyczwmm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xhcifsop.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pywottbd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2apwrlbik.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2aremndjr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2gbxdpfok.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2efeotien.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2oouoispv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofezsepl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2jvmdumum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zkaldvvs.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2mcyfkjmz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2oadqxlwc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnfbyezw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2doasdevg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2csqwbhjh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2aakcnzrb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ewdawtzp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ntmapxvg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nexcnvxh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bscjxndw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2neiukfad.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zddodxgk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzzhmury.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pypllukk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jyjyxsht.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ksfihwlz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xljgsbrp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcrhkyzk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ykmhnuek.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cxtczwco.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cftiewvi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aiqnmtki.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bqmczwde.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rnyutxzv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2jmbjgtrg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vjwtjfpv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zdwxgekp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2rnbtqtsj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yrflbbfl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sddlzsqb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kqrwvdsf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2arfwcdmx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ltjiqtry.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ixszbffv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2utstvgbd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vwujvabo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2enongakp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mstlpvje.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojmblocv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gvyninur.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbiwefvi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovmjigbn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vsulnhhb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lspiphnh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cixhpvxc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2meqywcgv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2pvyrsdac.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfidmtsb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2weuojvjs.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ckfmzavn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bsarqrwu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2mpsfdhuw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ydqbtbmc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2lsxshpas.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2abaeacnk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2taepdtbv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2wqjtpjbu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xnspmyei.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2slkgfglm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wajcmauh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2msixtree.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dwkyzino.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hlprfwoq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fyrlrxxj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2dbyufklv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2objazizw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2xzdauhgr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xtzfeuwz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ddubkwkz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2dxnsduyj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xzhrzgue.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rbnjwggd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vgujojei.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2uwzndqqt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2guvxdjjt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fgzkzsqr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zeiuyczt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptxvbfwj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2azzzjskm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2eoywsuuf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2jiqlzglq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mheyiaol.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2jglgwrpz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dvtlpbtr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mmexgtak.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xqknctuv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ryrmdsps.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ztvrhgdi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2znekwqve.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2letbnosr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2zetrvtvz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bvdbovcs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzzasbmw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kjgkcjoj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynkckbjk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrzssxxp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2feiacsxg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jtxqzwyh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2jgbxqzeq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xhfmhueg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bpdjhark.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrhazycz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pzujwmex.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2leooeydm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fzhwyczb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2frplrdfa.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hdpffrkm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yvyawkxy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2eazdohks.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2cawexizs.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2soqvsozp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jjmhvozx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bxfgywyl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eaofokgi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2cfympbfy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ilkzxzwr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2jnhqnhgm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2muiwiiky.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kojwtrbi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vurggevz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ppbbzvad.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2gixgmluf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eioahgyn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2tjnjhgpj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2gntcurhv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qmdjzvzu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ehiqbkmf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2iguprsds.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkcznyrd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2uinzoykt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tjbljica.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wqomcjon.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2xlvkmxyy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jsbzkdsh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bbqaerte.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2twccbltl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2uyqaionk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2kqzioyrq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qojbawhu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2brhnlikv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jislpbat.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2isbhfsof.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tiybftog.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2johfygsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvcqnpxs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2oeugcvda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tiyxfkmp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2cgquhcpw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2iwarnmeb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2nwtitxmd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gdoljesh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nivrcyik.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofjaqxgh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2wbjkmvmh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2dwkkxfst.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2nygizcsm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2kmycoqmt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zkzkwwnm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2axmxvrmc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2idxuuxlg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kctfrbrr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cdiwxwxr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2kveahdjv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gsstpfhw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wmmepaio.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gsdvxdzb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zbwihflo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2miyzmnhz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2utseoqrr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2axqoolkz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pafufmuz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2wvhhanjk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2tglwnnae.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ghwvbsod.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2nbzzonjt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2wctqvcyf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvuroejy.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpedghii.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajxdhlmk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2achwgidr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2usxmbdif.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xsocnqwr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lcsamjrc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2qkxzgnyw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2bhuvvnzz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2vzenimix.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tlfttxzw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jayqlkzf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywsnuxin.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2fkpzqrji.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2gblmfrag.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mfsdqklf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fitqcqyl.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2levogwsj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2uxabtzzx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xgoizpub.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ubxsfabd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2vroovadj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2cfqxdriw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ivfildbt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2qeqjozqw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2clknpsae.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ccohjvsp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tsjhzksh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kyslbzgb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sdfgdqpm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2frjjxhri.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2kzhnglzj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2hjpecamr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kqiautfg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2pftqsmrp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2dttfyops.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2quimzlzb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2woorfmgy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2mqkwgoqf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2vhlvpuma.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2euppchcw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ipujyvra.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2nnozheci.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2xvqertgy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2msnkpkav.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2lknppjeq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2jdmlmqik.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2weoqpeij.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2chamhggx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2nfbdzfil.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2bszmqjqr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2onzeleqn.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2qkbcdvek.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qsnppqut.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kosmdtbr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2yolmdieb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2sazcoydj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ldfxials.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ofrajqeq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2jjdtohob.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ofpplifn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwbgshgf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2dxuscskx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omxzjedt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2cdpvxqbu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ujgszsrz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2erctoefv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lroqtvvk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmwdzxjw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2xkdmibtf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2uxphwtfp.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2lnemkruw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2oaxsxluz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2htaysmur.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2dqukrzos.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2jpygbhhn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2lwapaqeo.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dmravuqw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qsbqoutf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2btehmtew.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vvgfgpkm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hjafhruc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2bcrrpdci.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcltlhfc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pngxdiob.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2otxxdvpy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jrxsrolp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2tufwhsgc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2mlfytkxh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2iacxxbhv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ojotuxcr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ueqrakfm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2elrurmzr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nickkekb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ytjnwcbw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nzsqzrpo.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2rcvqkxox.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2jljmypar.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2xisgnomp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2lzciwtzx.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sotnyosq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2djqphqpf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2flqrzvcs.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qlhjqxfr.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kzrjlxqu.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2zzwukwyr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2walbxyyf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2unsvwfyd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2pyuofosz.html


<!-- 参考信息 -->