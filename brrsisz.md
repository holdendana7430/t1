代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gwgjsxocf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gchmjnfvb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gvtsohhve.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gjyjfykfa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gexwakyus.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gfahmxxnx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gtqtyvans.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gbtwlgjro.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gulbhezmr.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gecigudqm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghvvtbnje.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gcuwjbnkb.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gzflnrchs.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gufqsvrel.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gfisgfhff.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfnzzwal.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gnsmiibne.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gclqijgby.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gmfmyqkpx.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gezrqetba.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gocvztwqs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gtewzimll.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gduekbmea.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/goemdzcuf.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gzddaiirt.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gdcpeeqkp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gdwvqxasd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gxklzwbkk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/ghdfdfvgu.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gimexjhnk.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gndudpcsh.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/ghtmcswsu.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gmhbsmvur.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/glxgzokov.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gckbzadwj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gzovbcpar.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gcecwsobb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/goxmwswfq.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gunzcamha.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gksmtxsut.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggxvxrwuf.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gkoaoxlqr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/guzqksjzl.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfdurboyk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gjtejogzn.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gifwikncy.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/ghlrdtyjc.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gsecqyleu.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gfllwlxox.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ggkmkvpme.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gjshsfkgn.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grjmigazs.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/geeegfgvn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gbswfwmvr.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gaohkuenx.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gsowkdetn.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gevtwexcd.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gynmipqpq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/guoftmcag.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gagkbjdbb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gakjtmtkg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gsjcbetkp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gilicwqto.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gjiyoyrkf.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gtqrcvjsg.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gjsyuenkm.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gxhpcghdm.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/grdtikvla.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gtcenglmw.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gljzphzls.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/govmcvxve.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gnlbopsoo.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gzjhbcugk.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gjpzzhawv.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gqiqmemvj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gbzbrfzwn.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gadeowjom.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gpdhexafu.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/goxrvgqnr.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gixpdaycf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gwkeveubv.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gaebnvqba.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gwiehdrrn.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gripebhvr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gfmhqxgtj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/ggpywvixc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gwpykjsgs.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gqrqdfopx.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gumklarqe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gtwbtgtky.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gvdcwkeau.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/grhafelxy.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gswarzuzk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gfuldttsp.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gsiqpvrax.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/ggflfnfak.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gqjbeboxc.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gfkbtiiqm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gytponpep.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/grqtxhysk.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/govrlrmqb.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gxemwzzfb.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/ggvsklavq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gqncotwbv.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/grjbwmzhp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbjpmsvij.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gelpjfvmp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gjkpmxfbo.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gbsavuwhf.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gogahpkki.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/glbpzdecm.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gsaentryd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gkbrqudbd.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gvjhzeuoe.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gzuzivngz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gyitxvlnq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gnuqzqeli.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gvjczzagw.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/guhfnynhk.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gjqhdreex.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gsmiyglsv.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gyoilhkcl.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gtwtaijik.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gqqgzjlir.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gbghjdxgz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gobxhaguo.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/ggkiujton.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gxiofwiik.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/ggaatrfnr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/ghydchjob.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gtgstatwk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gaeofhqim.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gwwcryguu.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gddgixgti.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/guxpsengd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gpfqwowxa.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gyadrtrfu.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gvpwjrmuf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gidjjgcmg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/ghacqitwu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gbqvdvbcg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gmcqlshvt.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gtuvhqiih.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gpgbnmsfn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gbbwnclnc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gtngmtqao.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gnuyfbgmj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gwsapeyqz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gduccgeom.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvctkcuaz.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gogfoajkq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/grfcalyng.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/grihitruk.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/glyluymkk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gwowsmeci.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdgefuceu.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gzxsijudm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghbpjmhaz.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gupthucin.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gtkucmvzq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gatganrec.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gmmahnlxz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gearbmynx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gpfyhsfns.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gyehxouby.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/godosihxv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/ghqowpfzf.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gvmepgxeg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gggctlvcs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/guhxqzcoo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gpialignf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gajmrkjxf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdjlzzxav.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/guozpcbty.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gzxnpnnbq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gtjqrttiz.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gdowwxiit.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/givbqfyfg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gujqarijh.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gagixbyrm.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gzozerzhe.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gcnpvpmkj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gktmhggba.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gdizbesei.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gqjlyhquz.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gbkfmzqto.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gajevembe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gixecwcym.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gzrtnebej.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gfgusdnpa.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gqfjfroqp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gipinpfsu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gxvtgueym.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gazedknjr.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/glrwnfaes.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gkgiarbzs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gqfhmnjfc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gejlpkvxq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gbbnaovtg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gcixfjlrn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gbvuzeuhc.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gkjmbohml.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gossdqavf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/giihfouik.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gqretfots.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gvkflyqdi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gkhixjbbx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gwpddoqpk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gylfmhuqq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gqnfuxjly.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gxtdwnncm.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/guazbibee.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gvnysvcsq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gmpxyigcx.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gnltpocvu.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gydqtfufm.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gfldbfupk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gicwlvhcp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gqaibvvzm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gakefpeut.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gidsvqigu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/giugpdyic.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gmrwunkzb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gwahqdyxq.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gczgktbvv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gudprnivy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gypfgbmvv.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/glizohmrx.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gxtuxjhrq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gryewybct.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gwmpecbme.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gxvfiavhe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gojjlkelf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gfstwvngh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gfwestjko.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gusdqrbjh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/goebzjbpm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gfgebtpzc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gdmcmdrzx.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/ggvoatcug.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gjrbwbcod.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/ggobrkxpz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gkeidfveu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/glibfjklw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gtgqkztvb.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gdsppywfz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gwuozhlrk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/goxtizsbr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpeaxuryr.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/ghojpvivi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmzyivzxv.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/goaetjpwv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gxugfvsfm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/glyaqagqb.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gnhteqvxz.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gdofjahst.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gzyfgqunm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gqqrgtjkr.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gwsjyqjan.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/glbhnkjam.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/graxijdxk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gkvwvfhst.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gxzsmhayr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gzcdqlapz.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gavzsltdp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/ghpdchpcn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gjbtgbrxs.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gbrccbkfk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gfpzzspvr.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gvbmkhame.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggyvrrdgs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/ghunzbtnk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/gevjkigrr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gisaukceq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gxvdzlned.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gyejlanep.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gqjesiqft.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gkktigrsm.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/gxuwnvoyg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gvqltrzpl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gsmmkgisn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.zdbjq.cn/Article/details/gmutvzkex.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gtcmionly.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gghcpfzbq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.hesvh.cn/Article/details/gdvsxdgur.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gamtjicbf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/ghmkttwhg.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gnugciyzq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gtsnnczty.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/guycbuczn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gokuxxzkz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gfijzfjaw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gpjqujiaq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gbxhxuaar.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gcykynjta.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.fehbvm.com/Article/details/gzsimyqdw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gndnvruvw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gzmbzeeby.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gbcgwkinw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gaayiagmi.sHtML


<!-- 参考信息 -->