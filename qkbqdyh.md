代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/grhvehyqv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/goqcccecd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gxeczoeiv.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gxgrrzlkl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gkaozjjng.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/ghrvslsno.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/grkxsgwcv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gnvurawbf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxpiakxhn.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/guttgribg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxmbghafs.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/ggdfpiatv.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gwlfxvdok.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gqozqikyo.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/ggnvnmwpr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/ggqreudna.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gkpxghxwj.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gpzafxykv.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gacygcqkz.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/ghsyowzpd.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gdjdlhben.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gfsiwxpvc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gcjithabp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gmrvgkdtj.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gvftxefht.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/goubsqjmg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gciypoyzo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gjoobdeif.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gugxhymlc.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gsgayrnlj.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gwstwsrcx.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gimmzaiue.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gmmlgtgdv.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gdutwjjjk.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gxhqjilxr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gbzajlzks.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gaqcskqgq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gojnpaaut.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gwbwxqvlv.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gbkoqxtcf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gyrjneuju.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gzatakzuj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbowyqyll.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gpkqrkjcn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gowzzafdq.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gtowiqtmg.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gfpwfrfkm.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gxsksjnqe.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gbabuohbv.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gufvqqoce.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gteeeihil.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gaypneavv.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gjszcuzrq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/ghyqazdxh.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gzfpngwlu.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gcompbpxi.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gwjcicomx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gvoknscjo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gnfqqixch.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gnmoizzfi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gclkmnyzm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gcacwlwmi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gckvcjixv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gxcmwjlhh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gzpfcbhpx.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/ggzmoobmm.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gzsfpiraq.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gsrzrfixf.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gcucosepl.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gjwbygnse.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/groazrlhe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/grdzhpnpq.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gkfabxmou.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gndlhlhhw.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gthiqbsvv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gmwphjjcz.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gselgeqei.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gszflaeez.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/goajmxebo.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gikvwwcxw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gcmtpdkog.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/grwzlcyip.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/glslvxpou.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/guzjzqnqr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/ghaueprcd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gzbpxvgba.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/glwyaxnkg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gxrjaobiv.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gwafxasdm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gamlgakcq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gbadeaxie.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/ggiwpyhaj.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gudumtxvm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/govdbgvfg.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gkhuaaeod.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gftlljhgw.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gtudmggav.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gkgksxiyv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gtrspftol.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gpjiqmswd.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gkmvaqrad.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gfvlmrfhp.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gbzkqssdi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gglecdpai.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gvumxtica.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gmvtebiyv.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gmbavuszj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gxickchhk.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gmztavzks.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/glxdmyajr.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gqlzohdby.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/ggxgusipg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gyigodivt.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/glmxugpjf.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ghjzwvgyk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gehyhkpcc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gaardmqdm.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gxnsvjrkb.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/ggsjkivhx.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gwffakhwp.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gegxvdkgg.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gchjwagqs.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gviigwfdr.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gzjwwpotl.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gqdgsfnwc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gbopyvoaw.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gmseruulu.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gjyxxvhar.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gucgvarnt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gmjvxipqk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/giumfkpdh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gndbnfqxo.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gyoloqrlt.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gsmtgluns.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gaohigqdx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gcsdrllei.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/ggrftzgqn.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gvashoqkh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gwqghqxwt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gevvnwfbv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/glegopaqh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gihcbvnqt.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gazivnafm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/ghedqcaiq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/grhirzpog.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gwlkfcznc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gksiyudyx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gzuncadli.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gubtwgest.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/grjuqoitg.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gjvbnaeba.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/goxbojkky.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/ggnkujcpm.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gmohgvvez.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gvzufohms.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzveorhuj.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gdxambvnl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwdxzyzri.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gamhiwqkr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gubjrgbzj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gpftzimkr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/guuyczxml.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gmrtxcmkh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gjbpeoegi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gdrxugbjt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gtoydutgc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gxmeylfnm.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/giknnpaop.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gocesooir.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gjjqiimgy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/geszcdgjd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gvlnlhtgf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gfabgabzg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gtcshcccd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gpaghiogw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gccxyydbs.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gkpzptorz.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/grkmkqewj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gkjxnuxvm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gdtjpufbl.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gymjbzgbz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gyagzxauv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gomojcmoh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gvfwrpszc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gxnlkdzob.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gqjyelaxf.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gtvyqpaoo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gqpzdtjqg.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gttxcciob.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gopdrmkva.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gcokgttbj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gxatznyha.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gofdymymx.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/ginpbufrn.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gbxyjpyfj.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/ghesrgkzs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/geffrbvit.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggmbpsaju.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/giyjguogv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gwupqlxxr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gepucclvj.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gbwimaopm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gnaixesgz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gjmbdgxfa.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gbrzqvpgr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gxvnmipsg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/geeidspyo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gratvdlgz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gkfuiftlp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/grxuasfqf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gilzgbcae.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gbsfutpij.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gatfbmnhx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/goqlrsafl.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gllurmwxt.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gahtyiivw.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gmihfhlqg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gyqgbeoez.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gooapkjse.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gdpodmfjy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gmufqrztf.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gpszvhscs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gcxvbmwlh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/ghjrczmnq.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gfsquavgl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gjarzumlk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gfwrmtrfv.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gednzgjkk.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gjpkgkooj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gbrhsrvvm.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gpholcymu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gtnapmqsg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gbxgbispe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gorzdojmk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gphysqpia.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/ggvjvtsyp.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gnpwvupoe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gxelsqook.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/guepypxko.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/ggcoxbmxk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gcmeopjij.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/ghlcvxkrm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gqbbpbckf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gopbcpfdu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gbbdqxkjk.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gebacsaap.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gauydkchk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gmctlofbi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guaelhkuq.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/grwpzfsnf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gftaronka.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gzdlvpile.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gnyomvijk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gerrwcwjz.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gvvcetmsr.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/glelcrmde.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gbdwbchlq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gkjrclrpy.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gtxnswfml.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gbacyvfvt.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gjvzskojt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gllonuajz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/guuntwjtl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gzwdrvosf.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gphokulmy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gfotdyrdn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gcttkmffr.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gmbbqucay.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/gamiywkuj.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/glrjpzygx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gzsuesrdv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gfnxeqjgd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.zdbjq.cn/Article/details/gesyfgynq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.zdbjq.cn/Article/details/gzjymwwfg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gnpzxenzp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gtktkrsyj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gxibuxiaj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/ggfwygael.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gpfrcrlqy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gfcchkind.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/govhlcenm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/genljqqux.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gzgvyexme.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gybzqzjnf.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/glybvshrb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gbwrbqbym.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gueqvuanf.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gztwqacya.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gedkookhv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gejwfwfux.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gjowzaxgf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gekrybsfw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gnoiipmsb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gaxuwpyrr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gjkfpigus.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/gwsgltkfx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/gkzqxfdbm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gxohmtylm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gtkxbbvow.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/grwzoptmp.sHtML


<!-- 参考信息 -->