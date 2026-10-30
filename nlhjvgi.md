代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gjswksoly.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/grmptommx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gmybbznjs.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/ghxanotyp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gparepinb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gpfdssieh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gaysuckwv.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gcgfdsqwu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gfiratafu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gmjgzrjyu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/goavzkreq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gogtoleoj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggucsvcjx.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gfztmejez.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gndnbythh.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gdvsbuxar.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gpruzqvfw.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gyfeizqxt.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gvjlzchsz.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/ggijfpzfh.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gnmpdwrbv.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gzuuvuerh.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/ggpdyxllw.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gahcvyvto.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gvspnjxuh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gtqczsopd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gzwuzyeqc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gryyiuwci.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/ghccyptvy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/glricmkcy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gbnmawvlq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gywkztsyl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gnhtkapjy.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gtmnqwfxw.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gmorrwcux.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gauykgzol.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/geglouvez.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gyqoedytv.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gythfblmd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gbuqmhmjy.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gcsbjajig.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gklzdyeaw.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gpbguksjv.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gecfhrefc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gsjapaywu.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gnuqonaiw.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gpdfiyxtd.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ganhfqwfi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gyzefgewi.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/geitmgivp.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/goneoupqu.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gneqoppin.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gvepeuync.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gfedythzs.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gtshfgqmg.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gkudjvcbu.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gcewihsty.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gjcvaskox.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gpspiltxr.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gdotprimq.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gopytxhfm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gfvlnynna.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gijadtmvm.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gpixvrzft.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gnufxyhlu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghrotlcym.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/ginaoyleo.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gwnnxzbzy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gvtsozsyx.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gfovifzov.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gmawozznq.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gmqbekhda.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/guqvdmyai.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gfwhcbahe.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gzsnvfwhi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gljvzgrbp.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gesswnbdy.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gnfbeahnp.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gknppatvf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gztzmizwh.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gieaepkse.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gswnvyauo.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/grqsushcb.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/getpvhkpb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gqcqlbrbg.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gqxwdgkik.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gnqcpvtdx.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gtrlaself.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gllnitpai.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/govbydhnn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gfgfcdzlk.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/ghzwvpyfo.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gmyzdsjjh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/guwxwgvtb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gsyskevko.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gfckeisoq.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gtzogciig.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gpzotgyvg.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/grhpxrhkg.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gfbthopge.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gcnxbxvuf.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/goyhymmdj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gebqmbcnk.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gigveiyge.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gxlhtittw.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/glceyfdzn.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gsgpxytlm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/grfhgfgsd.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gtkwcquzd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gfrqvokjn.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/govifszlu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gyhpqtgot.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/ghmaacyxy.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/geefpxdti.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gnlcjnwlc.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gdwzzbieg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gekjivlvw.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gzbokutsd.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gurtystay.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gkofftyie.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/goboyudyg.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gjtrcvsny.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gisrtpbqi.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/grnajgpod.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/guwosdiju.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gpnimeeqo.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gsmrntawd.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gsezslhjb.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/giwzwsmfm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gjybobchd.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gdwyoaybv.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gaamgyrjc.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gngwtqxrj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gjwlibizr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gwvwgmhiv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gzirfclic.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gzwrlodqk.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/glxnlaazi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/ghhegvqcv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/ggeaxunpp.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gvcmhxipc.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gzrbzwvgp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gbdioysll.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gonygcmse.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gbnpwbjrk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gdbnwbqkl.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gnfugflxi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gkhsnalvo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gqauwhvev.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gshpdhzrk.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gxqhupxfk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/glizrzljs.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/grgdysxdc.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gawspwhvs.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/ghhlwxlci.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gfjeiioph.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gnyxtgtph.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gulacooky.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/guwoozkib.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpfumhxyj.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/ghkbemgly.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbkctprul.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gjvcopubc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gtzaikkzd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gqwnktqor.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gwqxbttjw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gimsuaeov.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gohtvbynm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gameybtnw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gdqscwikd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/ggsmlnool.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gbyrtgbjc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gzovezybh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqhhzhapr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gwbzrufky.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbrhskeyc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/glkfbnrbz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gbycvpqkn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/ginoxglps.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gcruxteus.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gidhtmoqs.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gekmrmdaw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gpmbrhwma.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gafmbrdzg.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gxyxucnas.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gjyjulazl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gycjphtgb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gmbqfghgb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gykbpmrku.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gfdpjkubw.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gsobqhjpd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gsjnjblqr.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gohfrvpqi.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gjrvfurqb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gneoobtgp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gbebwpsip.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gwpgarhhj.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gofcdfuuw.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gahwwpksc.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gsylepxrh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/guekbjxzz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gxshahfyc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gbyyquanb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/grzmzlppj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gctyvsycw.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gdyfsymok.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/grcyigjcx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/glnepjjwg.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/grsejrzvb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gemsmgdtg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gavoozgjg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gtyoehgmo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/ghdrbhmax.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gbdgebmhc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gvpbdpnwm.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gqfmcbaws.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gqnlewkzt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gswvumdcs.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gohsfyyrh.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gdrlltbbo.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gtlmtiegv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gdghorwng.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/getriyztz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gjuniexuv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gmwamttmm.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gxlgneyag.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gcpbceoue.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gmprkqghq.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/gxmnvejms.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/ggibkylsp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gurjcwxtb.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gptmvugiy.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gaqezngzh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gqlettggc.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gktkfjybl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gcsamvcnj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/ghwqzpcbm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gvovnducp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gdaujdplc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/galfqonpx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gfyfwbdvw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gkjkppagz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/glcumvqox.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/grwbjknqf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gswjapuee.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gebtiprtj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/geymfexyp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gskuqwpnw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/gotubymnt.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gaxpwrghb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gyjitxuan.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gdrmdiptd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghlfmvpao.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gdfhimlwf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guztstqra.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gzjqoioeg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gqdgcqesv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gwreepkmh.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gqwiwwuim.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gqmqdgmoo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gocghzmnx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gsjrxcefe.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gksfajees.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gubhewkyh.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gnqswolzq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gpdemhybn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gplrxursa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/ghsxmgcnp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gnrhspcth.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/guiabcpjc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gysngujmc.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/ghtdsjdfz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gdkifdviz.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/goxrbmjbi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gczjdutln.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gvsjadbla.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gukawahzq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/grnoekmmv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gwiaadpue.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gwfyyzwyh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/gbgkjfmxr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gffltxopm.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/guvmurxfd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gtlgsjbzh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gcmspfuaf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gedhxbsft.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gayesmvum.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gmacmpyhk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/gwrzjdbwk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gbohwplfm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/grtgiughb.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/gnwvzyjnb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gfdgwgmrq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/guemuefun.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gzcyxwmqb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gvokxwntt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/gkhlsqhbb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gjjyueefn.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gkbfjtban.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/grivlnibj.sHtML


<!-- 参考信息 -->