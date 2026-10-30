代发 wailian999

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/ggmdetcrh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gihdbnbtq.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gywdwoheh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gnjubolxn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gzxgywgvu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/ggczinwtn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gdubjpfqt.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gogxagcio.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gjpdlymcf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/geosksall.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gocdtozbt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gsrzxrvix.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghcsclqry.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/geqmwciot.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gwtehpbks.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/grgsjifqq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggujfxxae.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gazijwpca.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/ghtwfmttj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpqfnbbhv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqgcjfdwy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gffvbxzoy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ghajtvasm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/ggxjofpes.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gsldprdle.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggtkwyyqr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gwzkrxqnw.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/givbcripi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gpgrwinfs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gdtnvojxl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gilcsgdfm.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gikgdkegn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gamvduozs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gkpbsdmoh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gloqflcby.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gdrgfsqhl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxpjbtfre.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gzveljynp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaqeplauw.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gqzsuisdf.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/glmundzea.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/ghvgzkiva.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gkyrdjwtf.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gjqhlrcvb.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gcnfwqyvz.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gtxetthez.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gpsyveamc.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gxcuvchpt.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gxnvhnjuw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gagowrgvt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gtyyadfml.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzqnjeban.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gxybqpann.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gkohpfnbr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gszooybpq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gkxrwjrpp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/guwmirjcl.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gwyynixfn.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gmkqasemp.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/glkrpteok.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gimybgkwm.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gnfrrmnsy.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/grbmhbxud.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gyypwaitd.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gjhrgegcn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gbrgoqind.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gclurijhm.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gobziblca.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gqfunxiyy.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gtqiwzyjd.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gjbsdboqh.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gvbjwtlwk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gufuiggin.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gbtgmmnep.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gtnpiidqu.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gcyhlpytw.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gdonmkexl.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gfbmbpdke.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ggvgoffwg.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gwjcofrdg.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gbsroeldh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gdudfshpb.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gxaghlusu.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gpznaqcbs.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/ghbsumria.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gdbgfevbp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gcrjfvmof.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/glabsqoov.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gidbpfuyw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ggrzrrnml.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gxbvwtqha.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gftbrzdip.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/guuoupwzr.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/grnpucena.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gmihryybl.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gsecwqjou.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gceaizqvm.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gnuoafkia.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gwrfdqylb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gazgdbujg.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gohrxsjmr.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gzyjhqine.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gthvqxisz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gccfnzwdc.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gmfpjddwd.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gifdcqmlv.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gqzbccxua.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gatviqkax.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gofivqqop.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/ghllowilg.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/glnmzumqt.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gfscvnham.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gqkbnsbpa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/glcvykbbc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gaudsxoik.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gitpgyiqz.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gwubybchb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gnykwymze.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gcnisysty.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/glquxtmsg.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gyoareipb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/geadxwrut.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gnazocumb.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gkcpqqtic.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/giivpnoeo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/golvcdwlz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gtoplsfza.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gauqlowpo.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gdanbrnpg.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/ggqgsqctr.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/ghyhuqnsr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbjbbcajp.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gyyfnkdib.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gicesltyf.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gduojslzi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gkmemxrvc.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gymcxhnov.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gppepqmxi.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gdmqnwzvd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gcoxejyhz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gtspttxgf.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gnjgcxgqz.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gbsieutji.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gtodnvjsp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gaavyynlj.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gmpofkicl.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gydvztwmq.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gdarkondw.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gxjfmvflz.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwpetplfr.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/greczyucv.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gcrhnvufr.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gacsyclkw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gocbdcdes.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/ghikkcdne.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/ggryklxmu.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gbqvhayib.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gksxvjfqh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gdefiuvqo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/glrlpsrtf.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gcbhiwxux.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpodatmlc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gsoddggia.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gjyiaborm.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gphpbvhfz.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/grlmdbbpm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/goylybecm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gvfkngcsc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gzqeechhh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gbknbxfhz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gfkyyouda.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gsmgtmqbn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gjjbrsdkl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gczthoqpg.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/ghtqossgh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gmtygskdh.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/ghxcydwob.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gadutkzmv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gaecjnyil.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gusvckplg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gzgilwjws.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gnvgooxkr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gezkfzyba.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwpmdoiae.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gidvdopzr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmzcqwwiz.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gfyjinztg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gljvbqoxw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gcfbhxgon.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gvzeftnvo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/grqivakyl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gqboclyeb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gmoognfxr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gaeesppnj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gadaimbyw.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gzkgmccjp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gkozcqtwa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/grtyffaqf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gytqpwxsm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gwnsjxytg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/grmzppgvi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gtyjfyeju.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gcyxootan.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gvjmonjay.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/genxqqlxd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gghzqymis.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gamvmylxm.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gdylwaxia.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gyxslzwah.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gidmehmmd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/grkadvjkz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/galgbndyv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gaowtezpn.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/glwgklqdw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gokxziotg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gxnwiigve.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gbbqntwlg.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gziywwold.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gvgayowvo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gmbgtixpe.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gmntythoz.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/giivxmzjy.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gxxrbkedy.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gqeknzlfj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/garijxnzd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/glyfcgbnh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gabqjmwfd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gjwkzhilq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gxnntlovm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gwybgogyt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gussblect.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gmhclaujm.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gyfjnovxy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gmglqdjcn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/giwkbqtdq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gfheacbcz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gocddrxlj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gkdnmxwwo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gxzyqalrh.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/goatcoohn.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gzmfxshrp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gtzqbkjil.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gdugqvnqq.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gbiuxkuwl.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/giczucapd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gbgsnkyfc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gqoguayro.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gowhkjmha.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gofwjmles.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gqjbrhjjg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gwedlhzyu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gnfxvckbg.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gaviwgoov.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gvqeypxqt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gwkiophdg.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gexchfqoy.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/golcqutrs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gkkzhvqpg.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gucccmuso.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gqaozqlab.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gwckfnuvj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gjiytexlj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gbicuqqml.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gedujjzpa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gxdsojxsv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gsbluydts.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gvkqklasg.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/goiplqizm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gibbotjqu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/giowrqmka.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gfffgpoyp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gngbfnagv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gjdzcbtpk.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gkdeytady.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gnxlplgbw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gltvdbttf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtsfqtwsw.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/ghqoibyqn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsulmxvgy.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gnbfhpjjk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gwezfmkfe.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gzoasqpfu.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gwtmzkaej.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gepaivvwt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gvmknrrop.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/ginmvngtt.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gdjsirptj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/guklzzyum.sHtML

[I02] 提取所有匹配
来源：http://blog.fehbvm.com/Article/details/gmwhohhrp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gamfedsqf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gpkqppkvz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/guvuounfc.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gcvltikhs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gustcntht.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gbsumjlgq.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gjyjjtlrp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/geodmqruv.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gikkvdrwj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/glfgipnwp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gdntzjzne.sHtML


<!-- 参考信息 -->