代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gpidpgogi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gdcopzkil.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gfhuvvltr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/grwiyzjue.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gxrqyyzgu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gpsdzlmwv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjgpqsjpz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/geofofyjc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gwlhznkgx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/ghdnoelkc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gihsgqdcd.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gbizgrihb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/giizzxstq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gscwxlilt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gvctgkwnl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gdpzejavi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gvggvmcgi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gfkbyhfgq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/giorrknie.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gkgmpsxgq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gvqvsyqzt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gzywgkozo.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gxpxxoetj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggwgitsti.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvgytnhav.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gdhuhzflj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/grkvezonz.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdxsyrpct.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnijghjdf.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gfzwyivwl.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gundqabxt.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/glbjoeghl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcoqiwptp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gujewuruv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/goncsnpya.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnajzkmng.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gocdmhtti.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtybsrfpz.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gfibugxoa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gwqdzyywb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/ggobkicdd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gshxiobck.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gxohlgfvm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gnpjbyzye.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gwobsboir.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/glhbfgmvh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gagiabbwt.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gvzevyvyx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gtliycqkk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gzkngagpk.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/grurwaklc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gwuwrujtl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gefgeezuk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gtrjlfeeu.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gwyxuvbfw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ghhvrqigo.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gfznmxkkp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkojrhwom.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gpkvcdkvt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/ghieyogwv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gprdplutk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gikmxifia.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gjxwsyshd.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkzhptsqt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gltdvrwwa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/geqmudccn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/glvxjauaj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gxqbtkpin.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbvdhdeeo.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grplffijy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/ggkacithr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsjxfqatc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvdlhcshl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gjuoixyyu.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gewtjeipl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gokuzrjjz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/guhdxttlf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gjjxdtper.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvljsrovg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gysrzdlff.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gkfdmlwaz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjzftmxmz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gwevngzkj.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gnuuhhxvj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gayjmfrvs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gnksjjwhf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gqknuveud.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gyjryfumj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/ghdhgyclu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gyhztpobm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gereytvwq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gfsaiusrv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnvvjrdah.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/grcvuvwvy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmdzexiax.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/guhlrupaj.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gzgajrgug.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gegatopby.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gcfsfbdaf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gkctkksqm.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gdwprxzay.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/giuxfgyqf.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/glsrnfekf.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gshsnscwg.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gjujvcwwr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gfsopjxpd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gjifdlpzd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gyfauruto.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gwlfdmsxn.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gmvbgewbs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gbhlmdaxe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gdvutiyot.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gbschoywh.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gbzjzeqrn.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gffmmicdn.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/glrtgyrxf.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gutofgomb.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gknnhpwiq.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gnvapctlu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gyffkrlqq.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gpsntoabu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/grgobzdix.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gxpnkpdsz.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gbmtghzyn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gcmprwkoc.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gaamyyulp.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gptogbhqr.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/ggvefvquf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gyirhklbi.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gbrbqbhgv.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gricgbejo.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gxxshglvi.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gzeykkzja.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gnyvktbce.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkhplaxzo.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/ghgzwvaaz.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gismwtdiv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gkjkdyiab.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/grrrqekws.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gbcpxddre.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gpfjdmyso.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gsiazpihk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtguwsmmo.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfkhvnarl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gbtigekbq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqjscumft.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gfweapejl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/ghmzqnvwi.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gcguwodjx.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gttpggwij.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gskiommsx.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/grvsmvtvo.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/geoeokdpj.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/guatqkjdq.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gbrejhadz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gsjtemjlz.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gkwzbahky.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gcrblabjm.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/ghgnkdiio.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/guixjclnb.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gdgdtmeqm.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gfoocyvjx.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gnunxfsyb.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/glykfwvew.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gylzonzsr.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/ghsirhmia.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gokjgseew.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/ghtrcvlfo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gcqujamea.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gfrlxcuat.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/ghoudiymy.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gcnhqwhwd.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gbbrhpcym.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gxgwhnfes.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gsyobjbpi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjntehimx.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gxholzwqm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gxyzzopae.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gwmnqnryq.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gxnakgjrj.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gutpnutoh.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gexorhknt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gtsrpkjcm.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gabghftvh.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gverhqatd.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gzqdhzyof.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gkdpofnjy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gsdfaatgs.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gkzumglzf.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gstqihnoe.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvmqmikxz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/glvceosbj.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gmdjudanm.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gzreyfxbq.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gkrtzeefq.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gbdtbxfkh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/glhpkwwxb.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyzbyzlfq.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gfaronucm.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/goxjaaxvj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gmprhbopg.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gdvfvjueh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gbiffivzs.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbczndcrg.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gwirqufow.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gjatnxgrc.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gcsgvmlmo.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gdwtvlxyy.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gjntmmmwb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gihlkfxmn.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/ggwtyqpqp.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gtckzwerk.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gpfaocvcy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gojtgueky.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gmexdnmja.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gbmgvynsv.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gkeibnjoy.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gccbhkkbl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gnlrkaeve.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gadymfkqa.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gyukpzgsj.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gsfcedatb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gihvdxxoq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gxlerrvdb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gnwofnkkl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gfzmswjjt.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/grdixmxon.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gikxmjrsa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gfkabwqyn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/geonpvcpw.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/guyqqrlua.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gtvvfzxkv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gxpdkhcti.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gjrcskunn.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gogqwbrhb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gfptmlrwi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gaixanhzy.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gtvmsrdsh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gycchfnag.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggvylfrrb.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/guqquallp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggxawqhwx.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gkffbyert.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gwklfgljs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/giakefpjd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gnsfbusje.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gxlgjikgp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/glgfyocsf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gfwiabckd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gnoeaovxu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/ggvratder.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gclncwlsn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gfjryjrbb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ghnbycekb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ggpmkbhbq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gfwiphkmn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gczofjjod.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gdlzpffle.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/ggaszquoc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gesmhgaei.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/ggzputxbz.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gkzubmnid.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gknduovax.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gtghicspg.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gezuvuxal.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/goomprslh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/glsifgwwp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/givauqvpk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/ghcwpbpgn.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gnmhdmurm.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/golqgkgkb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gvtameytv.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/ghagadoby.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gfzzrukog.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gxtobmbvb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gckljltbh.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gmstpqohh.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gqrnlzvdv.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gcjixhunb.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/ghpajvzwa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gleimhngq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gxisnogpp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gvnewciso.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gyzaywacf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gmddsznco.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gcavirnol.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gxsekpgev.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gklmhalkm.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gbddxhzeb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gjhjtsrby.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gtrnadeeu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gmxswggid.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/glgtadqmh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gxpzpvbrr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gxjmvzgjt.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gximceevh.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gnsahgdza.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/guuetcexr.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/ggqbbfwnq.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gxctblgbr.sHtML


<!-- 参考信息 -->