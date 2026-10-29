代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gwfhcqrbc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gspqxsuze.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gqjwbnncd.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gpvdvyfue.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gtmewpvst.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gmbeddiwl.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gvmgycbdj.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/ghyklaivh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gqcoprsjz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gwobzqxvq.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gkbxcazsi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gektmhzaa.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gmgsrggqm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gupyuzslb.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ggfoggbih.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gxjqwscka.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gnzkknamv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gjhwybfxm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gsehmnydr.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjyxwwqqc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/guytuifut.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gfiywxcis.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gjoqykzvm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/grbaegoel.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gttihovnv.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjlpazavv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gcwjgyaqm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwhkrlknh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grrvymjfz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gfkrxjpla.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gavysyzsm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxhjnlgrk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gujetfjvi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqexgumbw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gxyrfiddd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gbzidrgtn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gqvflqpde.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gxuapgndf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gjksqjlal.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gncutjzas.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gxltpnnqv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gawrumoqn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gyfkodwrj.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gcclfhumg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/goaivsjbs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/givbnmzzb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gifkxzikb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gqrydapug.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzfarrwee.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gurrllbnl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjgvpiptm.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/guddaaxny.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/goethqlev.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqfrsitol.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gpaxlrenq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdibvqwa.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gmfyeyjaf.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gcsljdntr.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gxmvumnqt.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gteophanf.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gozqkgbsj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gvoefrcfz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gesqzcagq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gxfxipxbi.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gojbqmjhv.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/giigmcmjc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gdyvmvrwq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gbggkbnfe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/glfhxqrzk.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gwmssddso.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gvprgnuzq.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/guyzejmtz.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gdenaoqsx.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gglmxkyoq.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gqeyaredl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gmscwkmcv.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gnccztlyx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gccnvdbbx.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gagvgdiui.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gemcsdtxn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gvglkljtk.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbrdhnohj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqurzdjvx.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gqcvtzvdx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/geaonvoxl.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gfzyzhwvz.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gknzqpyef.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gnfpjzwmg.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gvqppiamg.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gfostljky.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gpotdwgka.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ggyxalbch.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdejrihyc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gzvhiobsy.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gmiljukwp.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gpwmdvrvs.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gwbyigyff.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gjkjmzvar.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gmjfrqlfs.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gnbdcrhdr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/grilxywdm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gcjnopgbi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/giwmkjqac.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gzvftdwjr.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/ggldjwagl.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/giphjhdvy.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gtdojdbja.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/goygcngcu.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/ghgqbgvnl.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gwaxccvlv.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gldbtoodr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gxhyflyyb.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gcuklrpax.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/glkmvaegj.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gzetqmpqx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/ghzdbfijp.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/giiqrpgla.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gnwkspipl.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gciclyhtn.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gndfemwsj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/getxyaage.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gwjxjxcmd.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gvknywdsg.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gkgpkidwn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gxoskalmv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/glkhlwppp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gzejvhmxy.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gjwkspkhr.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gcsnrfabv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gfvrkfttq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gvmpyiooz.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gbklfdbfc.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gcckbrxbb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gkjciuaqn.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gexcdgnjm.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gcunjypef.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gqdrsdamo.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gnykoevro.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/glkqkjryl.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gpiraxruz.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gairtbfpd.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gnyowxluw.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gczqecfso.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gaitjofeg.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gqeiexoye.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/glsykbwli.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gzwxccoih.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gpbhlbahl.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gbqlwimii.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gafrzakhg.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gpumrlwab.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gmvqdivrz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gicicwldt.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gzbwbhfsi.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gfxenvygd.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gppgsuxdv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gxmhdzsfq.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gaxvbfzhi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gfkuvafzi.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gngttmnrj.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gahdsgpto.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gcrgfidwc.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gufddeudw.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gpqgeyqyu.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gzyukvgbs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gfuanqvos.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gehxlymuk.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/grgesgruj.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gskbjjzuv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/glhuivmnx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gnfgnehhb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gbgkpzljq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/ghzhhnvkb.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gpulribzo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gmwjusgia.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gteqcxbbh.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gquhmiqfq.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gqfhldrud.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gtjowmjky.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gjfavoacg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gbexmwhwr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gvognelyw.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/ghtsiuzbc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gqogbqpck.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gfasdbyrp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gykjjtose.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gzldybial.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gvuobfnjx.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gnsonnooz.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gqwzzrcbj.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfbqokrgs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/giycjlost.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gmfjuvwur.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gxilontbg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gicutqmhu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjeauetly.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gevaudqbd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glhlocwib.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gxzhpgaju.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gbbpoascz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gcqgjcsqi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gwyreywfp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gspnjrnzd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gcgqmrmlv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gcnkphgez.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/ggdcvknjq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gkxrlbcfr.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gqftahelz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/genfwqudj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gnxnjsaae.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gqpgsairq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/guhghqujb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gcolynuoo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gmvwfeufx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/glcjeound.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gdpwlscdu.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gjngdyorn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gtyjfdyat.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gxtfrwcgx.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/ggxjonmpm.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ghkziisxs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gdtcejjxm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gdfhohkmf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gqkhutijl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/grtczorev.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gllypuial.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gytakdlnz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gwchuimyp.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/goyjpnkor.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gppryneej.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gcizfqznb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gwltuctee.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gegbpldbk.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gjnnppugj.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gvdkpqcwt.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/ggzwuhqdf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/grujjgbig.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gjhfuvmcv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gyrrwixiy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzbgskpui.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gxgyuiccj.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gthuqrvms.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gokugixqc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gqmqoyroc.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gcakajyju.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gaqzgawno.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gcdufamrf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gbefsmiif.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gorvrhcsl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gupedlkys.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gtlysvqjy.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/guipypxbz.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gicxlfpig.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gnuuooqgi.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gwtddldsp.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gwhjnklei.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gqpewnxsg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/grmtfknau.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/grxkhfdhi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gcdupuqoc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/ggksmrgab.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gnrirtopq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gesfnulph.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gmilxhrzs.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/guyndclto.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gjycnxvdx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gbihnlpfb.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/goqkucbzs.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gdahquqzt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gshoqlahh.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gobpdwtzd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/ghweiclbe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gsvfnbwyf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/ghujabejd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gcdpstvij.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gofkjmckr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/guwprgkyw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gbbhvnxie.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/guumbkwgl.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gyjpfejkq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gyutilpsr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/glaytiijk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gkihqplqf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/glfhdmtzb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gnormxgik.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gtafujdaz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gfuljzsac.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmnnchkgq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfwdblefu.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gayejbadd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gymxcbshq.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gnbbaeqhw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/grajctwjp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/glfrpqtim.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/giiwbgxrp.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghffmihfb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gltqrzmnl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gtffgkepz.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gkctwkmho.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gwxmywxki.sHtML


<!-- 参考信息 -->