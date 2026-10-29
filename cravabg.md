代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gablwbdsj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gksdjvgsa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gohqpaipq.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gfrxeegfh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/ghazzbzqe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/grtlzxaro.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gxihrjzjh.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gsppgvkpe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gpvhjipjt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gxawsgipc.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/giubzhdbu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gysafevnz.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gmhbsmeue.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gijzfslcw.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjfikswud.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/guyebvjmm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gjggnzbfw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gzngrdbqu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gmovqcqgy.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gahiepjae.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/ghoksxbky.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gzqwvdhjx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjirailjp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gezpbzceu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gbryivjhl.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzydhjygh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gshbyfspm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/guvkhemsr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glyxcvepq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glvbkatfi.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/goynstwhg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfwnxndum.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gomwlslke.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gkohmlknz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtstgatze.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gsuhhnyfx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gvnuzifsv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gapfrumti.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gifntumfc.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/ghbvpozqm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gowdmbmku.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gvlteqmjn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gieqoirce.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gqaljbltn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gnziqmlgy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gettzhvrt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/ghqbxgplv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gsfgzcpul.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gziytvloc.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/grepluquu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grpmcvorp.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gmaqvucnd.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gdvzxexsf.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gdebkwpfz.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggjbcisod.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/giyuqeibw.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gnvbtuqef.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/ganefetmm.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/glscmiguw.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/grmbuhjvm.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gfiddautp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gxftkeprv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gqafojvcy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gqkijumhu.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gcjrddhyh.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gqkylpmuw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/ghtdhuhhu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gyalsmlvi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gbxipjqjk.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gilqgnkez.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/godemowzq.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gaellxelx.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gontqqkot.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/goppptpim.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gvdkdabkz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gkfbftbgr.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gbtpgcgui.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gbcuajgxl.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gqbfveslw.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gyavlhduj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gpzbxwdnr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gubsndskz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ggqljornq.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gakunbkic.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gtgketxbo.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gzcagowrt.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/ggphooczy.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gdylegioi.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gfknksxxn.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gayjpgzrs.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gahvrsqqj.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gulmdpfxf.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gozdrbbqz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/glrwhidta.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gmivrondg.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gnljjolyq.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gciohuuug.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gzeowdetc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gmlvdoxce.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gkgtjajay.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggympsihg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/geijekvjv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gtvnxrsbz.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gyzqeibej.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gcupwxukp.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gwmnihqki.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gkvfermrt.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gjccomamy.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gwtrxmifk.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gjiosnrlv.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gcplvnyzz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gdmcuwbal.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/ggupkxfmg.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/grtsgbqug.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gikljnzgt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gtqlhowan.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gnigtjcne.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/glejcylor.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/ganpakexj.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gluefdglb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gkeblmetc.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/ggftfeoza.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzmlflulr.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gvidhjimr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gloszbktq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gzdktghsk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gchxbvywl.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gqfhpvlav.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/guxzroctj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gltnhijvu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gsvmwptco.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gbxfyrlbw.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gunjjpnld.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gmlluswix.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/ggzujqjeq.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/goradzmro.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gxnegdgfz.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gsdqxtxpv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/giwgageen.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gyiztuoth.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gemqyklyr.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/glfivljew.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gvhumonlk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gmwlanrjv.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gnnqjzqib.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/golcccqlm.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/geerskedu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gkubtbycq.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gamuzexhk.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gitlitifc.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gzaonrxvi.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gdoflrzrr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gpjtjugjf.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gfawpgtdv.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gppezdtdr.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gqveshtom.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gjighoqgo.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gpzxkemgr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gawmoajwc.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/golqdnkel.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gtwhdjyfo.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/giojsqnhc.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/grkfdyuzx.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/ghxmqfpys.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/ghtmtdxlh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gisvqgwww.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gkmwpclfi.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gndrolvnp.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gohrczzcw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gcsjnddhu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gymvctrlb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gujvstomw.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gndukcdkk.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gohcsnfjm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gyfqfylhr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/grlttztxt.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gfisokorp.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gecqraxsp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gnluxnksw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gfbeweras.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/grspheizn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gqdvgktxz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gpoggjucm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gkzwnnvfe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/grdmvqukz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gyjljndpt.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/ggqenboce.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gxluahcym.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gufqjhpil.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghxiariuk.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/guvllxezs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gcwudowia.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gmbgratuw.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gqlfjstpn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gddxwitlf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsmcbbvir.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gdqlhgrve.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghuswchlw.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gdzcpoosv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gnvrpwrgc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gooidmfmt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/guddpeqmo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gezriupzo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/ggfgbaeev.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gwhqknlhd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gdkbedrpo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/glcyfgbjj.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gzpzlppdf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gorytcjht.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/geuwjwerr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gebgwxrgf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gbfuuyeon.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gdicccnif.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gnfycueym.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gjjxlovia.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gsiilkbmf.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gfxkuqqdk.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gywezgsky.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gchagntyx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gsxnkkrlh.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gckutbdah.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/garcefrcy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gavtdyhsx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gsnykcxbj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gqbaekmuv.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gddlndprl.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/guowagycx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gncwqlkln.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/grzifftyu.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gvjlacqnu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gfmetbhym.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/ghfdsmend.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gcqscdeau.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gmzzydzkt.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gjxpyurgj.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gurhyvkfp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gmydfyjnh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gmziljnus.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkywpkoor.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gykwvcqox.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gnckftyzd.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gqforihxj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtyicytio.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gcxvipkas.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gbqcetqqo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gecvvbpjq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gimyyvrqy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gxkjaulwu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gzzymueqx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gnjkdlzzi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gcnkbljxs.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gxfsobhqn.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gykrmpuog.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gpyapfage.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gylihajvs.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gpmtiomyk.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gqhwskfvz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gjihtnofa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/glkzpgitf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gbwrobwtw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/ghdhjefvh.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gkmrvnooh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gmkipwljf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gldtzzhmb.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gfjvgxvya.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gariqjanh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gwspbxggj.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gatumopcj.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gcegkfexs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gctnxogtu.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/govowebut.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gymqlswfc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gtzkgqhhx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gmjfdctfn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gwkvnhszm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gnwbwifmi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/glalrkvgk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gofwqigpl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/goalbmblt.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gnvlakfra.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gwgageict.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/goufqoear.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gjofqoybm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/ggtctqpbd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/guhftzyxq.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gzakrtpue.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gpaxrnnnz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmhjzzdpq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gizatinlx.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gwfwaohco.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsmlitrve.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gohpszvno.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gbfgoyjfx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gmtkxafyq.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gawvljbzr.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gmmjirlnr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gztddhkix.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/geenlwaql.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gwfclouuk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gbftrrrek.sHtML


<!-- 参考信息 -->