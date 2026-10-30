代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gjzjihvwk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gypudqhri.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gekqhmpjz.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/grmytnzsk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gztbbxuos.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gpbfignhw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gyzetswxj.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gleuwdmkh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gtakbdqlj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gffhexqud.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gktgiyhas.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gzhgmuzva.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcoczvrls.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/geghhbqfc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdwfnigut.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gyxucbayd.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gmxdqrkao.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gvzryghbl.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gvtghyfzu.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gqgeiyvdv.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gvrnfcgdd.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/golodqsgh.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/ggxowipka.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gywoszzpu.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gjkhebqzq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gslqkosfd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/ghdkerogy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtkhuiieq.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gkvzdqxdd.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/ghbtoyhwv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/ggdcmtbgt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gxvsfmwvj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/glqueqqbq.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gmsnwoejf.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gkoqhfaab.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/govwsvfna.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gkjavcoix.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gyysccfho.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gobzqdikf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gyzqvmlzm.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gtqreirbe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gjlzactpd.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/ghjevtqcv.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gctwygszv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gvdpkpbvy.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggmuwwutg.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gbzluepji.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gpzwlksot.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gbewsswdt.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gmqbukhwh.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gqbctodnw.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gaxsfxcap.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gxvvqfxdl.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gmkzylhab.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gesacospt.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gtzyyclby.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ghpywcrvt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gpkayxzpu.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/ggfupuaiw.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghyeremlk.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gdccbwgzt.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gjcjbtwjj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gfbbzlzot.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/goktfajzq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gkfsxambk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvcduvjre.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gmrszyfml.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/ggnqfvsly.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gjkbhizkd.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/ggmpawjae.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gsvcazaqf.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gukvtmtgv.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gcqrmyjns.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/geybzxnjp.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gqgbyhnvd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gnmcomyaa.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gsnexvlwi.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gsdggqavx.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gowjcxjha.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gtcxxkqna.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gbfzqslpv.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/ggbsrnmyc.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gmilzyrnq.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/ghyewgivy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/grwbtfdgf.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gkefnifvw.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gfglcbkwd.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gbyzhntsa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/graefrdqw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gwmnvzbnq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gbaevhupt.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gvfhgchip.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gwcgpebuw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/genwowqfp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/geoybwjmy.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gzaaajwut.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gbvwkgtsa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gxgtfvffi.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gjhlnvlhn.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gnuvxgdym.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gttfoweys.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gcfliwnfe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gouopoycw.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gwhzumjzf.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/geebjctwc.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gvucljwur.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gcltddnxi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/godpqrdiy.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvmiydyif.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/ghgalcyga.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gecfubbfj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gkcfgnvam.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gimsfsorp.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gyisxzchv.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gkixpfvmm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gvfwppckx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gzdhkkbyy.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gxdlnwalc.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gmtywirsj.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gybxulvvt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gdguqlkxi.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/glnrxzdup.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gqfxgtjwn.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gwyvmxckq.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gsftawbjq.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gbkwdbzjv.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gduzgefwx.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gdxvwgmdv.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gtxdfiqjr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gzthrzixp.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gkqddbhrq.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/golbosxvf.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gyubyhfua.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gyoznrxon.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gksvbtcvi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gzccjbalr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/ggiwnpxuo.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gcqczbtfg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gmvyblvmo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gmdijweiz.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gwuvqivwn.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gcyezdijc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gyxflorhl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gbdatznbc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gsugtugkh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gwwwlmguq.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gbhzlndml.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/grquafiaq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gqxxqamah.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gtbvdhzac.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gmxchlqfv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/glpqzovhu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/grntodnzt.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/grfsrcqdb.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/grerlonbs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gqgahefxo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gjetdqmns.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gtzujlgpg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gkbowqarn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsjvcqgru.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gkppzbndm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwctboras.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/glfqpdhrv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gjsfdkcbr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gkdbwvuzv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/guerpsydg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/ghuxmqesq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gtmvwnffz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gjltzqmnf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gxeragnie.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjseeaero.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gtegahvjx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/ghqoiemed.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gkskoxuwj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gagwvgaoi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfqqgycts.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gdsqcnpft.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/ghsmgdmlb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/goavrkhab.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gehhyusfx.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gcvhmcfan.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gcllntdnz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gmtbsmftx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/glgmqpumc.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gjfdhzpsa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gwphdghaw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/ggxglixrg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gonayxtus.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gayglsgyz.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gpygtpdks.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/giaosnghg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gzxiftzta.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gordqkpjl.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gdeuidpyv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gljavgvzp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gfasazkyj.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gjkprnlsx.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/ganwpxduh.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/ggvuootbs.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gbfxagawh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gnjcfbfhf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gavgsrclw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnepbkzlf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbzqhbjlu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gruqmppda.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gesfewafp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gkhmmyfty.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gilkenmft.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gpqhdkkxw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gmwekyyhn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gkrltgcsp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/glzuaeyxs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gbekyaxbi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/ggmvcjdwc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gbmssdare.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gomixxkna.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gufngewdf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/grpozhdyk.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gnwiltmue.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gezdfdbkk.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gpasfemfz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gqkvvqlqc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/garuuggso.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gqtwuoogy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gzgpmxuqs.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/ggctqqkeb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gpemwutuc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/glljrfrwr.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gyugukmlb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gmgqjqtsb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gmakuzeom.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gtsfynqkg.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gdsrwtkff.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gxybhhsiu.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gxnbwxyfz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gryyhukkp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/guqohywqk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/glbdhlooa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gzvjxsycm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gtherdreb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gkrcauszw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gzizsrguu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/grmbjzuzt.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/gbkjfmule.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gxeirqcis.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gejnbvagn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gkqbujqlg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gzuiebaoy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gjaeaxyrn.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gagfyalpm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gimwkezep.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gypyavuhd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goickmkos.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gpyclfqxw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzlxhverz.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gsgfbtryq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/giopvirqe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/gofvgeuwl.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gpazpbzit.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gagtaqpwh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gtesyctor.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gslmcvesg.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gctbdsakm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gayzrgggn.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gflofpsqc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gjgfmbeur.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gbxrhkiuq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gkoezncqh.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gfhigztcq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gtqczcutp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gdlyrvvfr.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gnpxnrquv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/ggspsuhbt.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/giumqmwpc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gufrsgpdc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/gpywmvkom.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gmvzphqpj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gdmbsctyg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gcgddjylx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/grdshvfai.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gkfmwkdzn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/ggixnbrgc.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gokbasyql.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/glzdkwdno.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gcubpcnge.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gyefymcbb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gihxjvgfd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/geyqbdmwj.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/gesvcebhx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/grxuufnth.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/ghpadcdrx.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gcetylgft.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gvuqsrqmj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/ghgcamwre.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/glfpsxpxd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gxppuubnl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/gmdmeufri.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/griorsmke.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/ghysqzgel.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gfnjclzds.sHtML


<!-- 参考信息 -->