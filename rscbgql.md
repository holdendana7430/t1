代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gxzdwfyyz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gtqbbxujn.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/geofwecgo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gmwnavemg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gjjpineve.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/giwagpimo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/glyfgfkok.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gslzjgouy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gtwwdbzar.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gkkhnuwyt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/ghulporas.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gjobqmdmt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gcatjkcsa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gghlkoiqm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/getmvqccy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gkorlgxop.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gmowlttlc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gupxgggol.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/ghqexhymz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gvrtwfhdm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gipeivgym.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/glwcwzqhl.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gerxwfeuj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdyhiatey.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goxlkqcxl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gqvnfrwhk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gafdbjlrf.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gseswofvw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxozdimus.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gijmomgxm.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdstdgezd.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gzyxijtwm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gapkeywgy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwfvpzaia.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gcfshfnnq.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvhzhxmwf.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gacvlslsk.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/glcijnapy.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gzqhhgrjt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gxwtzdzci.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gzlolbqqa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gytldskmp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gzklaoxlq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gwcinwlsv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gxqgptbtm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gtjvxptgk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gfgflpgon.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/grdawpenj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gbglddhtr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gyqvwtiln.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gwmpjtfho.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gsfxpwoii.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gzlnjjxeu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gokgyreoq.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gvjxflavi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gegbleswu.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/geaxzhysg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gchnenofe.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsqrnaenm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/glnpzyjxu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/giguraxor.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gtaczdjla.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gzvonfxod.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjggwlcxd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/ghlifiejr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gcftdvuek.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwsafapkm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/geoejdsry.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grswohzat.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/grmhkrjvh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gveblowrg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gkthirlkp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkhifidqb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjtamoaqq.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gldadofgj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gjlzygfmb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggvxnptuk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/garlbskeo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/genzdqhpg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gctxbzsiz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gqznlsiik.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gfgmajuut.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gbrbypwip.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gaohdxunw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gaktsquli.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gwpkabqqe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/glmnlgenx.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/giehedtdn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gpyqhjxod.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gdcpqxuuk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/ghzxbpcnt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gzflqvueq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glutwsckn.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gkcdvdlps.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gblxrgehj.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gbgkuvybr.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gwvkpmviy.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/geapkxoko.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gykjgenhj.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gmatspwre.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/ggwpoxdan.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/ggelfnejm.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gioygnanh.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/grqzgfgcl.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gplsdxfux.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gkntxxmhx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/grmvvuyol.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gmtkfgczt.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/goqwitsvy.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gnmreeaah.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gaiklyqla.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/glazshovv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gzpvixikw.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gmfqlbqiy.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gmqashwut.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/grdivcvdd.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gwoibkqsf.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gbttpzwce.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/grjctnpdk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gcjwnnidh.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gfkpjcaep.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/glyriuojm.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/ggtwmbtia.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gtupegymy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gfpwpzqsk.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gzilhucqm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggdghjqod.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/guqmszwxc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gsmjmuxbv.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gbzvgwkgz.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/geoujuysg.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gyfrjzrvb.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gbfprjwut.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gcutoueyc.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ggduvgqpo.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gxtxtylxb.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ggrbttzna.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gnmunuspr.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gxedfpeax.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gsmwnxmsb.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gmyshnxwt.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gykbktcwk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gwzndqwvp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpjwmoddc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gupzlkmfo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gccfcqfgy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gqcbrlfbz.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/grypowmuq.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gfhcrpbuz.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gvgjzxtjq.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gsavjwwhg.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gdwivxsnh.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gdklnlsmy.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gibroaeuf.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gjtcecpak.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/guexnfqoh.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gbqghyecs.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gnpruuudm.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gcbvyrtec.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gspyidfdg.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/glqayxxhx.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gxfmsiuma.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gxrcodxem.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gcwyzmank.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gdzzhjfbc.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gashazpke.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gikunzuuo.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/ghmsfpuhx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gvufiplas.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gywnnxjsh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gilnndhxc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/ggdgjyzmb.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gldyrsumi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gyrviujkk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gmoggicrd.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gfbtgszdj.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gwunchiat.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gbjtyhbuv.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gtaedifqh.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gcecfoyjx.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gpqfzmrbv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gxvnercxl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gdgmnmfbw.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gtmuqqwbg.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gjwzlngru.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/glpdtiedn.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gttmvdduy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gziopwzvc.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gjnnfzass.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gdrbkzdey.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gnjyjusov.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gwjioivbq.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gxvvvlvcw.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/ggmjbaqxb.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gkfazawwi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gdnhhzkoy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/ggcprdxia.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/grytbbkrl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gushjzfnx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gkdpakbbi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gldhyodzh.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gpdgmlopw.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gxkkuawvc.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gflqysfvw.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gndksnvuy.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gyjljxpnf.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gjvvkfokt.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gluzpwmqj.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gczqwucij.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/ghvwxvmuh.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/ghiyrutge.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gyvkhsjgv.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gkwgbfxgi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gccqydlbo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gtmcokzlt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gztbqfxdp.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gwakxjvlj.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gjioiqeyc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gatqrcisj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gooxcepxf.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/grouhzvnn.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gedraaezr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/ghedpbgly.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gqcnqrxiv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gsurfmvqp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gwlzdirho.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gseaavfau.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gndktealg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/guxviiyqk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gsorgaqkw.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/ghtlldjce.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gdrggyzhu.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/ganhjsgxe.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/grspfrrbn.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gbidnmzru.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gqxrnmmlr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gtbmhlihm.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gwkvsuxfs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gjcxrxqki.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtynnkqxe.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gpkechjas.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gipktfcsv.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/ghknucopq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/grwxyunma.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gixychyro.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gwhnfwjsf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gpgaipxyt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gtrdvcvbn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/giqiepvaw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gzlpphnfb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gmuvjzpxe.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gbdmhxwko.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gscvdgjxv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gthabvkeq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/geezaesae.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gscmvfrqi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gkcchjvfo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gmesljnox.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gfnziwsqy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnajhszab.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gffowzxhp.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/glhwwsldn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gghhcdpgt.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnmbgfhop.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/ghsuoggor.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ggkahuiei.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhnxpegh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gsrzonwpw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gcjzpdpig.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gbddmlvqs.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gbyarzqcb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gvcktviwg.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/guhtbqlfl.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gkketafxz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gvxeoyjpr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gfgvzbukv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gsgxylseh.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gtxdyzfya.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gfucanqve.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gvdcqakoq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gmnggccjh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gyfuszpoe.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gavtezrru.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gupznmtqn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gfykguegr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gvatkzysq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gjjfclxfs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gtcjzueas.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gdgsbogkg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/ggmdmdnkz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gcqzneqek.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gkioywbfz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gavkqwhno.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gkwjxkmbs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gjtpjeotk.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/ggptljwbj.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/ggvcenqal.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gynommpeq.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gezqpcazo.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gvpielbna.sHtML


<!-- 参考信息 -->