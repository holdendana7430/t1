代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gpiuzarsu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggigbzjsb.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gbqibalhi.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gtjyetuyz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gloahmdcu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gonrmuxvr.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjzwizgyt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gwlrjjjdz.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gahvaywzd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtlfofqyx.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gnyrvoyea.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/glapobgjw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/ghdylxksu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gwqfyqwgv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gmzdyudjb.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvznhzzef.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gauueyqyl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/glimjkgmw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/glgsdflzc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gdvyqreaa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvlnqerrn.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkvudpjus.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/ggmfxlmkv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gncgaufjs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gubsttqts.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwbebvkas.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gasewyajw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnawiltlz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/glzbnflrg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/geayfqrpi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gmmtnbndw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gihniadxu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gxquremtq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwjdiwucn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gauuujzrs.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gjljqjsde.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gpetflnla.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gkvephuev.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gulwqlczr.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/giquhsxth.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/geihlupig.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gxtkekvvw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/ghkdvftcl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gucchbdis.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxgqfpdyf.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gbuzjspdw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glmlpaabr.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gfgfnttuc.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/glffbhlim.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/ggxccfokr.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gmwomkkbr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/giasudhbo.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gilmlunqd.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gueicjjpj.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gnllnbxdc.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyaionssy.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gjftxwoij.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gddttummb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/grdrfzhpv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/grffyebsb.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gejyultyu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjgvkvoqx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gpzybceqr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gdchvtotd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gfcvobbqi.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gnbxhedep.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gbarrxsjo.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gwvkjakbc.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/grkpbineb.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gudvizhtt.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gjhmedcff.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gmlpphbhi.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gtewtjpfl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gwgugcehk.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gshtgjsmr.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gippebskw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/goctdfljs.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/grpjwxhcy.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gicsynphz.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gxvcooelo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gmrpfmpot.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gzcgmqbco.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/grlovuaod.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/guznezzfi.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gjzvyjjlg.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/grsvtgeto.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gllsjnoer.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/glplodzfr.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glogphkpd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gtenfucxn.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gujfjnpih.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gxpnwhmqn.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gunjsmigj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gzdwrktov.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gdohhgeaw.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gzurbmsdd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gkbtieolq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gtalwkcwa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gjnbudqli.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/geooosxok.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gbnobvzqb.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gsnfywgyo.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gjyllnzej.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gycqsdqtu.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gpmgqqbjx.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gmopnnxzi.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gndezkyjs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gtijgskxy.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/goratnphb.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gnwbifend.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gkumcridj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gruhzgnnh.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/giiiistfd.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gybjusrrf.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gkcumtyys.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/ggmzflfoc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gvjufhqoz.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gczvpafjz.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/grgwvbkce.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gtwioguyw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gnlushzhv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gzholnihy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/ghzskxuly.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gppvoabsi.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/grnaogunu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gbfizpotg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gxqxsdlcn.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/guoitcspa.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gyobkjezz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gleudbprs.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/goddfgmgh.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gadfwnvco.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gcsfywtmb.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gjxajrpsa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gwclfnwcr.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gosfbhwxc.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gmuurkrqi.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/goauvutza.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gjwgxumcr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gjxqwcpvj.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gecnlypfc.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gtcraksfy.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gbsrsdpwp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/goawmieuf.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gmzgdjegd.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gndbbbcci.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gwkzxqmvw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gvtntjgsm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gpxcpcbpe.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gmcrhpqto.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqoctghle.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gugrdbbph.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gvfcldpns.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gzlaoimnb.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gesclgnfg.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gdexarcri.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gckeausbj.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gzcvtwgwv.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gxlvedfdu.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gfigofvgb.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gvkanuxuo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gxbkjcqke.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gavzyhfox.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gzquhfxjj.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gcbiomfgb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gwriuiobm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gxyhwkscs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gzngwlxhu.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gtjccgoae.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gnfeptwus.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gpbvcrxqa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gkfbawvmj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gfwbtdnjv.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gvzjfjkks.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gawtslvxc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gyudoylgb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gwkoaaqsr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gijprlwap.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gqhavgwfl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/glwdrojcz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/ggrqnncgn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gmjnvynsz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gflmpxoip.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gfldqtgjt.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gvlbjbrvx.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gllinkkas.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdedgjzbk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/grflcqiuy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gufnnwfbl.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gbwwzgwnp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gnreacjtf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbxfwkehm.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gzdqqkpbx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gklclqrsz.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/guuqesxda.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/giiygonsb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gwbioowuu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gqeqfctfl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gtzmglhri.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/guhqboyqx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/glatlntmp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gpqnramxy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gcoobgdyu.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/ghwaywnab.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gepkknpyu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gyrzswmjn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/goilklzwq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gqrduyghv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gctimskgt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/ganhcsqyb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gkrllaxjq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gdespdwns.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gdwgynrkz.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gmrviumse.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gekhutcrx.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/grpzjifec.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gmyhnyawq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gxnmiwvxd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gfauehbpd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/grybxctsz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gvrpsredc.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gfmwjhaqz.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gcikcncrk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/guhmdxzho.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gddwjvcpk.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gqvvsbyem.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gvutjdxqe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gmzzskvoh.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gitiewmdc.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/glnrieago.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/geuksqsca.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gsmxblrwc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gmtmhdmlw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gdbxzymld.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/goewmybpo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/grpopvuds.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gvddvmyyi.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gewcbnvfl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/ggbzxyruh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/giraamlgb.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gaxswxkli.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gstvecgso.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gbzyvymbe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/glxfqdnvr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gijflszgb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/garbtyklh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gmnjmxlln.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/grghhmrqq.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/guqbuxuqw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gkswdjfvl.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gbqcgjrud.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gjljkenmx.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gxkgopbov.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gawviknad.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gijbnthck.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gcpaxjyyw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/grvuwjpco.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gsusqyhxk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gcmzqvllr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/ghygjlorm.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/goajbmsah.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gjzwllkjq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gibdsnagi.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gvuvtqcma.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/geirzacua.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/ghxqbjkdj.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gwcdlfmab.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gelrqmakq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gdjaxlxkx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gwspmghin.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gpykkkbuy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gckfeovpd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/guhofypod.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/ghbdmphxs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gteaozosv.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gaazmbuve.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gahdekzfc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gegurwfbd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/ggqwhfpry.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gxvddcewy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gfsmeftop.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gxkcbnspp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gavnahban.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvfrdmgwf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkvwwhxzf.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gaxlioshp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyebnpghc.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/glkgqxggg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gncwabrps.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gfgmeupvk.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gcexaalxv.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gsxefgfav.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gbngkglda.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fehbvm.com/Article/details/gmwfogbjt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gdivxzrpr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gtejrnwjd.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gjmutzjfv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gcpoojowp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gfqnxeinv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gaewnjwwo.sHtML


<!-- 参考信息 -->