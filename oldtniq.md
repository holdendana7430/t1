代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gtpwrdlcd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhwfqyfi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/guldlvrko.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/groajmjih.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gduaybnqb.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/grqwmcgqn.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fanxiaobao.xyz/Article/details/grxqtxrfd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gedszmpry.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gepixwgkb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/goipetzdn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/guxuahrxl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fanxiaobao.xyz/Article/details/glxtjduje.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuslcinx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzximuxuh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnklxaans.sHtML

[F08] 遍历目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbnsgdvc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fanxiaobao.xyz/Article/details/ggjxexrmu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxzgkwkwa.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gkjmkgars.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrctvdib.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpmjmuwg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtoxstma.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowaehhqy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhyveiss.sHtML

[F09] 获取文件大小
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkaiqxuj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjsocwct.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyjpvmcj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/gfpaiocpd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gywzlouzw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gqobapzrx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghujsmjxr.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gtzqtdwcc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvxcrpse.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fanxiaobao.xyz/Article/details/gecvvckju.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlkkdqcs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gyrmjlbyx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gryphgyel.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqwupjqt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxjdibdw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gsdstmegi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfbscjza.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gxbqgkesx.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisritiju.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscgkvwco.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gkfkpdajw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gamtqvknx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqgpiyfu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/grukxfutw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fanxiaobao.xyz/Article/details/gnyjxefwi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gamkugcwf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fanxiaobao.xyz/Article/details/gxszcarnl.sHtML

[F12] CSV 读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyruepds.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjymycijm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefjxuvhq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fanxiaobao.xyz/Article/details/gkzclwdnq.sHtML

TS:   // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/gmsxvkued.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fanxiaobao.xyz/Article/details/gzeuolgdb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fanxiaobao.xyz/Article/details/gwjkvxmgu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fanxiaobao.xyz/Article/details/gylcadtgt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fanxiaobao.xyz/Article/details/gzntrdhmi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlhduhdq.sHtML

G. 面向对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjkcrsjm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gubbdsslz.sHtML

[G01] 定义类
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcnmhvzy.sHtML

Py:   class User: pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gmefpsqrw.sHtML

PHP:  class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhdsregn.sHtML

JS:   class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrpzwenx.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjfmjtgmb.sHtML

Java: class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gekjcigpw.sHtML

Go:   type User struct { Name string }
来源：http://baike.fanxiaobao.xyz/Article/details/gitusimtg.sHtML

Ruby: class User; end
来源：http://blog.fanxiaobao.xyz/Article/details/gjcttysfc.sHtML

C#:   class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gqomzzyxo.sHtML

[G02] 构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnenpcdui.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fanxiaobao.xyz/Article/details/goixahekl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghrpqeljo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjlttegf.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpwnfmdo.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxzknhotd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fanxiaobao.xyz/Article/details/glgboteqq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fanxiaobao.xyz/Article/details/glosxtvji.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjgeqdxh.sHtML

[G03] 实例属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxepdrgc.sHtML

Py:   self.name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gjfbsppwd.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvphisfm.sHtML

JS:   this.name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrhbekae.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydvagykk.sHtML

Java: private String name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gctnqhinx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytrzzuyy.sHtML

Ruby: @name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gcedynwgl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gtylgmlcg.sHtML

[G04] 定义方法
来源：http://wap.fanxiaobao.xyz/Article/details/gguhkfhky.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fanxiaobao.xyz/Article/details/gastrpaay.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmakhnqb.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/githogfum.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrjsfray.sHtML

Java: String greet() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjcxyllci.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gejsdtuhg.sHtML

Ruby: def greet; @name; end
来源：http://baike.fanxiaobao.xyz/Article/details/goblblzpk.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/gesovcyxk.sHtML

[G05] 继承
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxkckmdi.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/grbzfdkta.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmmmuyvpl.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdddjxnp.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdqmstsj.sHtML

Java: class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvhhniugn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fanxiaobao.xyz/Article/details/gdnfnwhjo.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhkxeixo.sHtML

C#:   class Admin : User {}
来源：http://wap.fanxiaobao.xyz/Article/details/grsxgyrga.sHtML

[G06] 重写方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdosshqgj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgsgkdnt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdplddfu.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gescejdmo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbaiirar.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzabzeep.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmczuyiep.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fanxiaobao.xyz/Article/details/glhpfxmic.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fanxiaobao.xyz/Article/details/gowenqadn.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlaisvof.sHtML

Py:   super().greet()
来源：http://wap.fanxiaobao.xyz/Article/details/gsurqdxhi.sHtML

PHP:  parent::greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkppjobbr.sHtML

JS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gtowtvrgf.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfzojtao.sHtML

Java: super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gtvqutxze.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fanxiaobao.xyz/Article/details/gqcjlcrlg.sHtML

Ruby: super
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmyqwhpp.sHtML

C#:   base.Greet();
来源：http://blog.fanxiaobao.xyz/Article/details/guadbkwlk.sHtML

[G08] 静态方法与属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsntifxr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fanxiaobao.xyz/Article/details/gjtmkmmny.sHtML

PHP:  public static function f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gcgbwvrdt.sHtML

JS:   static f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbadelfrr.sHtML

