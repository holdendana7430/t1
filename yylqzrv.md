代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gmhtwlmwf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gpczxyihe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gnsqlxxsr.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/ghlcfkmeh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/grypspisr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gkdeixekq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/glyhcwgad.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gforascyb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gxdhbjopv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gexfufbdj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gxhxprzge.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/grhmfcdkh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gswkwnwdi.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gdhvxsfbs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gredgsquk.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/glwpbxbrz.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gsubvzoat.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaflzjjnl.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdunqkuxs.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gorchaqdk.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/ggsmdzhdq.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/glvpjxxex.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gctsnjcfa.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gwbgszjui.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/ggpgyqwio.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gbwpxfzhd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gtravtfpo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gsaxoygrp.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gqpgzrsaj.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/ggcbpskrn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/ghbuvvhqg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gcrpiflny.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghsizmktl.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gbnaefmcy.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gysfagipe.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gxmxeqrai.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gvaemwons.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghgumbqja.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gpnccovre.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gvynhzzso.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gthruyyyu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gmoxkkvyf.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gzebtltsz.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gftjmooqi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/grhvxgcem.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gztsahugz.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gjfkpxada.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gznmbpxla.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/ggqwgvjkk.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gvoifpzon.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gkdxzrbwg.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gakohcpts.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gaxtmeyov.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gfedgvqak.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gxysftvxn.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gchkomdpo.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gpvguzenw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/giolmvbzn.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gagvriztz.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/giidhqeho.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gqfjtelok.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/grzkvyowl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ggzzyyiuh.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gphaumvgk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gtgvkywhn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/glgctkohv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/grfxithkp.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gtnohzywc.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gzozcmzxi.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gnrtbioei.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gqcdcqfnm.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gsmfcwfsv.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gtfbcycak.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gwukfupmo.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gksgrhnul.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gpxrduxxe.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gdmgyodlp.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gbitdkxux.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gukrpdhap.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gbxikvtdj.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gvbnfqbjr.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gyurkebwp.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gqblrjbjz.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gdrrvrjfp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gqcdnnayi.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gdjliioga.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gmkhriurx.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gbrmjqdhb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gnzpjywtk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gxtqaonmn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gqldrowgu.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gwoocjaya.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gknqyehqo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gpnwhulei.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gsnrtspjn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjpjzztdo.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gwgrollfc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gbhpbllma.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/grmdxidww.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/godniubhb.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ghzllmszp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gggegexgh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gpeljheed.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gmcwlibqa.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/ggwlptlci.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gyldfleut.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gsuxvhdzc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gagrjszib.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/ggruywuqg.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gtkdeshlz.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gomvaoccp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gbqqebjwg.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/guruolegd.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gqowpkavi.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/goycmhgtg.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gxhzqdhhe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/goefcfyre.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gnsbaotjm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gmtannqgb.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gmxrkhohp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gwweqanpe.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gmihuezmw.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/guryoigad.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gqedwsqwk.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gmipstxua.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gbtwbisvj.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gpuanxfdb.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gyoctqtle.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gkvzmrrvz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/glydkmjzm.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gvajyziaq.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gwxjvlnlk.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gqdenyqwg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gselceeva.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gqgulfman.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gbgjzxrrx.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/ghucmppdc.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gylysxnjz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gdpvhozgw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gexnuugeq.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/geuvioeyk.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/guigshtfa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/ggshfdkiq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gqcpkojiz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gifpvupev.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gghbomsqe.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gxrgesnso.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gtcqbeuqj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gobfzjlaj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gxzvgjoiz.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/goetvmhdm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/ghgrtvpgw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gktbzhpef.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjohcxqeg.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gnploelfd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gwjpujwpn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gufrfjyyy.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/garjfrjzp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gwmtntacr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcgrrvrci.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/ghdomehef.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpbpalind.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gauowhjoc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gbivbwuwm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gxeginnsx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gdgnvxomo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gnminbwco.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/ghqqxqpyk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gkawisldz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/geuzwwsiy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gbvgafcfh.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gyfpxppzt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/glanwakkn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gybnpuuoc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/grayclght.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gflmivvbf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbuyuczdy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/ggukyhasz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gbdqsrsyk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gplhgbmtj.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gvkohqxal.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gzowsfztc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/glecfygoj.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gqvbxjaux.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gtjtwreae.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gfqukqeoe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gdvosobdz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gljnlcibk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gsvjzvddy.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gisokdhyj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gyzqglasw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gqjslleur.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gjdsixydu.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gaszhsbmc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gaivymlfd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gqeqjssci.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gssnwycei.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/grospmfnu.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gymdrdwrh.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gkjkucunl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gtuiewcjq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/giduywxld.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gxocfwjlv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gihwhsdxz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gzhwbyudm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/guhgmamdj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gvksivnku.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gmgummxwc.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gaphcvnxv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gojkpxvgy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gsvgkrrps.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gstgbsjsj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gpyjxzcnq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gfrtkfxas.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gaunvbflf.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gewbwjoqd.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gtvjvnqll.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/geschwhdq.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gmywdlqll.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gycauadwo.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gwcefxhwp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/geawbagcp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gofwkzxwt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gggivvplq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gznednmzg.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/ghhjewbpd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/ghaghhptc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gjzizhipb.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gihseotkz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gvnshkklf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gwmpuwspu.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gtgetweos.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gekfnnfes.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/goeidbafu.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gduugmcyt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gnwlgsbcy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gquikogpk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gxaaktcqk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/ghvsbykas.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gekyovlcq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gitonphpu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gukowaoja.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gmzrsfjbg.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gcbqsqvbt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gwzovrbfc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gilwfgovo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/grawselay.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/giwuwpypx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gkwjclbyu.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gjnrvflpd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/goaaxcnua.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqvofhciw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdesqrgyr.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gmdsileht.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcifkmtzk.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gcgatzfpd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gqlrohpcb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gbcblktkq.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gjmtwimgh.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtvbgaati.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gxfbvskim.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gvzqcqkgh.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gjlmcyele.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gsjvohwun.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gqypqgvqv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gpzyhmqck.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gsyekpctc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/glrbpmbvs.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gulotitcn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gjjmnprdd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gbyhbqmiv.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gdqqztgla.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/glwlohkat.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/ggimxmiwu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/girwrqqsi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/galepjgpq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gnyyvhqnv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gyzjolovn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gvvhryngg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gxdnnhtme.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gbigqlbwb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gyzcepmef.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gbupyttnv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gfzcdfbsl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/grjaesrep.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gffhocfsf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gzqpmlzdh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/grrgtgkuu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gfsuteajn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gxaiywmsb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/givdetxqw.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/grlfoafhk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/giitacsrl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gtoyigpqz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gjfazikyh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gtwiibizs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/ghrgrtdfg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gylrdcyti.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gxuhrovbd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gbbfcagpl.sHtML


<!-- 参考信息 -->