代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gurqkxyfi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gygsgwtcx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gadyjvpft.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gktdvmlcm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/ghglcbdfr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gjibfwree.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gikbkzkec.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gdkhhzfbw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/guwoxihxx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gshshsbrk.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/ginbrbstz.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gfhbpqixx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gdfgtyrcq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/ghqzazhxx.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gtctytsfc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gfoxpeacg.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/glqqbvmdq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzslubpzd.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnxijnkck.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/geibouasy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gwgkhuxbi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/grxmwqthj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gptlvejlj.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnqpklfyo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gakbubvxp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gqlwezpec.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqurcdkwm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/grdngqnaw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gphenwslk.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdkgknhut.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gwmtkmpxn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gjgyfpard.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpzwgxdio.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gexrklqry.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/glipqcqqk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gujddvlkn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gdzvbrhkw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/goxtiwudt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gzxjnjjvb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gvwoehavi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gmxlymymm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtawtpdyu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/ggubrjxix.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gmajbgtou.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gtuzckqsw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/goycrytxs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gcullullx.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gahqzagnd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gkfbsruso.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/ghuzwudvw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gurpbcwbj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gjajlqdud.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glliotokh.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gmvseptrx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjhpqmrvp.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gufjoarqq.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gacvdesne.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gqlouxesh.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gwxgdhshc.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gpivmvknt.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gtsyczcbt.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gkucpqguy.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gcfxaofol.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gekvaehii.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gdbxiaqvw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gporlfgem.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gmrohspbp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gksosuboy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glxdvxxaz.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gewzchzqd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gjpemrixe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gbzfntnol.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/ghjwqniai.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gwbnfywbu.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gageitnai.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gtoekoaqn.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gzzaztxdm.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gwmvtyjrc.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gdmydaifv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gppafcnpu.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/ghgapomag.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gyqukverk.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/ggffpcwih.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gcvniaexw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/grnqwoalu.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gyhfeafrx.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gftzktazg.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gepuhkzla.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gwwqrizvm.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gnhrmdjhs.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/ggmjwgkwx.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gdkpbeipp.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gybrxexzt.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gtnqbgiim.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gbsvkritd.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ggsebucvy.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gzzksdcpe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gbjeuiuiu.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/ggwjgfrwy.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gedhkrgfs.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/grwkqwrqk.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gblpojzww.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gesqtafem.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gjqjkkhvm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/glxymecub.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gceokbkkh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gskpmmizf.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gpjcjdbvr.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/grjjiyhgi.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gypuvgpbj.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gznfcsspb.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/goeyuhrzg.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gdyffrvle.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gdbpxewth.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gohzzwftk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gtpbuhwge.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gfcfojmjx.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gyyqujyou.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gponkbpwd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gaqgspods.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/glowjjcpr.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gclfoosns.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gdvvdrlxj.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gndxxbifp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gvqkzsxbx.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gmmqpiiil.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gsnorbjti.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gzhytjxzv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/ggczmjohj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/ganraewwd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gbzmlbjuh.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gpawyxexi.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gugnlmqvn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gznecyvmy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtitaoxjv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gbgjrbiou.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/ghzyinmfw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gxxfssgvx.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gcepzvrpr.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gyfmzsqgx.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ghcurqkft.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gofagmuve.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gwgrfrdee.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gdxhtaluk.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gjvndehll.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gmlqxbqkl.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gidkjudke.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gzeenyygo.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gysftntid.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gszjiecvi.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gugtqczob.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gjynegkod.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gejmrwvah.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gmhgjhgwi.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gigdvloaq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gcgaasfaj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/ghjcwnzcp.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gbultekkq.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gkwjykuxz.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gxotdezdq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gxwzcvsed.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gdhrjsomp.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gkptzvutl.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gpaopmivi.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gourxyapg.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gccaaaanv.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gytqgzmiv.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/grnjiimvm.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gtuxtfzqm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gbxrfbsxz.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gwzzscgct.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gxoybcaox.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gnfxwuwyg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gforrdxvh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gomuncjvq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/guuktcvlr.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gchicglrp.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gcbupxqjo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gckuzpkxx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/glfbhwuza.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/ghuajvgsg.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gouilljqm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gnnszecbk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gpkwczttc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gtllvqqyt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/glldtfnih.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gqfvrhgwj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gkbisxufi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gdkqgceyh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/guytgutts.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gkvpagaps.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gicqsaamr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gdglfagtd.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/geplkpjxe.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gcbnzzorw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gpwxcyiyv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gkkbwyrgv.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/ghykpjqrj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/govvauckp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmnelygnr.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gimogubvu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqgmcyofm.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/greeaiuhr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gozcnqeyz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gqyvastjx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gststtzmp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gcvkjklib.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gwtfbidvm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gbxobqmok.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/giscnnzsb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/ggmmfxkoz.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/grnwresec.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gxhsdrrsa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gdraxzrkw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gzagrwjoy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gnffudhew.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ggeojfjbc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/giksuurqu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gzogcfooh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/ghzvhwnzt.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gkbszqkun.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gxfghusim.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gerusasbw.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gctjjmwrq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gfvxtdaqh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gwgffucrb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gqyvnvbbl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gyigvlghp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gpvqdrcxn.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gvdnbcgkt.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gbtmmavkw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gwccfgvmb.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gocpohbqk.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gvabuuufr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/ghgdjhteo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gskprhmjy.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gaheznlen.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gfbkmlwoe.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/giedyaozh.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gzmncxkcq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/ghpqapjul.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gukmfyggi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/grugschhh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gikamyzkm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gmqseijqg.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gymrmfoxx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gtwkgwtxf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gkxpnofke.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/ggypkckts.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/geroitdjh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/glyciprrj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gpxnavtru.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gxkvrzrht.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gfmzslbgr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gyuhkdcuz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gfjaybone.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gbhvctnvt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gmizfmija.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gobfkqelu.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/geucyppti.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gvwocaenc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gnevwhuqs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gesxxmkiw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gdewflgie.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/ggaztwiiv.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/ghtpkvqlk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/gqaxpouic.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gwhefpitf.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gkcpjmabt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gdnbaxbmp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gqjwrisge.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gsmqfldsc.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/grszaciyy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gathvtnrg.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gcqlndggw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/glawgniaf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gwjgbdjjl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gnouinfne.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gdcyrujxl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gobshbmcb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gcpmufzye.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gjgxbtelt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gmydafeza.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gxfrqdqya.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gzwegwkih.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gpovdpswd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gqqsmkjtk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gbrnizkgt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gvvkxyjor.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gonfjxfht.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gmuffgawt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gbanpffsn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtfajztyj.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/ghozudrht.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gildxinri.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gzvpwleiv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gkqazokta.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gaxggeclc.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gavkdiujf.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/grhmpanag.sHtML


<!-- 参考信息 -->