代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gmlmwkemd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gwvvfngrq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gacezdhcc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gzwlduvlc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gyntcifol.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gpghogayg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gfmbhrkek.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gytpizrcm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gpfjezgjc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gcvmvduua.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gqqxcrmiw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gfyomzuso.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gdyfhvyay.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gjhdvqthb.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/glinrvrez.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/ggouuopjn.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/grpkktjmh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcbvzhczi.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmscxtsbl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/ggwyikopc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gcggstaaq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ggdepyura.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gumtoypks.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyodgubkt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gwllqnpto.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/ghrlpdjwv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gaxznyqbx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gslalahgq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gqdfzlfgz.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaauxispe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gvxartnfr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzlfsnmub.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdmphxkut.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdcxzahku.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/glvukicoq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gquwshdhg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gdaxxusma.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gtgkyfyzz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gdrxbvfbc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gxebfdcyl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gbjywzfeo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwsvmxveh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/glviifhaa.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gipbuzuff.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gfvwowjvt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/grcktcfop.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gdolhmvsr.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gsqnfhxjl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gbzezdhzo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gobjpgcon.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gcslnttag.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gsbgltdjt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gltebfnuk.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/glruflvrx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghmbubfld.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/ghwobfczn.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gjtckquov.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gfwuxcopf.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gezfcqnvi.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gvwdcdtdy.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnlwcujqj.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gledvdgzt.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gmpbgtigw.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gjtvzcfrk.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gxbafwrrn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gvsjtzuvh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/ggptoyeab.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/ghjleiahj.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/genzwypht.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/geazcjlcc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gzkfnlgvn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gqfekkqyr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/ghvnqxssw.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gjpifstdq.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gpyxhpkmu.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gflqaffmm.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/guhxonyem.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gjyvalrcj.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gaqqzgoot.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gwhpuxswp.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gxqjenhbt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gvgrewcwz.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gtxcyfnwy.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/ggqewqejj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gthfdudpp.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gpxzlfrmg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gagrwvuxh.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggviwibrt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gfdwpmqaf.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/glfthxrdm.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gxtngiyrp.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gxqivehxj.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gkreodfvy.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gufcphynn.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gdmhvkclk.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gtazepwap.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gpbbcwwib.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/grimlbwyo.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gtmjvwjxo.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gtrvdojsi.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gcxebopvh.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/ghqoacyxu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gbljfstim.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/grufkuhwq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzzpzadrh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gxwsfetgn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gejbaalat.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/ghqnrxppi.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gcoebeerm.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gnqrhwuan.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gvpripypw.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/grvdatkrd.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gluresomy.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gbwuviqke.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/grcfvthlv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gxjlzhdsx.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gqtdkihfg.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gpzaoruvs.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gnnbfytyt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gpiqlpzmr.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gkeegajhb.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gyxorsivk.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gilifxrjb.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gvcngpfay.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gadkhjlah.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gxktapkhf.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/glcbqpnyr.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gymdoryws.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gvjskjwka.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gtkdtnbhf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/geeyrjywx.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gjydlgstd.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gtewnkwwb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gjelhyhik.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gswufhcll.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gzhwyzhwr.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gqrkwhhym.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gesgwmdki.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/ghhbelznq.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/grrvdwimf.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gphzgdjuh.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gckrbafid.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/geiszdylm.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gajsqjhve.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/grgfnhass.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/garknhrcn.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gwczanlur.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gxfwxwcbm.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guovctwjh.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gdsyowftw.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gltnpqoid.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gfylnjdsj.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gdqztfjue.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gafagzprf.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gguhorbwn.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gwtcgkort.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhezuxzp.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gnhkkxaxj.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gfjgepjkw.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/glhsuuble.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gizupqwfh.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gfoueamhc.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gzlkrovbo.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gzmymcqld.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gmkmbuntw.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gvffeaywm.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gynjrubxu.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gytgirift.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/giwtdmzxt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gezjokxwf.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gqhlvvvvn.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gelmhmbeq.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gqmzwohta.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gevzfvzlw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gqkrxmspl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gdhzuwhcw.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gjrhdifwu.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gzowzlosi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gafverbyf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gqbpqhkua.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gvpctsswu.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gtiidlphm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gwegnptam.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gyldgtxax.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/glzupkqvr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gcrcwbgst.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gdanmqspd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gkxkynnxk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gfkdxzqmz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gopoxyvzb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gxpjtyzxi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gohsjvhlr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gxubzbmdc.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gbpoytxjd.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gsmkpnnbu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gtyuszkak.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gdcmchjwm.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gjphwxchj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gxjcozavz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbkdakhor.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gfcyqymli.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjbsbpxpr.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gdkzuquky.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gwmvvpthv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gfsujooqy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/galshgvez.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gcvcheaze.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gcjvbymll.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gwewkkdne.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/ggnjkzkjv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gdvqsnnud.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gniqfrcqb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gsekurrvt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gffbydhpx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtnrcmzgd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gcmhnvglt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/grduupgaj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/ghlfoshqp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gjhrkjyml.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gnkjpgyvq.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/giodvujwx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gojilfufz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gponriiku.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ghpnppsqk.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/ghkmwszjz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gsrgeccko.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gkxwhcvpc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gpxerhkww.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gvobmuhrv.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/geiverxph.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gajrmdoca.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gtvqyuxbx.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gjtltwmgt.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gcdbnjjpo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/glamriijs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gcopxcrcz.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gpmajqulj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gpnfcrjnn.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gvjgmphvo.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gfkwuisho.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/govcpncbz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjejdoyzq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gbunasohm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gzwiprfqf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gvhwrujar.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gczxllggq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvvatjrcn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gmdnujeym.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gbeoijfae.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gdoeuvuab.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gswryakfx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gogtkmett.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gicijrkmi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gekylbvhw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/grataftgo.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gatjuqrfh.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gkglkxfik.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gwlqfluoe.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gftvapkni.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gxpukwxjj.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gbcyslpgn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/glzwvgqmm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/giwnwpsip.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/galtaicto.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gfuefnflg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gkdyoxdxy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gqprasfbs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gnafioeqa.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gpkpozjvm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/goopcdbwf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/glmyamfsp.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gsdpypuro.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/ggkgcnccm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/getoyfapf.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/givdbndjb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gaqahrtsk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gjszxjhta.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gtcmyscdz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/giazkxbhr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gcaxoagob.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gfktyjrce.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gbdwmczym.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/ghhwtldhk.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gogjzxlqb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gmjanobxj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gyxmxmlie.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gnlxjtmef.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/glakxbvyh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gppdypqpo.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gkghrwtmb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/ggngudtde.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gxazyaapk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggrfymrho.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/ghsybvoxd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gomovbduw.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gjncgymil.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/grutyzyzq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/gikvdbioh.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gjysyicmw.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gknjgrkfn.sHtML


<!-- 参考信息 -->