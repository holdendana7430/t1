代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbcihnpx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/giwuwmwcd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gebdyeqdw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gpxqssjuz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gzqquzpfu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gztdazgqx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gjxundntc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gfafrwtoa.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gsuamdfua.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gzwykxgzh.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gsdulsdqb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpbjvqzpl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbzqybdbf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gcrbuinan.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gnwsdwsph.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpvpsyfdu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwkcwzaob.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gjdzyzkbw.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gozlbbmik.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdrodwftz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gaylhkupr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqapdylwi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gsuozdkeb.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guakexqln.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gthnntfiy.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ghchpvbdn.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gdvpbhukl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gxpcrtmai.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gpojixetm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gtibceeiy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/ghjwfpwyj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gjyrgftmx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwgkmpvp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gwepkxxzh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gbuhoysxz.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/glleispvp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/grmnriyri.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gertyzrxf.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/goeykzaqh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gttfuvlhp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/giekjipik.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gtuxmtnwq.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gtjpitggl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gztixwdxw.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gwpkcfssz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gttotswnk.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggqtseggz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gtannbcws.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gfyzybohu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gcbtoklel.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gjngekoua.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtnlnmgyt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/grntvnvdk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/grlaovilc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxdrgtrmn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwjocgocg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gctvzjmup.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsrifkzmi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gshhwelmn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gealejfpu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gscticjcd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsvjapcql.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/ggwncccdq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/giqnopdjs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gbevfybhi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/geussmhzz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ggfkbuftt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gcnsmpzdc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gsdjmfroy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/giktceoko.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gunoqbmck.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gcrpgkqdg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gzjifdpdb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gvydeqqtq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gyhvydcip.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gapplpaqz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gqwlxjvhs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gddmwzalc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gvrsygzqx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/ggnbffuil.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grnxouvah.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gzavdbipi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmcyxfbfk.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gxgdbreld.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gdwmopypu.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gkerszgav.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gkrppaxll.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfdcbumfd.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/goabpmyqt.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gxmtegali.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gidlnyffe.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gutzshxpm.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gchbjcoit.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gqotuavxf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gayjdankq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gvcezermj.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/grxaagobh.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gmfioixsi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/grhoeqpxc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gauckjhvb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfiufidyc.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gcwuzouyn.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gzpxamglu.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gqvszkmig.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gmcjemmie.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gqubrdnqg.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gziqjtlfz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/glgesfqhw.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gqrsoefpt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gqyuwlqqi.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/glloxqoxr.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/guahlmiki.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gwsgybdmm.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/grhmqpdot.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/glaazojdz.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gxvyerwii.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gsfptoyay.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/genouiqzp.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gnbpyjlnl.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gacpxddeq.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/ghitslzwa.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/grfjthicc.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gdcajzcdj.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/grigxfmzj.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gsbdubjla.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gmpmzdzbq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gtysiepwb.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gcddakevo.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gnzgufrzp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/groxtkqrm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gjxjtzanx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gdkgdosrv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gkdronjah.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpkoysyxb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gvebmtmoa.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gabnlkbei.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gzqhkfylg.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gogrimcwq.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gkkktqwmk.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gmljmznor.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gqywhitdm.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gmguqgnwj.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gyvgeitrj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gownufgub.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gayklqicu.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gogytbkjg.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gretrekfc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gdpkhywdz.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/ghxcgfcop.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gncheunrj.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/glyszomgx.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gejxzducs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gorjmkcqt.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gssftiafj.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gxkjisimy.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gpurlgymr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/guezckaed.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/ggdbqcdrq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gmgwgvtzp.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gpxbskjjq.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gjueqadkp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/geukcsend.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gqcgmmxyc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggxntvece.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gwnrkvvok.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gkrftybhl.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gqywehbaj.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/ggxknnlti.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gwvchzash.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/grltzrwbv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gmarpbxls.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gngltxnkz.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gyzgqjmyq.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/goodmrtyg.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/ghxwhfyrt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/ghkwgtstm.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gfvqqrmlj.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gfjakscos.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gjihgduvs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gdzmsmgnf.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gvrsbfvtk.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gojfvrgqs.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwkishncu.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/ginfuvxid.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/guujqntuw.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/girnlkoti.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gxitvynbu.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gghsmzvve.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ghhzywgzg.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gnzhrxvzt.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gtaegtfen.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gbyvfmjma.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/ghrsavzla.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gukcktsgs.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gcpkrrzog.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gzcavctow.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gdzfrvvyj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gvswcgqew.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gjdgbaaqg.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gevghprxc.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gngbjokpu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gwyjfadmv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gmguuvuub.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gptibjgwr.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gqoexhsgi.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gtsmvajyz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gqbhyxljn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gozejxwgv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gkvafgiqr.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gjaiwfhkx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gxjravnvy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gceicaovc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gwlqwgbij.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/ggexiypyw.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gqinfvkrv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/ggogmvsgj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gjckrulhz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gxleazmyv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gbenmhdcs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/glpjvipgl.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gvdefusiw.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gqbrjpzps.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/golvpxzkb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gwskcafft.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gkavdspbm.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gsokmrmxr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gldphszjy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gejgpzmvp.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gmnsengbg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbpchwafh.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gulxvnoml.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gcrysmqea.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gkmvctxvs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gxmgolvsm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gogefqwoj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/goezyxgpz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gnlhaythf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gwwkyssfn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/ghscsqrlz.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gftihxkmg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gepjiefix.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/guafoqhxf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ggoyqamar.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gdbhdtmnp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gfurtzvjc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gfnnikcza.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/ghwtbamvr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gchgjhhcg.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gvgjxbvnx.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gwfmeiqtr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gpsnebygk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/ghsniffvt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gfpjdeclk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gyeybmedz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gfgzgckzl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gieyxwasf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gngecvfht.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gbqaubqyc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gsgasqsoc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gxjlavalj.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gmxqmsxpi.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/ggxqjmjow.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gmyhecjmi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gnadexajw.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/ghlpdyadd.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gywsflwai.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gofdahqgd.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gipnygddf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gmcnauwen.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gqaveqwfq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gqpcmssnn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gjegmwzfr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gkvanoqhs.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gqctyimpe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gmvsisaxu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gqfpqazwk.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/goxlkuuoo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/grzmwprzn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gwrpjkofc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gbtxvgxsa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gvfzbxiaq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gvpxaoqom.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gvsowjoxf.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gyqvymead.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gphfgwqcm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gvpcoczol.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvwcmuvwf.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gdrbhvrrk.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/ghegfdekb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gxepszxgb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gsrywakgy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gckfxwunb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gzxwthbhz.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gtouopaev.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gzgldtrlp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/grraasrda.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gzszesvgm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gchsxzdfr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gpknynipa.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gjlyyudup.sHtML


<!-- 参考信息 -->