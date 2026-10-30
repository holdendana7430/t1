代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgsfycwh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpraruqe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxfjhart.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsokvrke.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glsbwybgc.sHtML

G. 面向对象
来源：http://m.share.fanxiaobao.xyz/Article/details/goojdhvqc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbrbsbjun.sHtML

[G01] 定义类
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiwdlkyi.sHtML

Py:   class User: pass
来源：http://3g.fanxiaobao.xyz/Article/details/gcjlhepxm.sHtML

PHP:  class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxghrfbo.sHtML

JS:   class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/glkxhprtw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbgmemcdc.sHtML

Java: class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gygsncyqa.sHtML

Go:   type User struct { Name string }
来源：http://3g.fanxiaobao.xyz/Article/details/gmzabjqof.sHtML

Ruby: class User; end
来源：http://3g.fanxiaobao.xyz/Article/details/grlormmrm.sHtML

C#:   class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwkgnuzny.sHtML

[G02] 构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxvbhrco.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fanxiaobao.xyz/Article/details/ggjmecfzy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gullskswc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsbrtmexn.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrjwqogy.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvfylccyi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfjszgsb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gvaahfzad.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyfmhkelb.sHtML

[G03] 实例属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucnjikhf.sHtML

Py:   self.name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxygqfgt.sHtML

PHP:  public string $name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gphynkdbe.sHtML

JS:   this.name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfaypmip.sHtML

TS:   name: string = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/glpdkogsi.sHtML

Java: private String name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvspuzyc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fanxiaobao.xyz/Article/details/gtbdrrinq.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzuvjhdo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gmiqgefyc.sHtML

[G04] 定义方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwqamduy.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtulflrj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnwfxdakm.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtjemvrf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptlgvlpa.sHtML

Java: String greet() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/garlojsqv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxunskde.sHtML

Ruby: def greet; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/geoehudne.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gcwswzdpm.sHtML

[G05] 继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyqfwrse.sHtML

Py:   class Admin(User): pass
来源：http://wap.fanxiaobao.xyz/Article/details/gntsnmnqe.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/goccyoewo.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzstfzfy.sHtML

TS:   class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvxadbqst.sHtML

Java: class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqcplfyd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fanxiaobao.xyz/Article/details/gbjhtjcya.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gheyvlcqw.sHtML

C#:   class Admin : User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtodhxuyz.sHtML

[G06] 重写方法
来源：http://wap.fanxiaobao.xyz/Article/details/gxnkaahve.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvrkidrd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gysxqoeoe.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyzxkpbv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwxfqffk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtlrsmzi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fanxiaobao.xyz/Article/details/gklawpuij.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fanxiaobao.xyz/Article/details/gzczssfhn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyyfazdt.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxovxlud.sHtML

Py:   super().greet()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwxqqnwc.sHtML

PHP:  parent::greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkycgqnz.sHtML

JS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gdshvnfws.sHtML

TS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gwselmrbp.sHtML

Java: super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gkqqmibzl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaerozzd.sHtML

Ruby: super
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxafubuoo.sHtML

C#:   base.Greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbugebvz.sHtML

[G08] 静态方法与属性
来源：http://3g.fanxiaobao.xyz/Article/details/guotebziw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsodtlzr.sHtML

PHP:  public static function f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gswhwcazf.sHtML

JS:   static f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwydowolj.sHtML

