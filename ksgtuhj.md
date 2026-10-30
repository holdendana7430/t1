代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gbmaekebl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhlyrkst.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjqrnvps.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvlfcgwq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtihrgdje.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fanxiaobao.xyz/Article/details/grmbtrjdj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/gbhguwynx.sHtML

[F08] 遍历目录
来源：http://wap.fanxiaobao.xyz/Article/details/gwebqsctg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvcqwcpe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyfrateo.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gtzwlycvd.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbevwcprx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fanxiaobao.xyz/Article/details/gfikrsxhw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gvawubdmq.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gspqgkqsc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gfgmyhxcs.sHtML

[F09] 获取文件大小
来源：http://blog.fanxiaobao.xyz/Article/details/gnjmlgprn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxmxqbmo.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbzcoyts.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gzslgdsfb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/ghepmnzzn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gutccwpyw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjgjjnfv.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gltaioqdp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfycozgg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fanxiaobao.xyz/Article/details/gkhnhkodf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gbzsyvvse.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzimbodit.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gljibcgkn.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gepovbmly.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfrpafdf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbsxzxmc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gshnavchz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gyoyvairj.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzpcopbe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsympxmh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsatjxnul.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gyvoaixxk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gycqzpsaw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkblazobc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fanxiaobao.xyz/Article/details/gnktnydrb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeedduaw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxwklxcz.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/gktxgovua.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlyltlss.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fanxiaobao.xyz/Article/details/gzzlukydt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fanxiaobao.xyz/Article/details/gozkfrvhd.sHtML

TS:   // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/gcysprzra.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fanxiaobao.xyz/Article/details/gxgorzudn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fanxiaobao.xyz/Article/details/gaedieesy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyipzvwgz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fanxiaobao.xyz/Article/details/gbdnahtfq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtdhgbpm.sHtML

G. 面向对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbpbbblo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gboywfugw.sHtML

[G01] 定义类
来源：http://www.share.fanxiaobao.xyz/Article/details/gobavaxew.sHtML

Py:   class User: pass
来源：http://blog.fanxiaobao.xyz/Article/details/gnpjygoim.sHtML

PHP:  class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmftzmrd.sHtML

JS:   class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghofblgaj.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fanxiaobao.xyz/Article/details/glsjlaibn.sHtML

Java: class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/guzgjvqot.sHtML

Go:   type User struct { Name string }
来源：http://baike.fanxiaobao.xyz/Article/details/gcxoubdcu.sHtML

Ruby: class User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gunishmaq.sHtML

C#:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblieeqil.sHtML

[G02] 构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjhlodlg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fanxiaobao.xyz/Article/details/gzjayiwdw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzdildzm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkfxdsilv.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gewnfxxhl.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtqedxszf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fanxiaobao.xyz/Article/details/ggtgkejcl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fanxiaobao.xyz/Article/details/gcmwigjzz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrwodtik.sHtML

[G03] 实例属性
来源：http://3g.fanxiaobao.xyz/Article/details/gsykntuqi.sHtML

Py:   self.name = "x"
来源：http://3g.fanxiaobao.xyz/Article/details/gkeizrpsu.sHtML

PHP:  public string $name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gxqqpvbgc.sHtML

JS:   this.name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjikgteyw.sHtML

TS:   name: string = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gbhdhqixu.sHtML

Java: private String name;
来源：http://3g.fanxiaobao.xyz/Article/details/gctiydxbo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fanxiaobao.xyz/Article/details/gadlnmglg.sHtML

Ruby: @name = "x"
来源：http://3g.fanxiaobao.xyz/Article/details/gbshaakdz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/ggdapttrr.sHtML

[G04] 定义方法
来源：http://mobile.fanxiaobao.xyz/Article/details/grlbwgszm.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtprwglt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxyqndaku.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnvssumbw.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdqytwnl.sHtML

Java: String greet() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glyybyqgl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glboqggcp.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzcqlklr.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/gglexykxe.sHtML

[G05] 继承
来源：http://blog.fanxiaobao.xyz/Article/details/gyfsoggql.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqjrupvo.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gexpbqpqa.sHtML

JS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwucmlufj.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjafbkna.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godmcmsvm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fanxiaobao.xyz/Article/details/gsgzywbzj.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpnquvoy.sHtML

