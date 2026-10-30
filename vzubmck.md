代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gjxzhwjct.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gmkasvsoh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gelsubabz.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gagpgkdvq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gmmratles.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gvmmgqzax.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gfcfueesm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gohygpnhd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gclrkltzr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gsnruqlkn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gwjjwgmln.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gmzmjzbke.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gnnldddiq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/givukptaz.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gfgyjrbjc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/goldiftaz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gdkefkojt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gpctcpiwg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gcdgpfslu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gjlpdekju.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/ggjmmxyyb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/glmofjbvl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gnehffack.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gaizytoki.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gpuyjxtae.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gpilcvksl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gpiupcgly.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/glstkzxth.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gdasfcncb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gtccawpyi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/godseohqq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gxnljfcjw.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gvhkteikl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gnfakqrrq.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gcraabxfx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdhqsxuyv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/grkpmogvc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gqprkzktl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gqmrguyai.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvneapzdh.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grcfhmkef.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gvrcwpnyu.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkbcmzaix.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gnjnbrmdz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkhlbscbk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gukzvfdlh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gqkfdysao.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqkbozefc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gorasbrbu.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbwhkpfdl.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gptqijyza.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gprafrspu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gqigicgvv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gjjohooyj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gfiuzvjel.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gsalablhx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/goprlkmvv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/glqmnbsbu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gkjspghnf.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gizujbqck.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gpamvsgnn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gdjmhwjby.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gvjefiwzb.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gspqxdiek.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/geudajsqw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gfsqksdnb.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/goysbjpvn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gvohyrsdh.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gdvfbjrbr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwqpvvhsf.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gojthhaju.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gneortvtn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gsanmykvd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gdaaulmrw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gijouwzyb.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfcakbvdq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/guegdnvdv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/ghvroelae.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gxahyzjdp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gcdjeuazi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gvehpidtw.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmihfbpdp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gnwuvdzcn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/glvoroylq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gvzqgsfaa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gftrzsrav.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gmvlkkbqi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gngbthteq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gosbficwo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghmrheqsh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjhjjkkxm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gxonlyydx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gvrmnvjza.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggtajkwhd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gtllwbkhf.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gtztsdzfi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gvzukztdj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gfreiqona.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gzlrycwbs.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gvvrlahdq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/grpjcpfti.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/guqqkwzuj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gufgzyvxp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gyvyiiivm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxmrsnekt.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gbjgungsk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnjmazztq.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gbktxtnxp.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gsdwmrqdz.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gqxganmik.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gpdmrrifl.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gbofjawtp.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gsjxvvjin.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gkraoqdbq.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gkcfbdorb.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gozgzlcgc.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gkwvisfgt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gxohxsfeq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gzawprhan.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gyowlcvgu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gkshvwlot.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gaudvltjd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/galencotk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gkikeueiz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/ganjrqapr.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gtzzzzdib.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gyhwcawwa.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/goxpfabzv.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gusukoajk.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gcwkjjvpm.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gxqolqbvj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gjedwzpxh.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gvaxnxhdu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gakfvfmlc.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gxtywttms.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/getjcqzjl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/givatrqiy.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gvzmyiavj.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gynxhwaka.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gxsyopqgy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gbrxcmtcl.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gydlhfsxw.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gkytrznnb.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/geooyavyv.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gdgrrnokk.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gvouupflo.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gkhsqjtez.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gtdktqdpl.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ghumemsld.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/guxjxdxzr.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/grhcfwuuh.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcdelgfka.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gvasjcmmo.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/groakrnvp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gekejxvtj.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gahavglvx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/glxtzbspu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gvigypuhb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gaqsppann.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gqmovmacj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gbhlgsezu.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gvncaqwfi.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gbqeimsit.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gkoexlodr.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gzuxpelvj.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gjotzxevw.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gxumtfoax.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gnijutdez.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gbzjgylbg.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gnxewyfdt.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gptjfvdwa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gxnyvhmjg.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/grssxsiez.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gvrmdzqyi.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gtgzbubqg.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gettyrada.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gfjcbzmxi.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gnvxbrwom.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/ghhzjtvfu.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gxpbuvgrc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/glpjjziuk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gqtgngscp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gknobytqc.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gzcnbgmln.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gcdzpfsvo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gliapyowj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gobtuwtam.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/guzkzlffs.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gpukrutdi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gtrrfrwwv.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gssipdwkc.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/godlltvym.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gfmylaapj.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gxjfagcgr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gdwvewfzm.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gbledngki.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gacrheozq.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gzkwnypze.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/ggvfyezsn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtiqjlamr.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvwjefboj.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gbxbgnkxb.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gztpbbpzw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gatdtgfzo.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gjwxhvvcs.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/goncnoxjc.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gdgbvievp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gzsdvczol.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gsoqrgjis.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/guplqxofe.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvmjcxyam.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gxahexqwq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/golbfuloj.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gylqexwmh.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gxymjijxk.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gpznyoney.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/giyhknjzx.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gwzsusiwl.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gvouztkvs.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gezcmbfzk.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gsueiiaax.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gbqbspkum.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gdegoujth.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/giwmlmfug.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/golkbucim.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gcrtwneef.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/graqhbats.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/glbteovxg.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gbwywfute.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gudjctiqm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/geiucttdm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gbaaimqlt.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/ghwdfcthn.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/ggvygwjyo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gghjelmhz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gxtcanoyf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/glicigmif.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/geqadekqa.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/ghqqwobvm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/ghxbgszxc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gpcptufke.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/guhtjanpf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/glisjjmqc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gsdowjuzm.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gorabiymv.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gmnlpdicc.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gurdesoar.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gctymvftg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gpxrdhnij.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gzevvxpmn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gyyxbcgjc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghuaacprb.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gkmpvxxcp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghsnyvdyf.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gkdpshzft.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gywilgqxy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/ggqwwhoyd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gcmwpzqrh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkiafaisj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/ghsuuukoj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gimylgrbh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/guxoxapyb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gumkbasdw.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gncwddtlj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/goufpgeac.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gxrmdxrbw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/giquyczpu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gmjtfywyq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gzlhkrmet.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gnmtdduzn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gigzcessc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gokwkjqpu.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gzcajvwll.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gsvymabvl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gdpfyuwso.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gbpovkubv.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gomsuhhgi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/goepwbyjx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gzdayfedt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gkygtuvwf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gonjoehxl.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gubxgcgvc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gxququwer.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gjkxdqiyo.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gvdugszka.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gqaizhtnl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gsxprgprl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gkioboecb.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gaqcgcbfv.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gcwqokyac.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gxaslzvtd.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gctnyiowi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gyrrkbywt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gqdwjapvy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gcdyqdwwu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/grbztlqfj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gpwanigam.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gkrnlbssr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gduycclab.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gxhuhfsbq.sHtML


<!-- 参考信息 -->