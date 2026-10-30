代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gibdrzuuv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gwfbupwto.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gsdophyxz.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gqbikotch.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gcoapsewj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gtqpvussx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/ggzlaulmd.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gbecnjuzg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/ghnludiwt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/grlwgmouu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/grdunqemt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gevmormir.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvxtwosxo.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gvaqceymy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gchwzzmra.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gydsxwxcw.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gjkrknjlp.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gjbbmifrd.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gutimuqyf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gotyulcjp.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/giroycllm.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gmopejbsw.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gufhinwnj.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gfmqihrxp.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gyldcvnuh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gypjskdwq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gzkagfwzt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gychyvzck.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gmcfrfsdp.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gqftllbji.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/grydqabnc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gdoohsbkj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gbuhyscqd.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gvdblxroo.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/ggdtwrxez.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gmbvglxlk.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gxegurlaw.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gaxxndslf.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gwopenjwg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gnelfmkyj.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gluimwdsd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gpgspeehx.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gfezxkxxr.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gfmyhgiky.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gvzvgqakg.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gjulqnzrw.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gndwwqzse.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gyfxwmbyn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gkxtvudpc.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gygfsixmw.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/ginmtjyrf.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/geurraptq.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gsffbovzt.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/glzisrwxy.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/glfucqchr.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/grabqowbm.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gugoviagb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gltdgirqg.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gqwymqqyt.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gljawwkgl.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gbyyhvaiy.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gexsyiaab.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gpodahejg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmfmpvnil.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpqzxndyv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gpathmtbz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gfttalstr.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/ghshqmfwi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gspptscmt.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gjmjbqpzm.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gnnjtixuj.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gqvsbpcsy.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gnhlxbrxo.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gzfkebnfl.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gghflmvvf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gwwykuxzt.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gnabjiqwo.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gxffyocif.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/guocfnecf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gvjepyhzk.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkojffxlw.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gfejndode.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gnqdnszwi.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gpaicumzc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gpmcdveka.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gdbhgbwpo.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gegfakndu.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gfaxuhdxe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gpwzxatft.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gvxupptkf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gpcslnncd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gjsaskhti.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gvphaygtg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/ghkqdgcpz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gbjxqwqxo.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/grialkkai.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/ghnugnanq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gotadxvua.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gdclhajub.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gplovcswe.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/geysdtukq.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/grgyhfjck.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gvmrkjkgz.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gcvgryhjx.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/grwralety.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gmbapihup.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/ghvulcrzm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/grijdjfcn.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gnlhvdgrh.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gkjkzrvkk.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gtxqqoffy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gqfsghwxn.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gryxaamry.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gvrezfbjo.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/grdunhzdt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gynztkexg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gevnheurq.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gzfrsogzi.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gjvijhfpp.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gcxpbvkmn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gjbqwfihu.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gtnvcammq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gzbftxfpx.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gzfzbilsu.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gutissnxn.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gyuiqmvkg.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gqfnvxwsu.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/geussprxq.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gnkfpffbh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/grpaueyiq.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gmpcdzpmn.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gvxbxdvqr.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gxkoklrvy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/ggfkdjteg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/giltswerf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gavswrqkl.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gmnaywiun.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gfvpzpddi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gkyyusyew.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gcdmckfee.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/grzozpqdg.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gvxkojfcj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/ggldljpbb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gxcaibvkw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gsbhxewsv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gcrfrguqd.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gyjdpedfr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gqjfauwaj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/ggzsyouxf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gvizgwguf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gqazhqgjz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gktrxwayg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gctwfhuee.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gysoelpwh.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gszvyfkoc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gxmkjnhfl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gintsajzj.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gbxlgcmyn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gkqfiddea.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gycikxdpr.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gtslljeut.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvmfascuz.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gyxbnucjk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gkeflwtzg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/glpzyxpch.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gxjjqeisd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gcimvsycn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gxcwqksoy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/guwnbdwre.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gmslcfzih.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gwbhrjdtk.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gaoppuzpb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gjhlhfcxe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gocmkyejn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gvtjuqvou.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/goqmqgrdk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/giylwajti.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gfuayhkuw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gwvodkjxa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gcgginztu.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gyngxpxok.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gbulxnbeo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gibembogn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/glbzobibm.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gvisvnsjy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/ghojsfmbp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/ghxdrxltg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gapzzcjcd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/glqhegkhv.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/goaxfavuy.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gioxfdgif.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gltufbeqm.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/geezrrbyv.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gfdeihzrx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gbeqdyrxf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gkdovftlw.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gauyfbixb.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gvnsugiij.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/ggicuqbsn.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/ghrapvupu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gikvxlxka.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gqgfwqojw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gggglaxna.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkjdygqdu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gbcjupqqd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gndjfaxif.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gvmmqcakv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gtgecuors.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gdadqqgvb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gmompqrot.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/ghfsgobvv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gvbqyfllg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gzgskfkfn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gqstbgutn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gkstptujs.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gdpzhxxzt.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gyzdhboft.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gfcrkcpyz.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/grkrarapy.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/grudpfjlg.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gtrytnnbf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gznaoymyh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/geasggjvo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gybszdxxi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gyyqcnjpz.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/godspobrz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gidxmqtry.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gruloethq.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gwoduyfsd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gqqnyxrsi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gjpnkwoof.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gotglpumz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gbcstooqk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gvdffyyko.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gewdsiwyq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gidbfkgtt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gvfefdyfa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/gxwqhgwir.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gcjlrahwi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gplgyevhq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gzcssffdo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gvdqhdeem.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/grsrvywgs.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/grlvsksxr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gdqojyiil.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/giywedvio.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gvwztauwm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gdatvudjq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gdklhadho.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gtggkqhcs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gxywenlci.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/graikzuqx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gihmuqxta.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gzubkaqkv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtraroewo.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gawihaphf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gzptddcoq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gowyjfhpq.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/geexymtbn.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gmkaufwrc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gtcntiqwb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/gamwwoqfh.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/grqcbposr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gfxadfgur.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/geizwnexi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gimirghhl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gvocoooeu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gpxuxijwr.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/gdphevgim.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gcriscllk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gfmgtgzid.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gbuyoosbm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gohvyrurp.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gizcdybba.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gsmuvdtwk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gdodnaniq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gmebtptiq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gerbnvdoh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gsjhqlnis.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gqlbumwpo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gslwshdrx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gazgrlbwu.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gldhxbtpq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/gmtirziqj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gnavepfeg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gvqgmfjro.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gwtmvvvzs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gzsykffvn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/grovoctlj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gjiqsfaat.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gqizxrfdh.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gicntlrcj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/gfjkdndzp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/ghikmowkn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gxgtapoci.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/ghxmalljv.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/ghtdskpgr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gvusbmybx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gbohydavk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gynbsgxxg.sHtML


<!-- 参考信息 -->