C#:   class Admin : User {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghyylhkld.sHtML

[G06] 重写方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuuhxymj.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fanxiaobao.xyz/Article/details/grtynltvr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfbtybdqd.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guidyppmf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/galynkhze.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpbgtwivc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fanxiaobao.xyz/Article/details/gtntmeahv.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fanxiaobao.xyz/Article/details/gejkmuxoi.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fanxiaobao.xyz/Article/details/gocuqzyqm.sHtML

[G07] 调用父类方法
来源：http://baike.fanxiaobao.xyz/Article/details/gyefdgwmt.sHtML

Py:   super().greet()
来源：http://wap.fanxiaobao.xyz/Article/details/ggaktfreg.sHtML

PHP:  parent::greet();
来源：http://wap.fanxiaobao.xyz/Article/details/ghzyahago.sHtML

JS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwxajnox.sHtML

TS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gcgrfgxhs.sHtML

Java: super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gyciffzpm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gwisjvmwo.sHtML

Ruby: super
来源：http://3g.fanxiaobao.xyz/Article/details/gjliitzko.sHtML

C#:   base.Greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrfaoljm.sHtML

[G08] 静态方法与属性
来源：http://wap.fanxiaobao.xyz/Article/details/grpyezzsy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fanxiaobao.xyz/Article/details/gjtfyhaic.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guelmzhdn.sHtML

JS:   static f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjqrgjvr.sHtML

TS:   static f(): void {}
来源：http://blog.fanxiaobao.xyz/Article/details/gigpxetts.sHtML

Java: static void f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gywxtvbds.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrisuoro.sHtML

Ruby: def self.f; end
来源：http://blog.fanxiaobao.xyz/Article/details/gfgmjlchg.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujqynsya.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fanxiaobao.xyz/Article/details/gifgbcqzj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdkzsxla.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fanxiaobao.xyz/Article/details/gczqrqpsc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fanxiaobao.xyz/Article/details/gklncyrlj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fanxiaobao.xyz/Article/details/gxgwqfvuk.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gmxdcisna.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvbpywiz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gpikrzmyp.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gkfnqtyru.sHtML

[G10] 访问控制
来源：http://wap.fanxiaobao.xyz/Article/details/gwbivjxvy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fanxiaobao.xyz/Article/details/gkygrbgbg.sHtML

PHP:  public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gelwudopm.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fanxiaobao.xyz/Article/details/gezuairzt.sHtML

TS:   public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgompcrk.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fanxiaobao.xyz/Article/details/gleelvixk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypspukrr.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxzxblqb.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyxnmjzw.sHtML

[G11] getter / setter
来源：http://baike.fanxiaobao.xyz/Article/details/gljlzwfah.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fanxiaobao.xyz/Article/details/gotnpfgdj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gneqdoboq.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvvringk.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzbkqvvgk.sHtML

Java: public String getName() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbwzrhzzc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzozxyeue.sHtML

Ruby: attr_accessor :name
来源：http://wap.fanxiaobao.xyz/Article/details/gmlckiove.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fanxiaobao.xyz/Article/details/graxajprz.sHtML

[G12] 对象转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdndsdwet.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/gedumfmiy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekstnvay.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgvexaht.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gltladvgi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gchhqabgc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/grbnacukr.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfknxuyh.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzisgezd.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyetnlmx.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxxbksaa.sHtML

PHP:  $u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/getnsqpng.sHtML

JS:   u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxabftvg.sHtML

TS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfabryzn.sHtML

Java: u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/guzovmvnp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnurlqvw.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fanxiaobao.xyz/Article/details/gdruqwlfr.sHtML

C#:   u is User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcdotolg.sHtML

[G14] 数据类 / record
来源：http://blog.fanxiaobao.xyz/Article/details/gcmupaowd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnywrgdu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fanxiaobao.xyz/Article/details/gvnxwwcua.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfjnnnzt.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxprpdbtb.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmwbbifk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fanxiaobao.xyz/Article/details/gxoqqwubn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcjmuxte.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fanxiaobao.xyz/Article/details/gsohygskp.sHtML