TS:   static f(): void {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvlnnybeh.sHtML

Java: static void f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/geegqpohj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fanxiaobao.xyz/Article/details/gpybaceew.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggatqbdya.sHtML

C#:   public static void F() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwfjnnezq.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fanxiaobao.xyz/Article/details/guzethclc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fanxiaobao.xyz/Article/details/guljeresr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzkwiimi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhbhuozc.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gljxcrqva.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gtbtynhyr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvszfofl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbticmype.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gfqodajzm.sHtML

[G10] 访问控制
来源：http://read.share.fanxiaobao.xyz/Article/details/gijdxhwcv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fanxiaobao.xyz/Article/details/gtdqbezfz.sHtML

PHP:  public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gxxezlvjg.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcsgladf.sHtML

TS:   public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyunxadpj.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fanxiaobao.xyz/Article/details/gaxmnvkqc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxtqkclw.sHtML

Ruby: public / protected / private
来源：http://baike.fanxiaobao.xyz/Article/details/gdiwnregg.sHtML

C#:   public / protected / private / internal
来源：http://blog.fanxiaobao.xyz/Article/details/getoecatl.sHtML

[G11] getter / setter
来源：http://wap.fanxiaobao.xyz/Article/details/gzfimdgci.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fanxiaobao.xyz/Article/details/gpaaoxgrm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcckmiltu.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcapexfib.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fanxiaobao.xyz/Article/details/glxyjnozm.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaqibfkw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gjlepvfic.sHtML

Ruby: attr_accessor :name
来源：http://3g.fanxiaobao.xyz/Article/details/gdqdoqhzv.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeqpszhr.sHtML

[G12] 对象转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gmonrwwbf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzznhwkn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjzniawm.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvalyrunl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqajrmygq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpasinpfq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfztfrcoa.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaqsijig.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/geunrxndk.sHtML

[G13] 判断对象类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwustqwv.sHtML

Py:   isinstance(u, User)
来源：http://wap.fanxiaobao.xyz/Article/details/grwjbkjwn.sHtML

PHP:  $u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gaeyyauad.sHtML

JS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoautnud.sHtML

TS:   u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsirqgasr.sHtML

Java: u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuwitycp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gvksqlxny.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fanxiaobao.xyz/Article/details/guptubbnt.sHtML

C#:   u is User
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvqjjacl.sHtML

[G14] 数据类 / record
来源：http://baike.fanxiaobao.xyz/Article/details/gtisgwdhf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fanxiaobao.xyz/Article/details/giyrfaenz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fanxiaobao.xyz/Article/details/gjefrqooc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwcopsez.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfyjdujm.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuzbbqnj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgmsjsof.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbxikwjb.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxtbihsy.sHtML

[G15] 枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gggnrjrjo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmzmmjlz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gohpjvdiz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fanxiaobao.xyz/Article/details/gvyrbhcvx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gpcvjgcuv.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fanxiaobao.xyz/Article/details/gwxlqlilu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fanxiaobao.xyz/Article/details/grtvcfctl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxbttkzt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggitdlxyc.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fanxiaobao.xyz/Article/details/gwmuhwunp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fanxiaobao.xyz/Article/details/gplhkijzc.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fanxiaobao.xyz/Article/details/gcczueieu.sHtML

JS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gereoccig.sHtML

TS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gpzuelyrv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrpdssoo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdlsxrbm.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmncppof.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fanxiaobao.xyz/Article/details/genlprmek.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgiaftkb.sHtML

H. 异常与错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gbzhiqyow.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfioaknnn.sHtML

[H01] try / catch 基础
来源：http://read.share.fanxiaobao.xyz/Article/details/govbwixfo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/gifncedtl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fanxiaobao.xyz/Article/details/glrmlkagf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gicztfoyw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gomestyyj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gdlefmpgb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoovnntz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fanxiaobao.xyz/Article/details/guzrdsbpe.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giepdruhs.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fanxiaobao.xyz/Article/details/gfwlqsbmm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fanxiaobao.xyz/Article/details/gqjvfplso.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/grmqhuolw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gszxmsvxr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwmfwlgiy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gowzvfzxe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqenfbrx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpnbcfbb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxefxkay.sHtML

[H03] 主动抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gjxbnnujl.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnjatnde.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxzmybko.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghilknzhk.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqwkwesd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwivsyblu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/glguqwncb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fanxiaobao.xyz/Article/details/glxuiawqb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gokssgann.sHtML

[H04] 自定义异常类型
来源：http://blog.fanxiaobao.xyz/Article/details/gcizvvctc.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gdygavwba.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqxwslcic.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzifinhx.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/gsuysxecn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddkhebhz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fanxiaobao.xyz/Article/details/ggiklszkp.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gwedqhlxl.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fanxiaobao.xyz/Article/details/gvxiqqcvq.sHtML

[H05] 捕获特定类型
来源：http://blog.fanxiaobao.xyz/Article/details/gzllzinqh.sHtML

Py:   except ValueError as e:
来源：http://wap.fanxiaobao.xyz/Article/details/gtrxoqpby.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiyrkcdq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gzxnsstco.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbplzkogm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxmhdijpz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fanxiaobao.xyz/Article/details/gflsjftjw.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fanxiaobao.xyz/Article/details/gjdyevvwb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gcdxrqern.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fanxiaobao.xyz/Article/details/gcqvlnvuw.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fanxiaobao.xyz/Article/details/gwcalmbxq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacpsxdcg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/gbsrexwlq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gmfwasekv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxshrbqd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fanxiaobao.xyz/Article/details/gmshhcoiq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujcuiate.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlulkuhm.sHtML

[H07] 断言
来源：http://3g.fanxiaobao.xyz/Article/details/glkqmanuj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fanxiaobao.xyz/Article/details/gssswiswo.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcacbkoo.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbngmbtrf.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/glomhecyw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fanxiaobao.xyz/Article/details/glsulhsjd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gabdmfrkj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtjcowdc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzomrztl.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fanxiaobao.xyz/Article/details/gyzyiibik.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fanxiaobao.xyz/Article/details/gvdxleyro.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fanxiaobao.xyz/Article/details/govztljan.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmwsfvor.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/gibwmyshz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fanxiaobao.xyz/Article/details/geltokucn.sHtML

Go:   err.Error()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvziskiz.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fanxiaobao.xyz/Article/details/gkfofcvab.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoeqnkiv.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzehvzjgk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fanxiaobao.xyz/Article/details/guehafuhm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gveudavma.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fanxiaobao.xyz/Article/details/gnuiixluk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fanxiaobao.xyz/Article/details/grtqzzbit.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fanxiaobao.xyz/Article/details/gulgimyte.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gmedzdqqt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxumewkzu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqukvakzj.sHtML

[H10] 资源自动释放
来源：http://baike.fanxiaobao.xyz/Article/details/gjokwcbxv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrrjkdpb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grynnihqv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fanxiaobao.xyz/Article/details/gblwavsde.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/guazfupto.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fanxiaobao.xyz/Article/details/gikjgjkvh.sHtML

Go:   defer f.Close()
来源：http://read.share.fanxiaobao.xyz/Article/details/gckuxlilg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwotlhqj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypozgrdg.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtikkfnfs.sHtML

I. 正则表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gseumjbnp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvchpzpcy.sHtML

[I01] 判断是否匹配
来源：http://blog.fanxiaobao.xyz/Article/details/giodbmzwn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyuidhov.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gskqstrcg.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqjpyeeb.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdxdtkfi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlmecjxl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaodlexg.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gabzamiob.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gdzlisruh.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcdzkzlh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gsdcktqow.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzoreffw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpgbiphd.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gdwcdgwfs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfyqwcepf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/glaoppbkc.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrmfezks.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/guyruamkr.sHtML

[I03] 提取捕获分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gjymnmojf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfrxzcza.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgpwrghk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/godtqbayk.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gzocbaslh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsptlqmoz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fanxiaobao.xyz/Article/details/glfsuoxti.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gmqihnhvl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbnwcoua.sHtML

[I04] 正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gvvrscxsm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gsatjsdrm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtknzrgew.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrfkexej.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gycjslsvs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzielwuqb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsismvgmm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/glmswjhri.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fanxiaobao.xyz/Article/details/gyvsaxxih.sHtML

[I05] 按正则拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvwmmgkr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdvijgci.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gjiibhxdk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/ghiulbuat.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gpbrknfpv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/gqtajoxis.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmurguymz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/gwnpjztpg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqhfztxn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggygomrtg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/gydwxaiva.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fanxiaobao.xyz/Article/details/gswdidtik.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fanxiaobao.xyz/Article/details/glfwkcwsb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gdljyqxhc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtslhtyrc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fanxiaobao.xyz/Article/details/gexcsekht.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fanxiaobao.xyz/Article/details/gakooybpp.sHtML


<!-- 参考信息 -->