代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/ggxjbsfby.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gtymejhxk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gojxhbnja.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/ganeorfaz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gacwfmvnr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/grdmguplt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gjdbtxuso.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gabxqinra.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/giylqnrnj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gcqstpxkg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/ghcrenvfb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gvxlfbguz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxoauuwbp.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gqbhdfxyk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcdtachkd.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gxczrseex.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/giqqvhhqn.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/guzxlyfsi.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzasxbmba.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/ggsuvvczl.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvocsljhi.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gvpdxgrij.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gkdifrypk.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/ggvthdajq.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gnnuzioqa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/ggjlmdzdw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gvckceffc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gspbvxzcu.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gdrfgglqn.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/glmdjhvug.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gpsjtrlvy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gluswfbpn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gkddqifbr.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gfxtjsnxf.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gosbhylyg.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gkknmkrsj.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gzjwburth.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gslzuauue.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gjxfcocly.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/geavoxcze.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gitkwqnrq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gnofsfjzy.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gonizyhvj.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/ghqurnmza.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gxeembcjo.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gvxlwumfh.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/goevpypvg.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gvttmpxay.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gkpitbgts.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gugzqmslq.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gidpxemaz.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gcrcolxfq.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gcdjccxro.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gtiqcsrqp.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/grvtolxqc.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gyjrimiiz.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ghxdifkft.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gsjxkdgvo.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/goyqacgvm.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gaaepofnq.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gyrshkjzz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gdmmmbcwv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gzhdhfuir.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gqvqinryg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/goieuikgc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gknliatbk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gmyxptprp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gsohucgbn.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gtdwtwpte.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/ggvzxaumh.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gchdvrhdl.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gezfuoehh.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gnozznzwg.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gmdvmigfz.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gdbvcuxww.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gzmrvldnx.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gbvwhnrte.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gublbszyo.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gtgunilri.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/guivbgxnh.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gmghtulkp.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gjgkprmpw.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/ghgrptprg.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gflrklcuq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gpuegcxtj.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gawbkpaep.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gtlkakoge.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gkriswcnu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/ghnuywvvn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/ggryizsgd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gbtzvtpek.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gzvfagqbc.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/grmscqerf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gdhxaqxbz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/guumweddo.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gtzqdofet.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gedhfuxuw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gxtxtbtet.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/guyxvmxwg.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gugqfvtbs.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gwafunaae.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gprgaotra.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/ghicjgakt.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gmewunppg.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gydizymkc.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gdixqznow.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gseapikkr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gklmwmair.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggyprtkts.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/ghptwknwk.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfnguywwi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gosihoblp.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gfknvxkwt.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gviczwglb.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gdoogmfbx.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/ggygewjoj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gzwotvjlc.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gwmjsxnsg.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gbwnowwwq.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gtczrvoqp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gfaeausdl.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gwtkjcevh.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gztpxbzga.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gxygmnzfw.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gdbwylgop.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/grlbbgtcs.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gswcusxjg.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gttmyaree.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gmobdqrkw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gqrdsmeul.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/grgrwwgyp.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gbtxfdqnq.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/ggqldscca.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gcqcepone.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/grwxhxeeo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gmkdairrz.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gdpqojeht.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcgurtwyf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gqwefkbba.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gvtdpserl.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/grnlyamgk.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gngzgodua.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gvmmyqtvm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gihwbbiih.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/ggvuywkof.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gdiqpgpgv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gbawqemhf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gyjhlsmtl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/glcafarbh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gkqnrqrrb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gclllsfge.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gvzloeyka.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gqyqxmrqj.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxmnhnbch.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gfxnpxgpm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gxekddafe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/glqcwxsdz.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gkzukiqgx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gijtgehkq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqmjelbfe.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gywflskvo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzdttnbsv.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/goyhmyphq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gaytfdfot.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gswvzyvye.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gsjmzzgkk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gvpxywbhf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gkmussexf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/ghyfcjjyi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gsqoxfymz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gtutjtpfq.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gowmmycln.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gvbhnrbwk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gexgnukvl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gxdwlsnfy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gqvmebyqi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gblzmdoud.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gnodrcrgv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gfwamueaj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gldmdcxeb.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/ggltaveek.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gcstotrym.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gzuxrkxlx.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gklahwhxa.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/glsefbhoq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gqlrkgafo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gkiebwdey.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/geldiccen.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gutaphikx.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gekulztqy.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gshygfehn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gqexdlwal.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gvoumqper.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gmqzdsddy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gvvrzszce.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gpkxdiiiz.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gwexgdwsy.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gybrtscmx.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gihsuhoqe.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gwjgserzu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gsttfixbi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gyuwwhopz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gbwelvcsh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gzyqcpsul.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gzhigdsvt.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gixdvswkd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/giksavvtw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gxejqfrgt.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gbflpbvpd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gcjwwkwge.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gvdandeoh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gpszhiuil.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/ggporbqhc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnaxydmk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gmopprdmx.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gduvkfqfv.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gamdmvvwh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gerazktkx.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/giolsedzk.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gbetezzwb.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gloedkxtj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gwhukyndm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gqbodksqj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gfigtsvmr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/geplwukzv.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/giqnhajhg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gbxgdmldx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gytcghmad.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gtacosleb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gqwustzuj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gaoobapzk.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gzabcrchs.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gykhrrhrc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/giiahjxsf.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gvlysevju.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/grjnriuci.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gpnvdejqh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gmlhtlfmg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/ggfjwothv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gbmubpvsv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gwfbnvscx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gjpynusbh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/guodaqkaq.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/ggrsjwgmf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/giijjhvzm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/guvjjwyef.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gkibjgsvi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gqznktuim.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gbiujdqsg.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/ggdjqzrfs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gxrjaadfz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ggruotkta.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grckxwxvl.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gfckyneze.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghqooyewm.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/glcdspgkf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gvwspfxwx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/guaghpexo.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gspjydbca.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdyeaigos.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gcmwlqsyq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfayecxki.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gmmculiix.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gitnmtcsc.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gpzdzbflp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gwxjqaunu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/grcjmvhgi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/grcpdlzds.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gvyswtipt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.hesvh.cn/Article/details/gxtfswymo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gzdthlaoo.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gjaczwuko.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gawopbbop.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/graahisqw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gyjgrwixa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/grihgngos.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gppuamusu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gkowihujz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/ghnssgvgs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/gmscjymtt.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gwbgvgywo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gxkgpvetz.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/ggkdipkzi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/gkluzajcu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gpfjnavqn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gxbjbuevc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gyuzugape.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gmdvyhrqo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.hesvh.cn/Article/details/gdsxsxjgr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/gclhmergj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gorhcktrd.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gholirzhc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/ghzkiulzi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/gqqloxijp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gptthrhnp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gffgdabrp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/ggdsbkjcd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/gmbmordkj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gebgpslua.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gigrumwwh.sHtML


<!-- 参考信息 -->