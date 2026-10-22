代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2eqcyfsbx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xascjmjb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2myhknwrn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kpsjiuub.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rinlncam.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tjehxgdq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2pxnchesy.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2olmpybrm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ouimomlo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2hsxaikyu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2gusutmip.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qquazizz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yaifpcye.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2jhxwzgcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mooyehjd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2sxncpibs.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xjotqnxr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2hpfvmaen.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hfnwowrs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gyvvuogh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2psmlyybc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vnpwjbso.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mrfddzsi.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lwsiokve.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2lwtxzbsx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2pguffizq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysobmvwa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfgcbxuy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdebgnfl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2papanfpt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2eozhhkxh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yzqahzni.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzegtvfg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2pfyuhxxa.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qadlaamf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uqnrahzg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2afvdwcya.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2apxbzkxw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qxvqcoqh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gvqqnkjj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tjiemhty.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2jcnzbxcf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2rimyhjix.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2onltnwkh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fapjjjjl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaiklpuc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mfwydwnx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oichqiqm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xhqhgjbo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tnonykxn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2didastwj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2vphrjhsv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2fyworoah.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2olsgakss.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwfxdevc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vcupznxn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfwengrp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hodhzvgx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvhajnod.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2dnizlvyd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2fizjfjfg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2murcixtt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjrpdudh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ahofqzju.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2whqzwobw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbdixtko.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2wfcmxnex.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dpsephsy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2snleirte.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2agifuguh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gifpgpgb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ehwenvsl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vsambzlz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2osgzcnwu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tvnjzboc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2afrdwpak.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2pmboiior.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dpankjjl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2icfjdfla.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dygyfuao.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2graogflz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2puyaoxvk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2sulgdeon.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2iukeebgq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qvoltdqz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ncnkzqse.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbofbxed.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hcxebcdd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zzzyplya.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiavxbxl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rkuzprjw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkfbfwvg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rqdfogns.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dskyzlqx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2egitetti.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2wevlcdnp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2dctchkwj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pmqpgjwp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2aobocqem.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hizpbjca.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eihmvfbg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2bwrsbymv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2hfotfisa.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iuzmrgbz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2uwmxsezy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2oplzwufx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ybnniimy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lofqowyr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cpxtylcg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvxdxqsl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgijcamv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oecphvso.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ywvxytoh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2krdvnodt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ypfryyyd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ypmdkusg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fekaewyf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fyqcsocg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdxmsxpc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdlzqoav.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gxrdemgi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2moimiszp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ylpmycoi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xaffczjc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2oedbmzkk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lktotrxo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jntnnymo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nczyspas.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pufjtxaf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2yjkpgnqg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hdcffndz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wkjyiywa.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qafdvqnz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vcdkvnvg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hzjdrcil.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2dccfgjtq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2dbabetky.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfldzxso.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gclgnqgf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2omsmtsmu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2gvuomhhw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2buveafdn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xdbskkij.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xztuixtf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2gvgeukep.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gfghcwzb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yhkiqtpf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2zsrqyhwq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2spjsydxl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lrzhuhck.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ydtadqdm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2apkaklcl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2feyaicpp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ffdlyqin.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oqcvpomq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vkcgxsxc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2odisdjtm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2iyebxbjy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2nzvfvzrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibvdiygf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xpxywckw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwjxfgku.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2kkajcfnm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2illgdcgq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qbsmknpx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mjzubjsj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kisvavou.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwloevlv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2cihtvqpk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2dhztohep.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vqitpflh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2kyvitrmu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ekysqqic.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrsadfxs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zwhbzzpd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2saetdcnk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcyxvhuo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2dikhhetu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2bkcnewjd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oifeljhk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dikcdhmc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2shparlux.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eewgyfoq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2twjfaqyq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hoddtpga.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fuyhidwe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2pywocrav.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2heldzguc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ijmceryd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2pqixddal.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bpgxhkso.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydbquxwk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2uykazqjp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cwgqczxm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcxubhtt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vdodzxoz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2xqkoksob.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2btvjiapt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qzfzhpxe.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2tqsjzhdx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2scnfsrte.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ersxewqs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zopnowik.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2nhdnakgl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2vqztkmqb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2vstzfjgb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqmkzalq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2hzqbtyll.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2hmwopohe.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ytigawpu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2uxtcaykd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2htgqjisd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2eonzvitd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2wwuopyzc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2iqoxivqu.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pmyjlhpe.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mgyoyikv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2uveaauuo.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2omilempi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yfvjjpkw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jmzmdmth.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2kslldxwj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hhphfblf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2hgevfywv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2csddzyel.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2nskcndgb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ctjwizty.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2fpezitfr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2zklzjboy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2udbvcpis.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2thbgmpai.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2fwwujoyr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2tewtrbox.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2pfgpoups.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ahunivoy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2xypqhcjg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2zqxluyqs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ebpwpiaj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2stltvgci.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2tduwpxep.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ikwsaiia.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2rghipbuk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2npcclzao.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2eohswkgt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2vocihjta.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2qkorrnvq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cungmxdo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bensshlg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2fvavunzx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2eumlmmsx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2unbimosz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nslnmrxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbextrgz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2rpzmasah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igyqqhxq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2hophczha.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nmqyhgtq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ishkddjv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gvigcgoc.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bfbodhhh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2acldqzen.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nxxinrun.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2juxcmboo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qyqxewnl.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2wghvfhbb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gccshvei.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2nzjjblvh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2pywzshsb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2urodzzgi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wmpjpdmo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lphomjfb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ewljayye.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vivtgekc.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2acyvdvxe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2oywgtktq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cnvvsqhe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2fxkrwvsu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2exeerdbk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2hiobrczo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2cegeaexx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2esnnrlyr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2eylidmfw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2tgvwgyba.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fadhwmkj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cejmpuzd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2zgywhcjc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qiqtxhvg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2pztiitut.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qwpadxrr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2seskihap.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2eafqbzts.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ruafaxcz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ptxmtwyg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pqivunzy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vhgkjack.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ueieshfx.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2zwidbnck.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qkgoysjp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2yxfletwt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2dujgegnq.html


<!-- 参考信息 -->