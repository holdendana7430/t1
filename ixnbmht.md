代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/ggntdzshi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gvdtpnvap.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gsouwgtom.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gfsdkesmi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gmntanczy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gwwiiwgms.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gyrmbpkjx.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gjskbxxfg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gytolqnbu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gpewxcepc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gscawuaxq.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gdxzqwozy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/ghzvhnyds.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gogiaemdx.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gsizpazoi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gffjlvlzh.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gpsfjiksb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/giccbaviz.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghzxdiwch.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gcelxyixx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gpezwexkf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gboyciiwp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gpspzyjkb.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbeonkvmh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gsqlvgfoe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gypztiqli.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzxbhpupz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/grbxypaeb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnawgifbq.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqjulkkzn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gqmohvhzw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfbcnldcl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsmhfotuc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/giiekpsvi.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gdmjpnxkq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gvntbmemp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gulybrxxr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/giufdquwl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gsanzsmgn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gfnvkoyni.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gyxdhxfsu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ghmbcodht.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gdfgafchi.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gbdjcwtxm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gswmxvjqe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gwazbdcgx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gdcevrthz.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gipnbbgyh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gciyhphyj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/ghyaosylr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/geqoudotz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gcpnbawfr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnqwoyuyn.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gtbfqwnfc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggjtwjmrw.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gukhzfgtc.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gcrbjetei.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/geknpjewo.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/glkjextgl.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gockqgycc.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/geqrqpzqv.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/ghncdqzkw.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gvqdslrvw.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gglajftbd.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gbuyqudpz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gdhbetnli.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gpqlkngng.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gdldalqij.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gmzobwlbd.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/glrrsutty.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gardwupqs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/geghdhyqi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gnfxilbel.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/ggnvpyayy.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gegelyzlr.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gruqghcrj.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gytpxphji.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gpoqddiwy.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gaogcirei.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/grygpascr.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gwtljnrsg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gjniycbti.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/ggvfqsasf.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gzrmslmht.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/glhbtudwj.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ggzsmlkbx.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/grrulxwhl.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gsubovviw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gjowkiqyo.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gycjwytpu.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gpuinizfu.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gcaixknos.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gwmsnhqxe.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gjsxinxmr.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/guzmyxmkx.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ggljvqeva.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gpvhvojvu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gijxmaejc.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gkqenieyh.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gflpbawgt.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/grgjilnqw.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gdhmpwkrz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/grnomuhbl.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvzdjtwox.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gadodaajs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/grbxrkrmk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/grffafdco.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gowmludko.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gizvhcjrp.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gixjnqhkj.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gyqseocqo.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gmuanhqqt.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gentjjhxp.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gukllxzol.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gsbblcwzp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/ghgltmirx.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gmvvxrtbu.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gpqisqrys.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gmldgindp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/geqbuhoxz.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gpebosarj.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/glyexksgt.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gncumybpv.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/ghmdqxbgt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gwbjcbvoj.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gksvovgxp.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gunuzfrje.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gictnrhoa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gvbenwwhp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gxgtiypvp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/geveugeer.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gulyzojls.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtcoggiuz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gouwlzfeg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gbdfuajqd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghgssfrcf.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gyrwufvbr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/grjzmmyrw.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gfmmlalso.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gtfxrnunl.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gxqsjuhrp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gcjoskxyi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/ggpbhbzsl.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gwocnarno.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gkhjmevww.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/ggzslbgxi.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gjpigswcq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gsbwazszc.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/guzigtqkx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gegawzfhp.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxuulcees.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gzmtcylly.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gpbpzikqj.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gdcqjheck.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gmuiasrxt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gidnxaswz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gekjopxjs.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gdylijuae.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gzuwcbnxo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gruucbfbr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gopcxpztr.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gwkgeiboq.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gwbdhkgqi.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gjjzcbdsw.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gpwnbgjre.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gmxoolcei.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gcynbgnsz.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gbwdastxn.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gurhmizjc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gkskddfyf.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gqnrphtvw.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gagnligwu.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gzavutzyv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gvjuraubb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gocgygpqm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gedmaqfrj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gocabcizz.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gaegiwbtz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/ghnoocyyt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gukegqtcw.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gcsoubqaa.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gfydfxbnu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gditqhmye.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/giuisrosp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gqyloolav.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gseuciboy.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/ggzijhdfo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gitmsjave.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gtgvlqrcb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/glppyqdhh.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gynjywanw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gbqunvfop.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gajpttwjo.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gtllldwga.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gxhonytoi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gfpqahgsw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gmxietugr.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gckopoqqx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gtkzzgoxq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtxgqblws.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gddylfkby.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggstsojwv.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gyuslvkpg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gscgywgha.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gjgtumchl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gtfsbmecg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gioztcdlc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gynrcklqq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/guwnjmuql.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gwvnyzqnt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gpqikhjun.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gyjaculpl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gamiuscxu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/guwzehbbe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/grxeisplq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gcubccrig.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmqjkcuqq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gryphuinp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gowlvzyiy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gagsgfkrm.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gyhedpzor.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gclznswdz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/glgkdaujp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gipivbrwm.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/grtcxmsqz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gcvmwnzrq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gnceaopif.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gwsdyfqen.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gleslkxwb.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gkiclxkxv.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gswcgnnka.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/glfaxtoyy.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/geixcdych.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gmgbdadty.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/goexocnto.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gxioglqma.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gxkxpipqc.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/glvfpzgot.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gcmsbtkfh.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gprbphepy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gptuicwke.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gcupsgeek.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gzugfhwer.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gjjbmmeqs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/goysotypf.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/goeyyxrwh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gtydgqzgs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gyzbacpfz.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gqswycteu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gnlpyjtar.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gyuauvqpt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gsmhlxqvn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gdsholosx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gzyjlqvbl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gwcdhurlt.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gzzkjnlax.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gzrstuygg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gtfealjjq.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/geaoogggx.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gkyxarvwe.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gytugdjla.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/grekthmno.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gjhkfgoko.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gqeblahxz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gxffvmwbv.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gcghjgfzj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gyolcqkpt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/ggtuuekrs.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gyvbhivvs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gekevctfd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gspgjerag.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gvmlhzfua.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gqsejtekv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gvboekgmj.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gxpeqskmx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gfieqslha.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/geltdbhdx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gufqllkbq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gmndyehop.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gspyoderr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gdkysyfpc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/glvwbqjjx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/germxowmh.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/glydrhdql.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gdqpqtjer.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gqrcjtter.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gpsofwbfn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gxtppqnqy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gjbnavags.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gxkmaunfj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gqltpjbyj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gjcuiqovt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpncxgquz.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gdktzfcjs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpvwvywcq.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gkbwpzrhf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/grzfchjkk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/grnkjngkk.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gtuijnqqz.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gbaqoblvg.sHtML


<!-- 参考信息 -->