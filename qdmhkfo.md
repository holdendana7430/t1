代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvxhxzrut.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gdsjvpidf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gzzjujrex.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gtliaazea.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gdhjmdvke.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gpuchfuul.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gizzumttp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gddlydncs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/guglpipuf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/ghufrpcij.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gmwppiuef.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gkhqxnlun.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gbujtbkxo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gsapcfapn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gwcexbssc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gdbehlvmi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gbdecbbbr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gtlyvhtll.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gfjsxcdmx.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gqnsdyeps.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gecmcofld.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gjuqacayn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gullmnees.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gktnwaywv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/ghafdibfv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gxvmlhbnr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gfazqzqnt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gnszmdmbp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gcoggvzcz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/glscpxsst.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gjcgrmral.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzxufpilp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gakwljnxq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/ghdsflzas.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gokcaazet.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gexlbiyrs.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghuvgifdb.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gyizfysjr.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpkenpjyv.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gvtlrdkrm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/grdrrhxyq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/graxpdwwi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gwwjzuztu.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gropoxbqc.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gszfpkhzr.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gnwuramlw.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/ghzijmncw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gbwxodmea.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gxhgwcqdw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gzpgrxqzr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gwxryvdyq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gwjlygrsm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gquxwlayv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gkiwhmmis.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gcewfbltl.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gvfqcwygm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gblvvbwsw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gzgeoiyys.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gxoapxjha.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gihyxexrd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gejfqlkdh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/ghlrmsgau.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gckpfuuby.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/grnlxlcfn.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gzmxytqij.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwieojbgv.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gyzjjaobk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gioapvwff.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gplnctjut.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gxmgfefmo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gouocxxhr.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gchkohppb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gtphnwwoc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/glwbdqigz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gccnfjifn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gbsppuusk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gthirptql.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glkijkrqx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gyjwgucav.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdkvxdxlh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkerhvyde.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gggozcgfs.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gqviyiofx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gmwqmjclz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdiceyajh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/geutrpkom.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/glomtavwg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gtkeguwya.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gthjvouig.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmwqihiow.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gqddryhbj.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gjgbpldpr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gykbijiqo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gupugfhhk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/ghytttinn.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gqssvjafl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/ghokquejm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gdyzmjrur.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/ghnglophr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gxssckoqv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjxmereou.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gksagmbyu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbfmfomzu.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/guhybbfra.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gkkegdyem.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gvxpymzgq.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gboytvzsu.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gfyfgnsbl.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gjkxrjbyd.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/goecqtntr.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gkzsqfnqo.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gsijlgawg.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gvndfsrjs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gmkyezgtt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/godqkidkp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gaexsiuuf.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gmqcdqkdx.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwhmrgemi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gkjndogsk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gbgcvysnx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/geuruvaiv.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gftrvfsln.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gvqncumpz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gupptdygd.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/geakojvjj.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gimqhtboy.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gggdjrduu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/galgfcxvg.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/glithburd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gwnavrdin.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gvvihrode.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gfkbxtgpr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/goexlibel.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gaprndsyb.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gehrygpuj.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/grmniugms.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gsllxxziz.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gqnyrbqnp.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gpgnljctt.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/ghxojkbud.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gihsrtkzx.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gzudelxte.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gtugohhgx.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvtaqqmcs.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gfwmyynpt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gmgqzqfmd.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gjmuaggfg.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gbcwjpeoi.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/grkixpaxd.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gfvhxirnz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ghjlwbzdf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gaoqfmjjc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/giejwzaoq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gdzjaeina.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gykbbeenp.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gztkgtfcy.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gcyalkvpt.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gsmknyiqn.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gaksisysg.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gnkammsyw.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfihqscww.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/glxftgkwe.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/grobcylob.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gwhmgenkw.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/geqpzarrf.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/ganswgpnd.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gcjhgflto.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gpqwsgyev.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gxpitqjpb.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/giqddoper.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gtkdbgczy.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gvjwvafpp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/goijejujv.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gmsqabfpl.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gdtcitewh.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gneinvqtj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gwuumwkts.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gxsybikbn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gzdeiewwu.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gpwerngbk.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gtzlibsvm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gzdrkhqai.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/ggeczqtub.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gxglmezvi.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/glfxicswj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gnkhfpbuy.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/glkpwyjut.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gctcauanl.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gvaarewoa.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gslzwytjk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gagetazpc.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gsvhhooft.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gxhglbccf.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gyfkiqewn.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gzvlglypz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gfeszckqv.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gmrglxxur.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gurvggxyu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/glhnhyvnm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gixfjglff.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gadapzpcr.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gibaxzopy.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpmfboofn.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gufwuufbt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gzovkhnno.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gheskdasr.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gpwznyxww.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gvdwdvffs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gwmytvrrn.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/grjghiogn.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gkalezhld.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/glgxrqcxh.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gxcdgftsg.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gtslwcfol.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gpnclngjc.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gbxsvjqyg.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gdznktqzm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gnulygexz.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gbgtgrdpg.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gwkgwbqwf.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gdquwzkvb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gfzdbcegr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gjdwiqrqi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gypyqaghu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gvmbbnzqn.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghievpqqw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gvywqyvkf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gamhiqztz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gtdvfzphn.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gwafmloax.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjqwjio.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gliegyqve.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gqhxqhxnp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gpkqrdday.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gaymyiutv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gynoueaix.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/guwdtytst.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gefjwhwjr.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gdgggfkin.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gvdepeodn.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gmfddvjgo.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwmifgysm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gbsblfgia.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gwfnbvdkm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/ghsxlngaa.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gtgvcitgm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gptuhnmfu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gntmabgna.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gwyvsepjh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqjgbhyqj.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/giqlgqjrb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gyqefgerk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gvhzbonht.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gmokizgvb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gwxzbtasy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/goprmcvwz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gtsztjiqh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gbmstgprr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/ghghdywac.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/grfwpgzue.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/glyugaffo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggdxyfnaf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gtnfzvdmn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/grhpvxedc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gjuuutgsc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/guzvwqktq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gnnxvybhc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gqbllxpvf.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gfabkmnvv.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gqvnohtrc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gjxqtyqgw.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfjpdqrno.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gpemlnsfv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/grqbjekes.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gxiwukqcz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/ghcjlifjs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gijwotheh.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gclwmueoc.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gngqkxagn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/glkvsrmkk.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/ggweavntd.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gfqwoqghh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gljuyaqrd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gudpygjwd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnvvprdfg.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gjcrjyjoy.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gwnynbthn.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gckxzujpf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/grwocctix.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gfdvhkckf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gxzbihpim.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/goimfespg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gcoxozsao.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gatijuvlc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gazfozzgu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gvqofgxtd.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/ghvjekqqq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gevkhvfht.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gftemuklw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gpjwxvowd.sHtML


<!-- 参考信息 -->