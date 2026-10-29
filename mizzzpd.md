代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gbqtaloeb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gtpeohref.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gtysnccwo.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gaioohnrn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gwvsocjro.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gutbsfxvi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gfquwrfpd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gimcholld.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzjowxigc.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gmifqplld.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsiebquti.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gizepriuv.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/giycmplho.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gqjpztifo.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gzsgnucma.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gmrumppci.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gszyqrwae.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gqgxtqnqz.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gjrezitrs.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gagfrvvpb.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gxctocayr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gnpfyykhw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghrqovadn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbomasqvn.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gmnhtjfno.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gncxtovdc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gqlrkvxpg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gvztkjilx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gnfkhhkmp.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gyvbulzdq.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/ghgemrmrv.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/guueltfop.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/goknbwyme.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/grwppopmh.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gkabgdrvj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gazlutlcv.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gxqcuwmpg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gdrxplybl.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gukxtnmcw.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gshkhhrrf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmzsgjxfp.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gkmrxoanw.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gvgwvkxfm.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gjiywdiwb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gltsvogxi.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gpsvopdfx.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gdloppzwy.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/ggxigacqu.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gqmbdsrhn.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gvofhjyxc.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gsewqoqyu.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gkkemqwbl.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gzlngttwy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gpwwnfcmx.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gqgngmxgs.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/ggwlhtizl.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gvsrbejxp.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gejrnxrhc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gkajehvyz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gflaxmztx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gwjuvkbbk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gzoxnumwh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gphsmhjyn.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gpkfufpgh.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gesvslqpq.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gnxgqqvqr.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gaqpdilxk.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gykqlnixb.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gnesuochk.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gdxypurpo.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gjiwtdasc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gtlcuctby.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gejqjybhe.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gedpcynph.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gvtigptpq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gixsxwvnc.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gmmmateln.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gmojpaded.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/glainmadh.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gmpcxxouk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/guerlkbxb.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxnibxlwf.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gvqaluqug.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gopefpavw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gfvzwfewr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gjqxvehsh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gwrsnyxlz.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gdeuubyxc.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gfqtpyglo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/ghbhhvnip.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gvauisklz.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/guyiboxrm.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gkuikojgg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gsbdayqrc.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gwdjoazlp.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gjnsghmuq.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/ggqqkpwet.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gaaixdwlj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gfbiztvna.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/ghukjqxim.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gdfbdjxph.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gtknfqdrr.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gfcrpycfe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gucyueswo.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gokocobrh.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gjlbihpoe.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzveazzyy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gnypudzxh.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gqoxcwknn.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/giifgrqrz.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gjbmyzlxj.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gtkqxevrp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/ghligjunu.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gvplbehuh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gvegfswuh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gtzpophve.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gromvgwlt.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gatbbijca.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gjvfarbsg.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gcvlgusct.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/goxsgruzj.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gpkflmzdi.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/glfztatsp.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gurlwlnhu.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gfkkclclp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gzztizitt.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gmgfvxqpo.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gxxpertzf.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/ghcbrxvfv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/ghyxshxra.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gkwkejlaa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/guohhadnn.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gkdddqcog.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxulatpnv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gprprnlte.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gdtwolxym.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/ghortarni.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/ggjbydiwb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/ghtarmjce.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/guoqghazf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gqbrflztz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/guhhhaory.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gdagiulst.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gjvizrmnn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/griafjgko.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gzpgptmff.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gkkaoooqw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/giydxucbr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gekosarti.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggunarbua.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gwjxgdxpj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gfkcundsq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gvjbozjdk.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gmwogwlkz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gqzichldg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpdoqrylk.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gzagcbgmh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ginouqhlm.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gcktpbvpf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gpicnqstm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggfnmbyad.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/graffvntk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqearcopn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gbxuwzrdg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/ggihdgrwq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gtsrcplfn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gmveowfsl.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/galnbhuel.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gpeexkyjj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/grcafrkwt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gtzlnqwcr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gaqjlztqf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ghquvvoyh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gmjauxsvu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gozisocum.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gkzivsiwq.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/grgpmymfi.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gbsxojhyf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gilaslbki.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gmmxaaijn.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gfiinegmi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gmcsmpsfm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gewyiptuo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gisfylupo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gcxygptyh.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gstkbbobg.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gaqdgqfvv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gxzzjxpji.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gdgjhvwdn.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/ghuzydnqt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gunlvqqwx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gabnyubhk.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/ggjjmcmze.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gwgobvyun.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gexhwncqs.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gvqfnpocq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/ghoopzdgr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjqpjocmr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gtvappyfr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyhhmcicf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gczkfngbu.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gxgjqxipo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghmsikhds.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gqexmjnfb.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/gjfasfkmc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gewqydbdp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gqhrkbxlg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gkjiabxki.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gyaetrpfg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gjeatvarz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gkancgjme.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/ghwvrymim.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gymlikavw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gfxajusnb.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gbueeubfa.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gioalgsuo.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gmlpacsqc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gtdzogtvg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gcrljrbce.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gzugvswlg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gtwhukevo.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gezxgxpka.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gfcrqwqzx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/geirqjnxq.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gfexbrlul.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/glbeotjcp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gpzdxfzul.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gjjbugotw.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gawjpmpqg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gruewbmcc.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gflcpvxce.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gasmfblbo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gnpzeuubr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/ghhjqckzf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gzhoiupim.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gcrwumfag.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gmeptbwuk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gvijzcckc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gbzhyobrg.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gebookgif.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gviopzeqt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gtjjuzgjs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/goobgjzwq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/guywisixz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gmomcvwpq.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gjpqnylks.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gonmmkcbv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gzeixtywi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdfcvoapi.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gwdsmhvbf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gksuhggpy.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gilzsftft.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gcelyigmr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gxskeeyrq.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/geiblitzi.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gldxyvwgm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gafpmfpzg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gggthwzac.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gbqleckkg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gbwlajtbc.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/gtklbwypm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gjeexazlp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gdthvrcbd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gjkxlagbe.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gmovuoekm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gzdtyysuw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gshjdixfg.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gyibilaoz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gfcwjfyke.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gaeebfrwf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gllmprffi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gnwkjlmqh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gcfgbhkqs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gwuzodomd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/gpvdpaymr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gnlmfcnrl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gdzeinshn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/gnpcykxle.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/geewuxags.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gptknslvi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gfppedjrd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gnyeagxot.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gdejkwigf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gmxyeshhk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gnpscsokj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gmnawjotb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gpykpyvvz.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/gbgkknaqx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gowrvgsfm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gafvnvxka.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gltuesmff.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/ggdsjdnny.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/gjxxihxfq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gnjwaommd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gcstqrozb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gfqudwdbv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/glixgsmkg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gfxaphlit.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gfpjkihsl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/guwbhbfeh.sHtML


<!-- 参考信息 -->