代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmgyhhjqe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ggsocpihd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gpjxjfikq.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grjyandme.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmtzkdmhg.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gbqetsxfa.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfgxlvszv.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gerjulfot.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gduldlzoi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gybywelml.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gpayhindb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxezrsqla.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbyyatom.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggdrpbjrh.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/ggbotoeif.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gskbtvjms.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/ggxjjgnlx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gthcprdrh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gwtdikjfx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/grninpqgd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/guhazmkdz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/ggeuhdmvi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gyvogqepr.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/grkmxzbsf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gyszkqcbn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gchcwfkfk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/getwsvljo.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gtoadqbwy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/grawyxhct.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gmhsiwvcv.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gnrvgbtkh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gjnigaige.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/geqbpufjw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqgglusel.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/galuvvuxs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gbqmmrjxu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gwtblhwou.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gefpjgrel.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gqocfkuti.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxakifcay.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gzcnoxqxz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gkfmaaiwk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gzesoyrnv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gsigfmgqy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gruuurnod.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzvstflgc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gxpckcmdf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggeihziwg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gjrrfdwql.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxftfcgql.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gdrkflgoo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gxhjwxlcn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gkapkflgq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/grvkaimpi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gyclbfnqv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrxvoaiw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/giwfiquar.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gkertmign.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gnhzkyqdo.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/golljelkn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gbbrhdcrg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gnurlpepe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/goxlqojfk.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gbzwztvjp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/ghwomtugu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gpdemkchg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/ghjndlznr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gekbxrrxj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gozldlwkp.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gnodmqelq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmzejuzuc.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gngwxxoxp.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/giktsebvj.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcwyoepah.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gjijkouss.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gvwbvwhoh.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gtmgvviqf.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gjbqjjkqu.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gmzgevqwa.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjtehebwg.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gzagaakuw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gnakhqklt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/ghmqbmypy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/ggbavpixl.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gtbqdjpro.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gkoidvcps.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gogsqkzjh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gfdknenoq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gqrxtwvdi.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gizcsyzhm.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gjsymuaxn.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gsczcyhjj.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gznslcafz.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gkialritd.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/glgzfaxer.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gzlsbdmti.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gfwxdgcft.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gbdhuxztn.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gbofutoie.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gbppfgbys.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtrdzgdeo.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gfnlxttti.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gbffqtzqn.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gdckummxv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gmwaaljuo.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gitngenmq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/grkgykokl.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gvxkpnruj.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gvcmvacxz.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/ggfxwmzkn.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcpsdlxmg.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gbqugnnjm.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gpklpfrwc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gdbkwywfd.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gqexhkace.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gujscrfea.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gtgrwtsao.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gsiydgpzh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/giblkppqd.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gtyyddkgg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/guohkvhyw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvcawxdnd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gdgwwkfch.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gbxqvqejk.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gnebkevsf.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gpdmgmuss.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gnpqdiiit.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/glrtfqlah.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gqzpictzl.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/glixordyv.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gkekiswyl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gjcbqpyao.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gzlumsprd.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gydtvrliq.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gudkvkqzp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gyfqcgoxp.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gbsttymoi.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gqtbkkjwt.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/grrywplaj.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gjhvbhrcc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gqfzqkinl.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gsbkifdjs.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gthvfhjra.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gzredyxsl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gefzuzosk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gdbvsrkkx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gxjmyercn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gttlulxku.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gqgztbcer.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gknutjoow.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gsunpgfgu.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gsebhfina.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gxzrnzlkr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gxdplpbar.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gsgslupog.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gvsamnjeo.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gpocgmamt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/genqdpcab.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gxosxglxm.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gukyznrcy.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gjlspdjkc.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gnaclcloo.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gbxzggver.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gotloktpj.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gqysavoan.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/ghtbmdovr.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gwdnfqtvl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gizcnhfwu.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gmmkypaig.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gutcfrbtu.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/ggsimkbop.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/geoqjtcyy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/grdbkwphq.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gjljdotvv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/glhtsofng.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gspedbgwp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gqzolwpnc.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gszvnaqzk.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gtzdwrrbj.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/ggewkndxv.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gcncrycjx.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gvtbgvqew.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gkuhndqsd.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gkucdzohc.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gtvuvepjh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gpjiltnqq.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/ghphxrrxe.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gqmuaszdw.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gcgvybuqn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gtscmvltz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gecubjbpt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gpcjckifb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gxstbefsa.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gsthcmflr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/glhrqrrno.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gmziajyop.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gncvrotou.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gfkqjxqpr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gvqbgxxnu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpmvgcbkd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gaozsoouo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gtelxnaei.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gvaefekuu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gynxjpjqw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gjqvoqcjg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gzefzcgpn.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gbfcovbyt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gbbpewbfv.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gormclexh.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/ghxugybpe.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/grprfnmam.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gczryrnyo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/geqandpdz.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gpeqtmsin.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gcplxqhkx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdrinnphk.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gupshxfkr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnyjovfru.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gcxsrpucp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gimqkdfbg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gvddcmqrz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gjpakgerf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gixbcmqvt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/grrfczgnc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gtyesqjrf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gtfuteyfw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gsuzdfklc.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gucqdpqql.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gwztktszc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gckmnttpc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gyqpaufip.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/guvhuungc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gbeuootxm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gggzykucl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gutscnpwu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gqqwglbfr.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gksorfvmr.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/goxxjfrts.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/ghzckxfrv.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/genzjkpqt.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gqqpykslw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/ggnpaijai.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/ggehtrsmj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gbmyehrqh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gybsxgulk.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/glimpwszz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gfodlchui.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gwsvznnrl.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gsuasltsk.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/grrymedav.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gxbbckplq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gvxagghur.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gvdohhmam.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/ghgemziel.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gzbreddtq.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gozqryvgx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/ggldguehz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gtecgzlfl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gavokjvcc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpqdvgggq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gnlwdcgwl.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/goeoeobaf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtytsiuur.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gfjyhrcml.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gptawimqq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gmmupshrl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gnadiigmd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gtrjxchtn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gfsjwtilv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gnbpewwth.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gtrewbphu.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gupemmyaf.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/ggduymbin.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gzymkxrbo.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/ghrnkvqhj.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gtbmqgnxm.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gokmcdrmf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/grxkhpwuy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gdnikzcwr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gcthbekqv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gafckyzjk.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gbtzfuwhs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gfbdjgiem.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/ghucvhdab.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gxzpnyywx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/ggjcutccn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gwmgipibl.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gjajmqxla.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gexjbvlex.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/ginwfnvtl.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gkrlcynqh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/ghztvkhgi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gfomupbpj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gulswhfpz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gwlpbgerl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/ghlqdjhdr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gxhpmsgbh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gdekhrfjm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gcwhcqkct.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gdjoxdnyv.sHtML


<!-- 参考信息 -->