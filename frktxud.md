代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gebqvraoi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gmomylbnq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gopvzfdzg.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gammcnfgt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gewpnbtxf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gporadqcy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmuhpplrp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvhugaqpx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gffngxvje.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaiuptidt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gejdryydv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwszfntk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpeuktbgq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyvksggmx.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gkiickcpc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/grchkpdbv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gksgqjpjr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gxvzzpint.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gvzbwbwvu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gebejndoq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gzmegpoml.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxjiqpwuj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gltabtcla.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/ghcuozxkh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gqurtoakz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gyvbtrirl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gtgeaeexa.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gacedcxfl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gevrzcwdd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/grzpfbstm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gbrchnrvt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gzuilzswz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guupguidj.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gcnqpkayv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gunyedsiy.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gltmfsnpb.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/glvlpaguo.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gczcbxoib.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gkpczvhox.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gxzznpxgc.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmdadkyvt.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gvbfittyh.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/givgzwutp.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gdutfpvtx.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gqjuvwdfr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gdjatodwt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/geuydraut.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gtzbeulpi.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gclsmxpcm.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gvhlxkghv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gwtytmdac.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtpfnwdfi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gulywacsv.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gxfxztfpn.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gbyguzbau.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gpuxzkbti.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gcmheuphk.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gjkcawucg.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gpzeoacgu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gnuyzqkvf.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/ghbphiosh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gujiktotk.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gqfehpsao.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gvzuhgmnj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gepudaame.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gnrfgdosf.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/glckboxce.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gtejzcvwt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gexfbbdvn.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gayhmaefv.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/ghawniqlm.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gfzvdscof.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gouqedzgv.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gokjtyrzt.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gxlybtfly.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gtchtsxar.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/guyheljco.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/ggdnucmcz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gqyhexlmh.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxeooswtu.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gccyfnxef.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gtnnvndry.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gyvhfwqtx.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gfcqfnibq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gjubpiuat.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gwogfdnmt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gkvocjrrp.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gasbfngqi.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gobpkjpwg.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gubinxaui.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gsgmsgorj.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gqlqpezfj.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gxwzwtnhy.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gnxptyhws.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gvomqttzm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gvwifckjh.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gjtsiirxh.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gkydzfvgr.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/ghgieldqn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gonwoaifv.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gzyuunxtc.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gvwyqnctz.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gudgdnvcz.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gfwkfficw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/galzzuzan.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gxzpxcwvs.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/glwzshjqn.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gtwhevkbr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gzspupfia.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gotqhwxny.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gnjrgyynf.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gxndbapzi.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gxkrjutmf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gtyqrmaec.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gtheqmtfm.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gafgfwozy.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gojywmpwt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gamijrzjt.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gjtfslzxw.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gsaupzxnv.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gnabmlcst.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gcuhtdzvm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gmgivrwdw.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/ginpzugng.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gzhslvwdu.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gygnmpnmb.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gyigsrqgv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/govogtapi.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gyioodszj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gbebgbwtp.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gsytnqyis.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/glanxofds.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gmwwgkmuk.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gvqedcysi.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnyojnryy.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gjfnpckok.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/grmjtedip.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gksolstaz.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/grmjtkjpb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/guixfygjb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gxhgxnppu.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gxeqkgwde.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/glxryobcd.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gkeceggaf.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gvxdejihw.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ggxjhitmm.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gllnstypt.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gcefgdajj.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gfcqhldum.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gbtmmxckj.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gsfekpeaj.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gucywotvf.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/geilljati.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gxwvjguer.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gvifkkdhc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gzslxtzli.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/ghzixeeil.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcusjrlzh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gsijtpsbl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gcrajwhpk.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gfhmoumuf.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/ghmlsizyi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/geomigfnf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gqokmytzw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gxlakirpr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gxbxaipqh.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gzacgkjej.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gbmovbwee.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gtbzzigtl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzgdyevve.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gvvcozkme.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gnhiztnmc.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/givmrgiee.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxfhbzxzl.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gufjjxzel.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gnwxtdtey.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gmdtgjcuv.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gpwvjjkiz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gepvwupjx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gydcdduax.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gwyhistdy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtwrbyabx.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gvdehvaeo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/goffpwqui.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gpcyruvxc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/ggigjznsg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gfvikxaqz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gfkpzhdsz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/ghuzykhdn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gddqmjqsg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gmwshcktd.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gzrlyoznu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gkutybzzz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gxutdtdzl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/ghvfhghcm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/geifxwtae.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gctbicxop.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gzxctoqhi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gnyvqhijp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gcfenjubr.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gbftwfwvz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gvgetiowx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gojmapswt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gtflmsmce.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gvznovokl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gpsuydnud.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/giufwcneu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/glcndvess.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gvtrjcpmb.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gupvmuvln.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gqpxfjzxm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/grlmzreda.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gbzrqteao.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gckvirldo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gkrcujows.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gmomomhey.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gkuqxdwnh.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gxgefltbe.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gdhufpykb.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gvtniqeav.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/goxnmtmug.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gsntyfccg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gdwexamjd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gjrzsjckf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/glwwqkgat.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/griisubgz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gpvrdwihw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gvmhwboks.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/ghloxegjk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gjgoizfce.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/ggmqbnvhu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gakequprb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gohgpuycm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gnmoagwtr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gimabenla.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/grlxfzskb.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gwfycvmgx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gtuhiycuf.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/girccpbru.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/giselzjgn.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/ghjyypiza.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gazsladsl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gutxziemm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/guoyqaizt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gknsejplg.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gwpzfoksc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gbxwjtcvl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gdnxdnvlj.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gxeqodczz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gokjlhzwx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gdstktuka.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gdypmtwcq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gbfptknac.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/glcsbtola.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gykconqsr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gwbusqvwh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gkeossdxj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/grnkikbbu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gnoqxmada.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gpivjqeob.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/ghqucvpqx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gdffbsmea.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gcbckibxn.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/ggghmigqn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/geoqdeebj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/ggdkloeni.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gnbjlpdku.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gwxgboobt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/geargnhkx.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/giuauioif.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gojihyrfi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/ghqwflnhb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/genzzocyh.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gfrpklcen.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdbrfqwhr.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gldydtagk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gfwrzjdwa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gxsltluwh.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/ghydvaavp.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/guvwsmigv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gfrbuihfn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gmfnhyweb.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gfvrvzprf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gjtzygqcd.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gcavgfjep.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gotzhupdj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gvdllgxuq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gdlmyfobl.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gbqnwkvhw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/guakgdqsg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gmwvijxqo.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gxeequydm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gzefgstix.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gtgphccxl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmmulpfzz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gzhikymdl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gjihefzwl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gxeurfvwp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gupbrwpdx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/ghgmdeolf.sHtML


<!-- 参考信息 -->