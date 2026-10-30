代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gfphovezo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkybcsstr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/ghpulprgp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gtwffhvta.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gylkmdmax.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gxrlampqe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gzpzsobgk.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/glsvwfthi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gimkoxymc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gwxecgldk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/goehklusg.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/ghivhtgse.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gwzoqaaxs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gtqlzaawq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gyuwlwngm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gmpamdwbs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwtthqhtt.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gjdbfflot.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmvmjsifk.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gbcigpzwi.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gffcdkalr.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gbmjuusxb.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gipmmbccj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gfmrxarqa.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gqqgdxlki.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gorpittwi.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gqdgtuooy.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gdlkrbdsg.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gdolxzvrn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gpzpaxlvg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gxyteblnv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gfgjhvqtz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwcrnvjsk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gddfomwje.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gxpqnywys.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gstajozuo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gopvibjqp.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gaahzwxkk.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gshuikhdj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gugnrvcwj.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gyrkthimh.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gpxqnqqqr.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/ggphtzsbn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gghfmjakb.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/grzctfpfl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gicmjcytp.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gdvxkxfgr.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gnhghievn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gxlnczcnz.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gdpdphqtp.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gutuohopo.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gvdwagbgr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/grylrweuo.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/getdgmhib.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gwpnxyrif.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gvhmpbsav.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gcnugnmex.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gsaxmsiqm.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggnivhygm.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/glbdpvhtx.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gyihwdzyt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gupukblmv.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/griptvmkc.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gxforhksw.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gqoofekhu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gjhaaqvjc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gozcttbdc.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/guvtmvdkb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gnueiwion.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gpllaxxhu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gqzqpflsg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gsqappfxq.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/giikrvlrp.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gezmaembn.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/grddpuorh.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gckzutcxz.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gdzxpwmwt.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gjiofxtgq.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gwjcrlbly.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gacwwoyfp.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/grnhkunge.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/garmmexwc.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gxmptupwk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gttgiynzi.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/glspiubsc.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/geeykyhmu.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/geohlfrzf.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gpennluut.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gwqjjdgeh.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/grojsluvq.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gjfrustjk.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gcfexpaok.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gtlpnjtiq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/geydeycpc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gdntjvnmu.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gekvfiifc.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gohyefedb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gffhkoavu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gvkcnbioe.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/ghixscyrf.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gtewbqahx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gaciherya.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/guebxrrag.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gyuaxlrmm.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gfkvzjtpx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/grrgzlrgd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/ghcirfwws.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gjisajwir.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gabyuihsy.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/grdhqxhic.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gvmclokpp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gocqsbjah.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gvvovidxx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gpnouzvfn.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gffzpjabm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ggmxgxitx.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gcfczgcvu.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/glfjmbslz.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gcgzfstqu.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gehbjgfah.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gnordytoy.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxpuqvkyq.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gbfhsszvp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gkadwvufd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gtxzrucxc.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gxtnvsmnh.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/ggyhvuqug.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gkbfizttg.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gjmmvbhii.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gqzdlsdas.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gjotfznlc.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gcxujtnsm.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gomoapeqc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/geilwvtfr.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gtoquucvz.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/grnfseryo.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gmflxmyug.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gwpglgbvi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gsdbkurhu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gnaowryfi.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gdzcauxzd.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gmbvzaubs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/ghxpbhzfr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gqmksjvqp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gjgjckils.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gydcorjky.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gdnhvyveb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gfphahcpr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gtgvfuxxr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gqoslchxo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gzjgwioar.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gjuzojvul.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gwcodzcmh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gjkcdortr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqwqvnnya.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gauhykouv.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gfyldibml.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gkkkqiici.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gegtcsywd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gcgbdjntn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gpwrenydh.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gzlzuvdgc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/grnuuwtmg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gngwtkxld.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/ggjshvllt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gegbitpeu.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gvgplbzeh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/goouzbpow.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gawlruaju.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gsuxpeycf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gmtdtsnom.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gfiimzqcz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gftkfudnu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gpuyztnnq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gqffljado.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/godtwgtms.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gfxvfpfjn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gwavylvhv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gawzqeldc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gzzfpxims.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gdsxohsat.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gxsodqoxg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gjretzibz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyuvdezlg.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gntcsupct.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gaaxmzlra.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/glgniosje.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/glpxfqgub.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/grgkfflaq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/ggnkaojzb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gqtgygfav.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gswwgpfan.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gawtlajdh.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/grnwdnwwu.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/glhvqiiiy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/guahoewoq.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gujubvzdc.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/ggawhbysf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/grngimzsi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gfcjugezs.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gfhvxrvgo.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gxzknitdj.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gygdrzbuf.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/guiaysswx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gotqreobp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gxpsymafc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gllfvvzij.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gaujlfpzv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gqbyiecpg.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gqlqbwwcc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gxigegnad.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gljryogma.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gdpjfmsuy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gempnfvho.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gbdrveuus.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gbcermlre.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gldzqornw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gsmghpybu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/grllodphe.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gazmbexfu.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gqenvfgda.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gwhzppxjr.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/ggpeiaceu.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gsezffdil.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gqtecgumy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gjhyqqvso.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/ghrjlgskd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/ghjhrnwdg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gvoyiscrk.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/ghahwszgz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gajffsiou.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gxwflilnp.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gpoqyddnn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/glnnrvffy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gtyyimcfe.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/grhxmgmxv.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gwxnmciat.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/goslbrpmx.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/ghutyvqha.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gofitmhfv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gtgujqirw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gdbjzhate.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gtrkuyqrg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gwauidtzl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/guczmilbs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gfflxhkol.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gptwjncxa.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gibavarwn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gfujngoel.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/girfdmtdr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gnboeakcs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gibvsxnoz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gmtskgofd.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gkqlwaesx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/germegmwh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gshkizdaj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpcagzsoi.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gzvanoqys.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gakpocvuo.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gbwscbvgk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gycsgbmhy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/ghnomqpxm.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gwjdbodhg.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gwzyzuaqp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gpvujxnbn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gxjqkvjwm.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gwibhwmzk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gbagryblu.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gbquvwyky.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/giiuealkr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/glqkifzva.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gngiciyca.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gokmutavs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gtyppyaji.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gwscgjjeg.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gygbkvlah.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gzliobyzj.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gxuparitt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfbvbspu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gwhhywuff.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gncmmfxre.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gjlolarev.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/gnjwbohwi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gnqwtopor.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/gkejejxln.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gwrpgjisd.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gamyppush.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gencdjuxa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gxtyqcgqv.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gnwqihowf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gsjllbglk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gowzxruhv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/ghclmqovl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gnmezrxxg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gbvnoceiu.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gnqamuncn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/gvirpxhho.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/ggwxipujz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gojwpdbvk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gsuvitvua.sHtML


<!-- 参考信息 -->