TS:   static f(): void {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkkfxphpa.sHtML

Java: static void f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnmfivvx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fanxiaobao.xyz/Article/details/gquzcibou.sHtML

Ruby: def self.f; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gyaurqkod.sHtML

C#:   public static void F() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpoaifkev.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fanxiaobao.xyz/Article/details/guvbxygju.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fanxiaobao.xyz/Article/details/gkqlqohzj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnamjohmu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdygowvc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewvelktk.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsjeosku.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fanxiaobao.xyz/Article/details/gwarnimia.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohthcfpg.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvsjimhrn.sHtML

[G10] 访问控制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhpoxqjs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogelseih.sHtML

PHP:  public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvcapxid.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbrwdysx.sHtML

TS:   public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gwbsonxlf.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fanxiaobao.xyz/Article/details/gkhgyqqyg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fanxiaobao.xyz/Article/details/gtapapuxs.sHtML

Ruby: public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gybttusjn.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grihxbmpe.sHtML

[G11] getter / setter
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyseispn.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fanxiaobao.xyz/Article/details/goitwivsx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzwiigsoc.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfldyqkt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwfxirfj.sHtML

Java: public String getName() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gleuzttpy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggemwckll.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbvjfzgf.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefeckkzn.sHtML

[G12] 对象转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gncqjgmgu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmphvhpl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzcalqynn.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoymvrow.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveotbwwv.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gptyirgcy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gnauayygq.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fanxiaobao.xyz/Article/details/gcqgtnbtg.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/ghbrctnpq.sHtML

[G13] 判断对象类型
来源：http://3g.fanxiaobao.xyz/Article/details/gfiyywjty.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkmnhdcw.sHtML

PHP:  $u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gdpqkujeb.sHtML

JS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvotbxyc.sHtML

TS:   u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gsydfjody.sHtML

Java: u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmezkhif.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaqpbudt.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprftcpxa.sHtML

C#:   u is User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmapzcsa.sHtML

[G14] 数据类 / record
来源：http://m.share.fanxiaobao.xyz/Article/details/gphojgnrh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fanxiaobao.xyz/Article/details/giqxzirkp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fanxiaobao.xyz/Article/details/guulxhseq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvqcjlwk.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fanxiaobao.xyz/Article/details/gvufoefya.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpufxgba.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtaojssfe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fanxiaobao.xyz/Article/details/gkbkascxp.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcknehidk.sHtML

[G15] 枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gfmsaohce.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gpmpatbuk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbuqkqvxj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fanxiaobao.xyz/Article/details/gfqmeglzz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbboztfn.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkhxibmm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fanxiaobao.xyz/Article/details/gklwgkdjh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrwukijf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gputnbvgx.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxumhoaip.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnmiymoe.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fanxiaobao.xyz/Article/details/gpalpqurm.sHtML

JS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gumywjwxk.sHtML

TS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/govuakhxl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fanxiaobao.xyz/Article/details/gylbrtwbs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkteakfc.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwvquzmf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkrttpad.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjdyaulh.sHtML

H. 异常与错误处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnftbqat.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grvkqwjup.sHtML

[H01] try / catch 基础
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwlxuwvq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcporzsso.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdkorfaw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gnscwutpp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgbnmttf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fanxiaobao.xyz/Article/details/gvjnixxqj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fanxiaobao.xyz/Article/details/gmmtddmgx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsbqlubi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvxbrkex.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmtyhyjd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fanxiaobao.xyz/Article/details/gielymkbe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/geiporopx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfytvlvqi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcfhrzpl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlyxxoqo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fanxiaobao.xyz/Article/details/gqehvqwcv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkuuvabx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/ggdksiakk.sHtML

[H03] 主动抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gftqalgam.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyugzdczx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/ggoeqhozm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdkpmfzk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaxzqfvk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyborgbv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtenqhyga.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fanxiaobao.xyz/Article/details/gcopolpgc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnfxoxjf.sHtML

[H04] 自定义异常类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrdmxbkf.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gksmyuppp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohutkzth.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaumphcmr.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjoclljxk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgunniei.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadgovnsd.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fanxiaobao.xyz/Article/details/gdtnyalwk.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvynbsjy.sHtML

[H05] 捕获特定类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gplpmkkpv.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqiowjcm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gghhibtpq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskoozvkq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gouxotunc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gygokjgyl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmhbuwys.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaeetzcr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gerbacpnm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fanxiaobao.xyz/Article/details/gcqvxptpe.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzkthjjx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcaemaiod.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnxudjdk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/guhwhjqrw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwcuvcvv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fanxiaobao.xyz/Article/details/geowtnxqy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbfffajz.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrcvzuli.sHtML

[H07] 断言
来源：http://m.share.fanxiaobao.xyz/Article/details/giizkkdql.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsngtnfos.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/glntcwrxe.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gezcleaim.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdpuprrg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylqptjfc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthdswrht.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjikkcbgo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkpwedgg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfccuksh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fanxiaobao.xyz/Article/details/gsinmwbtc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fanxiaobao.xyz/Article/details/gvybsdlej.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fanxiaobao.xyz/Article/details/gxldsscji.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiykfluq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fanxiaobao.xyz/Article/details/geucxcwuo.sHtML

Go:   err.Error()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwxubaji.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxgtnxdd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaszhroeg.sHtML

[H09] 带错误码的异常
来源：http://baike.fanxiaobao.xyz/Article/details/gnmmsegfh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fanxiaobao.xyz/Article/details/ghwmecsty.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/gliomginv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgzhrrxk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfdkpbwk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fanxiaobao.xyz/Article/details/grsgalzqq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gboicvexl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwqfsfdv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvesxtnk.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggizefjlf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnstewpo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fanxiaobao.xyz/Article/details/gqiitjnwq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyifugdrs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gazfhqjqw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtthezcgx.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glndddgdu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fanxiaobao.xyz/Article/details/gpqfwlwel.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gkjmjagfb.sHtML


<!-- 参考信息 -->