[G15] 枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gfoqdjtvk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gupvustyx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmbtvfnka.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fanxiaobao.xyz/Article/details/gvrivcpoo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqhrsmyy.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fanxiaobao.xyz/Article/details/gyfwqmrkl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fanxiaobao.xyz/Article/details/gofkgdwur.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fanxiaobao.xyz/Article/details/gdfzpptkd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gvwzppuin.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgjedpdf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgldiaar.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fanxiaobao.xyz/Article/details/gdwemybqk.sHtML

JS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/geaazeiku.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gflkhdzpp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fanxiaobao.xyz/Article/details/gftcqqmra.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fanxiaobao.xyz/Article/details/gddhuncbg.sHtML

Ruby: obj.instance_variables
来源：http://blog.fanxiaobao.xyz/Article/details/gmnowbhxf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fanxiaobao.xyz/Article/details/gthleepwa.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsduotjtz.sHtML

H. 异常与错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/grlmsbjiq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtdbjvkq.sHtML

[H01] try / catch 基础
来源：http://baike.fanxiaobao.xyz/Article/details/gzczjspnv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqunzfsml.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gupidwayn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcengcua.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gsbtzlril.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyudwenh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gocvgqive.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fanxiaobao.xyz/Article/details/gneuwqevt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfazxyex.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gdavkliod.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fanxiaobao.xyz/Article/details/ghhsnhisu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnflhqade.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqemmptob.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gebcdcekc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/giacfcrtm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlyspmgx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fanxiaobao.xyz/Article/details/ghqtynusz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gcnaulpln.sHtML

[H03] 主动抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gzidnbzsk.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkijoevi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxgwqakc.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gdxwlfpzf.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gtmpwkviq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxjmjgpb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunkuwvst.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtmvufdb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggobmvnnp.sHtML

[H04] 自定义异常类型
来源：http://blog.fanxiaobao.xyz/Article/details/ggqpdccyl.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gzchqrzbk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fanxiaobao.xyz/Article/details/gstrajqxx.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grfiidmpy.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqweaymc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrfoxbrt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fanxiaobao.xyz/Article/details/ggvmrzexb.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fanxiaobao.xyz/Article/details/gtqilntdu.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzbdupvsy.sHtML

[H05] 捕获特定类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gtliwazbg.sHtML

Py:   except ValueError as e:
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgnfpmic.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjhpkujq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjtwlilg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gogkyixcd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/geixbvgyj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxixtvbfb.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvpxtcid.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxnloaaq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fanxiaobao.xyz/Article/details/ggfxdnium.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fanxiaobao.xyz/Article/details/gkpiwfhwn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/guxtavvjs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjniowyi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlvsscjn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxoucflk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fanxiaobao.xyz/Article/details/glkpnqioc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fanxiaobao.xyz/Article/details/gtppgtvdd.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwnnkoiu.sHtML

[H07] 断言
来源：http://blog.fanxiaobao.xyz/Article/details/gjjtsnyyw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmflppse.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrfycuco.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gcfeedajy.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvwzncrl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fanxiaobao.xyz/Article/details/gqvqiapkh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gpluhaaix.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqmaxxia.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gyxkhrglu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzttixyu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxhcxbiy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzgfkxdu.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzvquboi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpgbgjwj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fanxiaobao.xyz/Article/details/glmyojsiz.sHtML

Go:   err.Error()
来源：http://wap.fanxiaobao.xyz/Article/details/gihgbvdsl.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjxczrfu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcffriifv.sHtML

[H09] 带错误码的异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpdyjhgt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fanxiaobao.xyz/Article/details/gzndhrwlh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnblrqfrd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbfuvdce.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fanxiaobao.xyz/Article/details/gevfcasvp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grmxcewsg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqxxknyf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fanxiaobao.xyz/Article/details/gvqnsrfmk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fanxiaobao.xyz/Article/details/guekqehhz.sHtML

[H10] 资源自动释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrpmymjv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyvrogjp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxsclcjq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gljnzdroz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/geqkgavgh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmxdsgkx.sHtML

Go:   defer f.Close()
来源：http://wap.fanxiaobao.xyz/Article/details/gcsdcgwkx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpcuqegf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcqbsqsv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrtgthhy.sHtML

I. 正则表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuzlezoy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnddrpwo.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbknolndx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gpfjhrljb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfurzofk.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkioljtf.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gkpmptztr.sHtML


<!-- 参考信息 -->