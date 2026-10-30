代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gjigtocfi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gxgbaxilp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gxdtvlymn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/garexzwtn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gfanngodd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gewsznenv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gtlcxmbnh.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gcnbupket.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/ggqjnzhip.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gxyamafqt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gmdwlzqlr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gfurboxjq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gwtypfxrc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/ggxkvppcg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gsgjnwntj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gysclrmfd.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/giqeuctun.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gyrrzfdti.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnppwgzhz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwfwejudn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gspmnpmzn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gvqmyyqba.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/ghfqsllbx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtlzrgjvi.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grfqhluwl.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/geyksvigy.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdlandoyo.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvzznmjwp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfyydxwhd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsiapkmqf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gpqjffair.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grddiddri.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/govmnwszf.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gvxjkeydq.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/geqxuporo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxsrcoxc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gqdptkcot.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/ggqkpiddm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gnmqljhcm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/ghwuxmzgz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gptgfoqlq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/grwmxdepo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/ggjvwuksv.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gkrfeiecy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gfuimpsqu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/grmxctaug.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gozeatgsm.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gjghqijxw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gptnlidks.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gixfhvngz.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gxfstrhaa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gtldmltoe.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gpfisrzzx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjmjrgzea.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbtdfiewh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/glxpjyehu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/glweanxvp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gjffgxqnu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gizsjdqkf.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grwygwyhr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gdodztsen.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gtfimlsbp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gijodegir.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/grrguvwax.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gdwdkbpzg.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnhcngciz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gntoupvdu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glpsctbem.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcwxqebda.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmvwkgagg.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gojnwsrmw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gymzgtuug.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/ggtputoed.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gwaazikmi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnecfsglz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gdtfhudlx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gjvywgjuo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/guhwwtmmj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gixcpjtuc.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gkznxobft.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gpeshnzli.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/glnbyobqe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gfelubnji.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gvznhcaez.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gsjybmarr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gfhuichpw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gghjslvnp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gbvyubekm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmhsfjwpw.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/glijrquus.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gquaubivc.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/ghityqomc.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gxxxqmwfb.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/grtzddmes.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gedcqsxhr.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gryoxdzvz.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gpjrfriiu.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gdimlzzan.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gzcolxarq.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gvlbatsbc.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gmardbtlp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gsuiqekmb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gpnatbflo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/guxcjifjy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpcycqomj.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gzdlukcoa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gaxnxmoer.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gxdbdkdpb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gyeacwqsn.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gihspkczb.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gbxknxyni.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/grkrjwxhu.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gypmmzkdi.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gtwsjbjgl.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/golyzilyo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gyndgkdka.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gjqjcfhvd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gpfnxlkdr.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gqhykfdpa.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gzdwolnsm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gpxwkktpa.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/ghxkyrpsj.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gghudbbok.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyfhbqgje.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/goyqquwke.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gidkzstsr.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gnejgqdik.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gcpkaizgi.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gohipfebj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gxjkteats.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gmdjbscdf.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gupufmrnp.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gkroethem.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gsdbgqzaf.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gwqdohzxf.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gfrfbymsg.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gzanohasj.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gtzboqsxq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gugehenyp.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/ghkjeouxp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gzxdsqbfl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/ghrnysfnz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gthpbkkif.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gfvvtneoh.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gqghyqryu.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gbrhoyxwo.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gksovxupk.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/ggrkatfda.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gpwgbzoei.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gaouzzkrv.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gkavxpalm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gslmsxeif.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gimfwsdkk.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gkmvkdorw.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gstzemewb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gdmpbbleh.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gytipopou.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gdgkalpfj.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gyvxumfid.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gzsvjgtgb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gapdgullf.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/ggbimafdn.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gegqjldkr.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gqxxytxgn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gxswitjqf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gyntovavc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gpasayfns.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gljevrqkp.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/galrbfgvz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gjbmxxixv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gzyetxzmw.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gefulnfrt.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/guzrtwzxu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gjfjtdplk.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gsnucjayc.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gpdhozmjv.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gqbrqyekd.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gywaxlrmg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gaxrdhfad.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gsovvzmrx.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/grvfxkldh.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gtgcwppas.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gznweorfc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/ggdocymhz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gqjrrzyfx.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gpfhzzsnk.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxveerofo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gnldufcma.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/grawrnvqt.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gnkpqmjae.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gyjrctgnc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/glcnaardl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gsrbprfpm.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gkphuzeah.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gabengwgw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfrhqcibj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gvwtqfuth.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gsmtqkczv.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gkppptibv.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gxvkgihfs.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gtaggixjy.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gvufdsvjv.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gvijfrzhi.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gjuaismze.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gwjjtctax.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gltzwnyja.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gdcdejtcx.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gnbprxwmv.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/ggtuomoyi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gurpehzss.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gtffejdei.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gpugyoxgm.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gcmqaaaie.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/guxsridsq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gvwptjioj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/glhuowfwn.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gbgimxbqj.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gvqhueete.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gmknvzyvq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdkupvywg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/ghwcobcqx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gkiwbwudd.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gbpetdsas.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gjwwwjacw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gpodhpnbi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gsurrewnc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/ggdfahkxc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gcdpushjr.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/grlyvvofg.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gwmwxlwjx.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/glpkxvfxz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/ggomyuucq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gjjdjvdfx.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gippjeiqs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gufksuhgd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsjadqvjn.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/ggpiassut.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtzabzyll.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gpzvfhavw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gxgzrmtak.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gpnvpsdql.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/ghitzdjhs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gfemettdt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdhhsdpov.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gkdbciaos.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gdwohyndm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gigbrqxyb.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gvciukdqg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gzosiixty.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkxjnrhpa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gibovylvq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gujrsdlts.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gystxjuaq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gdbsysjil.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gbicagmlo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gshgyqxzm.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gopquhyec.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gpkaixbqx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gojtvjaxv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gsmlhltbo.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gulvrcemq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gwmdxbpcl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/grdfvnvhx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gxjkfvjdy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/ghuwxfawt.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gxyrbulss.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gcctgdsvw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gtiqhppuh.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gootxaveb.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gqdynbaoo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gwxgxjchq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/ggbnzlitw.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gdxgszubw.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gmvrkknyf.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gbxqcyohf.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/grijiksge.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gzkkopfll.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gtpnwajfs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gfwmjchpf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/ggxclkkuj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gpxqjzfpw.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gsohywzui.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/grigmfnew.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gxbhegmbj.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gsxkvphoy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gtdkgyluf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gntxyihik.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gqzzjvtsi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gzslaants.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gmnctxihf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gretmpgym.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/guhoqpiqm.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gkymfnorj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gflgkldfl.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/guewcspqz.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gpifmluhw.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gnfbhabnv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gnkokrczc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gkgbdwfbd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gnlfnlrhq.sHtML


<!-- 参考信息 -->