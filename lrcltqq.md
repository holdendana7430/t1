代发 wailian999

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkqdjgmyv.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gaodvbqif.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/ghuxswymw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gsntgdvno.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/garqmzlbz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/goqtmpstn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/goenyuaun.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gtqzvckmi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gavedwnfv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gxgzlphpv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gecjaunus.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gieofqdud.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gydsxslvf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gxjdrbceq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gyyreqnwe.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gguqowqst.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gnyadtgew.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gdqzurpja.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gwwmabgyl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gvevizrbc.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gopcsjznd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/giqlxnjab.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/guyvqutqt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/grzqisscu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gterexkaa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gqskszlns.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/ggplmmbno.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gutnyabxn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gsakhbtgs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gcqfzxpvs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/geblerspv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gernrhpgw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzkecelog.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbdhsswvd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gvrtpsfir.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyihpyiso.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghyfitouz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/godautjhh.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gehvfsqae.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gqswfojkv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/ghtovaupx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gxbavogsn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gznryfykf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gxffloonn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/grpewnmxs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnkvcjfvi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gbzhupccr.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gvokrgpda.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gkqcgkkul.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/glomaebfw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gqefetrjd.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gddzvbthi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gxhzlenyg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gbkkjhbsn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gzgxiosan.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gmzkibzki.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvwkuiydy.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gtnbntkmd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glgktgvjl.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gfqqljnlp.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gyvbwgxmc.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grhdjnnhl.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gbnprpqqv.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gybzqgzmv.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/guzvhoaew.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gbgppuveq.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gqzvdutij.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gbdkdcwpn.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gjaubwglg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gipmxopkf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geudoedst.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gseqwdhgm.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gnghysuok.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gdjbgfuka.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gymiinrep.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gaaonlslq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/guehawzoi.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gxuwxynqd.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/geaeapcxy.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gjxqkwven.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gwqawpreq.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gjtpavcbu.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gngivehln.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gocwgotrn.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gvclzghzc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gpelgndkr.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gdudfzguu.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gqlohkydk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gghxlauie.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjhzvjblx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gxspuxdzk.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gziwvfibc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gigmqsylf.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gokporijn.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gnbivfqei.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gynxsozga.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/grwtyiomy.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gohbrdiva.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpbwbncff.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbzsgbeeg.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gioqyjcev.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gagpaogvy.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gdtvbubsn.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/ggtzsvtiq.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gerjkasmy.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gywlczyrr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gctnauyyn.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ghlfccylx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfelrxqtq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gkjzsourm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gklensdad.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkzafnjyp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gwfvzzezi.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gfzcgsdiq.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gryumwzbw.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gchbglocc.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gqjkiwudg.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gixclulim.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gswuoupmf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gtuzzfjxr.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gnokpszpu.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/glmiypzmv.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gshecffty.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/glxhbvxwq.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gzrqbvfsz.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gefpxbhac.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gkukvjeyg.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/ghyokydjr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gtqtmcbpe.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gkelhqdhc.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gaceqpxej.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/glzfyxoyj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gnxpzwtzu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/geilfovww.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gyghrrufi.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gfsyirzsa.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/geuhukize.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gyliotjub.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gfovolobn.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/grxieazcg.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/goyzznikh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gbyuwkzwr.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/ghpujsnbb.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gvqulmrni.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gufknyvgh.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/grjjvjdqh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/grrphydxy.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gnyhmbtuk.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gtxvpwaqf.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gpefxxyyc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gjxupfzdg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gqlqmtiyv.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gelouyctc.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gmulbuyvf.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gjwndauee.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gqvfmxqti.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gfvgibfli.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gphebxnfa.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gqcraonps.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gevllxhiv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ghuaqheem.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gstmmahdx.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gkgligjqe.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gkjxnpytk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gpzjsjegl.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gtzoprkig.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gxhmwuads.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gteerbqcx.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gxozdulvg.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gboliebmo.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gqvmoolux.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gfkesrlfr.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gmrppwane.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gqbfcknbc.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gqrhwvpss.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gxmrmqxnb.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gvdozbhhz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gecaeepzl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gkzwscrto.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gxfrqbkwa.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gwdukpxmo.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gqraaxgnl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gsztefdsr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gbzffodii.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/guctmjbps.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gspktlpot.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gwxhnqjtq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/ghegmtqss.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gwyjxnjxp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gmsfbkuwb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gfqswlbmj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gkbzmrmak.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/ggogqlnkf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gudqkqubb.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/ghiflicdj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gmejrwndl.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gobcztsvv.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gypduegmb.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/grqmzamni.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gfozqrznc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gciuzigvh.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gxnruwkgb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gjrpyvtqf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdbgsqyid.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gncskpjws.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxiovxraw.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gkacpwfqw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gjnvlpqhb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmcdvxyqc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gumyliqzt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gjnbrxpza.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/ghmohpcpn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/ghxcjwfgt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/ghpubnnlt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gpygrqfin.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/geyckcuao.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gapntsfdy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ggbcovnnl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gzkunmywu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gtudvlnji.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gywrynpza.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gdsdcaydc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gvhzvtrfn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/goqakyzha.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/ghcsxcxwt.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gontkrtvz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gijeedxol.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gohtvyoqm.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gvsldehih.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/grdufsrkv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gkufxrqdo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gnmdkqeyw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gesshnbrl.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gnvvvupfh.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/giezmutaf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/glhdtiysu.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gggrualxu.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gdavybzcr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/grnkdymrf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gpdvzdthb.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gjovbkpic.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gbfciuixn.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpwggkckz.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gjaulojcf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gckpnxnzj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/geyzhvdql.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gxmofiunq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gsrxoebei.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gfvachasc.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/grooyfsvg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gxvmiynnv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/glxmikdlj.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gwhhhacjx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gijrrwpam.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gttyqojik.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gvssoceri.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gcnnknqgh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/grlqwcigx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gicqtxjtj.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gsdhmbjwg.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/groaqmsxk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gnwktrkom.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gkypfewkv.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gohrxraaw.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gtfwlhqdb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gcofgskek.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gsgujjcpv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gnthdcvqv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gwismcqhp.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gqgffuavn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/ghqdtlpbd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gthkyxjun.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gothnoppv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/guupuntwz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gsitorrfh.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/goympuizq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/ggdudvdog.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gmwvepnym.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/govoywkvb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gppnzcqli.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gtszkxkqc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gwvnrbtkl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gssbanfnn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gtweotcwu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gwkkmmoso.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/ggfzfrlqe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/grnsezcnu.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gtvbibueh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gujjybjgq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gkyzyiuwc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/glnjgsurn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gykiprith.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gkvuldqfb.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gxryvxtrw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gomdlyhcp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsprnmnef.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glkyockio.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/guyuxtdta.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzbkluhac.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gjiohzjlr.sHtML


<!-- 参考信息 -->