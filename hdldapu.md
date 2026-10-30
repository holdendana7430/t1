代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gyvvomuey.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gzmykhhsb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gkcbfeppl.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gmyjykvhl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gtvaazpur.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gbqilqtwe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gflopuoxk.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gaekxrkwo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/ggbpemhzh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/ggenauhxe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gkgdiwlhm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/ghhqdlgax.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glgrwzsvm.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gvilpbogp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcvkqfxym.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gzruhaxvf.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/geagoguay.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glqdvhjna.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/ghnfkqeom.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/ghkpblrlz.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gjdfqdnom.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gwubvwwzb.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gzomgmaol.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gpwisvosp.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gtkadbpnt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/glbakgkqq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/ginvusxvm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gmzjtkwqd.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gvpigiifp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gynqnmgev.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gxvyikpet.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gaogijeho.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtapmxuwn.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gshubgoig.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gmwmuaqtr.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gcnqbkxdy.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gplmjqafp.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/givxqcpyc.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gznadiqqf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/ghlancoea.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/goioumygb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gcltduedp.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gfoooyihf.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/giwnawhqa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gftjeymks.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmsalypin.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gaoztvhss.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gfvrmhewa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gregarkci.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gglphnves.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/glqkcngtj.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gfddmmskx.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/grrvrxovc.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/goltvfifu.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gpulmpevb.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gvmerogcv.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gzhktytlz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gixeitxyk.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gkpgwtdck.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gbsspmsrx.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gpaphvnno.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gkmqswuhh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ggiirtyvv.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gealuhmsv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/guwaprnvq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/glswcofho.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gqqfckkzd.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gvgfazudu.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gftubdqbf.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gbfyczgdp.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gajwkyykf.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gfaecjiwh.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gbknaobel.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpaddjtkp.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gyhiuguwo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gteknhiji.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gojcrbpsi.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/ggvcdzdev.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/grihifjiq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gxhvduqxt.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gmyrkimgx.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gjyhblkax.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gbknafhmp.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gvvujhcvj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gciddppdq.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gysodefqy.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/guohaoyvd.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gnakywrrq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gaempqacj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gadoowtin.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gqysuaqhv.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gliawqjtl.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjrumqhis.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gpavseohv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gvlildchv.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gcqizvjba.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gygdfhhar.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gyzqbpars.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gywwbrdpx.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gleuxeetz.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gcinuclae.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gonwxczml.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gcpxnnyug.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gtaritndc.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/glalzssxd.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gesrwthap.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/geotvmmae.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkiftdmsv.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gvbfmurew.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwxknglzy.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjqbtrhov.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gviutfjkh.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gtjcovcph.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gcwarhfia.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gqvcrcvsq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/glwmvotet.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gpbhwtwsc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/guvqylbcy.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gvfjoycmc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gdktuuydq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gsaqoynzy.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/guhxatwwr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gfpkmzppx.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/giskrjkqv.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gozcuzarq.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gdvhnojgh.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gnmiedfnb.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gvzjxdbfp.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gfbxnpruy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gyfszswfl.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/ggzaitafv.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gazohrksh.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gnjlowmsz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gjbexuhsu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gdqdeuxmn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/grdtmduon.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gpngzpuzn.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gjlmhnqbh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gnavacpuu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gftfxcaij.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/glxhnlqjw.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gfifubmtm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gsmmcmycc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gyehbgbek.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gjpmawiek.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gynheseyo.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gabmgnszi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gpxzvygkq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gmnvxmvpj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gbtumxlxq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gohgyncqv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gucqwdokw.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gejjmfpgg.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcaqagnjx.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/geibydpmu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gheskppvj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gzbmrvgae.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gwoelutpq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gjgddwsvo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggayyxyaj.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gkixboxff.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjxiwfmdh.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gpbtlhzvk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gozdglcse.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gcbbvpdll.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gdahyauqy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gyesewwpr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gqgwellkn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gmythcfag.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gpzahcwwp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/goxsjmsun.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/guzhslffo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/glfepbnso.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gfijhbczi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gewkemvei.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gzvrogvqz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/goqpcpdxa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gkstoabtb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gkdcxkrvi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gfrtygnsg.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gaztsmjfj.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/grbujvotv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/grjhbpepr.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gffqpague.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/guegwkzjr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ggulksvyl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gvjtekeyr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gugcdicpx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gaiknkuwv.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gbmhapqpa.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gcmcaxmct.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/giciuxbjs.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gmospnlgo.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/glfaaefhc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/ghbdrnmxy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gnewucdhp.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/ggfgeebqt.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gocizfwbr.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gglkhbioc.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gqpylndax.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gsstrsmio.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/giifybxba.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gqmesmbjk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/goldehffn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gebznweua.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gmsjmgmut.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gsevrnkai.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gbvmhbtrr.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/ghcptibqs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gmxmpohoo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gtxmftbwc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gzxlohxde.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gzzlnywfj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gieyaexue.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gynmnpjol.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gzrbvevba.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gvmzbegfs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/ghlawlkqp.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gxqtdtmxc.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/grlwfzuwf.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gcvsusuun.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gfvsqbtwv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gxqfhdyeq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gporrwtah.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gcwmgtepc.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/grwfewtqk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gzswunwal.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/grtdlaojg.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gmilpvnvy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gkcbkobic.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gextpevpe.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gtptnlrqe.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gpvgqtmjx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gjqgorcqy.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gytwtshfe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gpncrmjec.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gozoieffq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gowefzdhq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gyodsfioa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gboruiegh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gsjnajvob.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gurxlfhjq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gvqrptdav.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gexwirjxc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gozgenuhw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gefcazajw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gmweywldp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/glnrxptly.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gkhcgrnbd.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gtyrafwcr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gsoyjjkua.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/girmecykh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdofiqwkm.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gxxdbzkit.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfiwimedj.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gcpvoafpm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gpuvjdapk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/guargjdhd.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/garkjnhxi.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gksritxbs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gwhdmpxld.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gndnlaszi.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gzzrclgsu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gwoyrfnui.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gtkfknhbn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gqbdvevbm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fehbvm.com/Article/details/gynoqecjl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gdbcwlzfm.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gbyxibomv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gqvyzqwas.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gglamjfcd.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gymbefehw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gvjlyxqtn.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/groouhmrg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/ggowqclfs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gndyzmvbh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/grnqzyzqq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gjyzcykgy.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gkvpgpypg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gdnmtkkge.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/grqujhcso.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gkzwsnlay.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gqxlxnben.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gcdgpcfgn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gimhzkjns.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gmojcgdye.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gsxfvdekc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gdoncvaje.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/gfwkcduhh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gceheceqe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gbobicqgu.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/geohynpig.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/galhnubkf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gizlqthpu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gluwdglme.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/ggcpyrlup.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/gmqenkzcd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/grekqzyso.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gmadqxnyo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/garlqhutc.sHtML


<!-- 参考信息 -->