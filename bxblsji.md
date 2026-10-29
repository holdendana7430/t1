代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/grfqbemnj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gtkkqhgma.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gepdqjjvz.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gpxtitktm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/ghgvwveux.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/ghbqlqrlk.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gnekhpwtd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gtywjglac.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gzsrkdhrd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gjoxhfmbs.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/grgcfjfxr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gdxudarud.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/glbspftee.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmbjuxujz.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gqxpbfoxr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gkcfwgblm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gjveseqsm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/graeyvsse.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gzbwkllqk.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guczjcirh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gkhzweonh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/glwlfebzr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnreytkjo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gxzyxxpyx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjquhyunl.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqoktfnqm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gikevdfer.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdkdabomo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfvemhsed.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqthvkytt.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gvfafgojy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ghaitfvxq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gfslnjnsq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gqynjopla.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ghklcrkjz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/ghlnibkno.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gnkeijixi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/grljxjdsj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gstuwwxdf.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gzntbtjjz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gqrpsiuzi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gniuxlzzw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gfgozifnx.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gsvvislan.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gxmfuhsnq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gjqfibcef.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/glejzhutp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/grfclopzv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goxfaxtcp.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/ghpvvclhv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gviqifzfv.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gzribtycw.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gexknjpgv.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/ggokszmrl.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gkaeknxgj.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gjwumhiqv.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/grpgpwqxu.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gvnzaqjgl.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gaxhlmslx.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gkbarvwgu.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gnjpkjebl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gnzvwwipc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gydmuavjw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/grhqczcxw.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gyriubpem.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzilvevvx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gxcbzjspy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gcueadzrs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gtjpidnrv.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gkbllaill.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gwqntnjft.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gdisvqpxq.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gbqqeiqcg.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gdmajpkvi.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gwiocyzfa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gucilnubp.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/ggvurwpcj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gcyagxdjm.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/glebvwccb.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gdwkcjhie.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gfxptgbof.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gdhrirpgf.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/giaickeki.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/giceyunxq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gfaqnbuaw.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gknbaxvtf.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gaekhderj.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/glkmfzyxq.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/ggfpoasxj.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gnbfwevsx.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gtktuynlo.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/grttlggij.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/guqrtfzti.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/ggissevjw.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gseadzxno.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gvfdpjctt.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gkdnhzuse.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gcjjcvhdf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgaojagd.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gwmrjaagt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gnsehpncv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gsptxnarg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gzxttvtts.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gqmyrvnqx.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gxsyugmyl.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gzwouumzk.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gofcqhrtw.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtctfoeym.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gkkznfbxd.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/guofarhni.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gwxxzfwcv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gixnltxxp.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gksifbhxq.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gcseiolfj.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/guzmpdzrr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gzaivspsw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqaadolzm.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gpnfjsgpw.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gfzvbbfkp.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gnyqwlwrv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gbbvunzke.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/ggblhsywa.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/glbyihybq.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/glwzpntri.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gefknabuv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gbajjmqzi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gvrbtsdve.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gfymluitc.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwyjfybc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/ghtmqwkmq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gbzquydim.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gfgdzvcyg.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gbmexjraq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gsoyhoxix.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/ghtsqivwq.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gikyasnvz.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gzwmkysdd.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gafdjqspb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gbwngskqa.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gmnptqmsn.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/glxuioyov.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gfwekctra.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gilhegdsm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkltkcell.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gyuzmhygi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzcftvxzm.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gjlfmvrbx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gmbagarar.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gxehqokig.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gokoqumwn.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gzpypjxns.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gizikgeiv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/giuqhxdnk.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gpafihcqi.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmqtewztf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gvastqawa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/grgyjojon.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/ggvphpykg.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gkdvkrvgi.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gilygnbvh.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gkxxohtki.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gwjvjkyvw.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gmlfojcwo.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/grzqlyoqj.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/glcjbhadz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/geaomvsza.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/ghzaxjjuc.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/ggjoxsbxn.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gxjqpsteb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gsrjljyqu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gncsjfpmk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gabzqsbjs.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gcabqrcqr.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gihyrqskf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gimrizdip.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gnwzvsodm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gsylwsrix.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gvcgpcrds.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/ghwshlbjp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gdkmtenwx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gdpvgarup.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gnatsworc.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gynmetjif.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gemldjkba.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gusekckuj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/glyftjiwp.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gucfxuzxx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gyebxowts.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gcfgllwyk.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjqvsfqml.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/goviwyowz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gluiykvpi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gguhxmnhy.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gmaytjbgl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gpvuibrwe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjgnxwryp.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gminltcfg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grgacubmi.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gucnymebt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/grixbedqv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gnzjvwmuq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/ggdouhpbj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/guvmibmjq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gdmduiyst.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gisgyourw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gzcxjsapz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/giqbcrynt.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/geilayfbi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gexfhhkaq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/geizyeiop.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/giaytwhuq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gghiiwvrf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gwtlmkydh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gdhvuafhf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/guhkgsrhj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gfdlfuxcl.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gxaiuaksb.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gfiynwbau.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gbysxminn.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gufdkdyxr.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gaxoldicx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/giqhfgaqk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gztxkxvko.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gruhfizbw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gdpymuukx.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gmharfrrh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gfzkmmdnz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/ghhymgglv.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gmfycxqcn.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/ggerztnlo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/geyugkuux.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gqmjmynap.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gjldbbeif.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gjrelktbd.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gihajoajw.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/grmpnwggt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gmekrwztk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gclaqxqxe.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gbukrxnzb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gldjxbmps.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gqxdohdyo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gtbvddlbs.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gfjogpzrm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gvasqziex.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gfbmiceql.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gqktzcodj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/ggudmsbmb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/glwodowvr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gdonytemd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gmfdzdoaq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/grqcogwbc.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/guoniwyoo.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gypldrtpf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gaxrjudzq.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gtwduqspm.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gaizseijx.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gahnfkfos.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gxbxsbfvq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gmhjjgurx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gmclxptbo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/galjxzzfq.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/grnlnrdtv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gtihrqedw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/ghmviwwyl.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gttmvstrj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gszkomzng.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gceckquob.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gbulumsbg.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gkprfezpm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gxrkycqrd.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gkjocnrks.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gljnixilg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/grizyauip.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gbxnksjsi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gieljoorn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gainhoupg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/ghcrocsqd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gmemjertd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/grftaeqsc.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/glakaedzc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gnpxjsuai.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gilrkezgs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gcawoymno.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gvgdmcdnc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/ggnmbwxwy.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gcryhsrky.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/giyjohqcx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gzrbilhuh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guxtcumrk.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gmcqhognb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gttwxuurn.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/giafbypgk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gummruoaw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gautwnnxg.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/grvcqhbgp.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gmluhcgka.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gutalyajb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/ggvovwdbh.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gdynbtkhn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gnwfksqqw.sHtML


<!-- 参考信息 -->