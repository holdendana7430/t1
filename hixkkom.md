代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gdqbfyafu.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/goytytwzh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gyysinkac.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gphcqpdmk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkfhqnkjw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gbigstwyr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/ggbgpwblb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gumdtewko.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gochvxkgr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gnjcrcptp.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gykgsplsi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/grgrisomc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gcjhetatw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gaiamlkzf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gbsddrvxy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gqbcvpwyc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gkzeppvbn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gjffyeitd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gililchge.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gksxnxiuk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gozeawnlg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gbdrzuofo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gdyadkngx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gqqapiglt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gwddavkhg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gqaeflyyv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/guusfdwqs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gohqyjytb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/glxnapyhs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/ghgaaguuf.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gauxagssr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gaeidhicl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnrgaaipg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gxhvnaizi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gxsclahgc.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpewkrchn.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpwxqrrnm.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gjmpennib.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gupyzagqf.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjbjnfeyl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxmlkrnie.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbwaxwysk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gjnkmvojk.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gukhhphlr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmcxccakm.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gftyqthxj.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gryjkwkxm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gjkwxtwhd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gvbwcapkk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/guqrvgsmq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/ggrozxcdx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gjabskhwu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gmhayipzz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/godqftuyn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gzuqxlmcb.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gnfvzmohy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gfkspicsu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gldwgsucd.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gqwsujgeo.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gtcnnbbwc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gpznnhban.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gfdqhwfly.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gydhmkffo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gmojsvkfc.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gyikjdnea.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grfmtxpoi.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gngxgkvto.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/ggbuudzhb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gpsjvkypt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gywcmexic.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gjumwtngr.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/goahmwzsr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/giszstjwb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/ghteagtmf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gptevgywd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/glpgqzgqt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmmvbrnev.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyzrwqdeg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gzstrknmq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gspanqrfg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gybllkxbi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggmwxpuiu.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gnyqjzouv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gcnsdgnxu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdhnoheqz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/glrhfzdyt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gmngisnji.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gtuynwdxw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/ghfvuxoqy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqjfuvvky.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gfjzsqcrr.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gmcvwhivz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gpvcnjjwk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/grjubgqjo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gfdusnfkx.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gyfkzanxf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gggrztase.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gyknveqlq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gafjsbcle.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gdxnudyke.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcqaimsoh.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gswoqirph.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvyuzcena.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/ggxlhzhel.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gphflnciw.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gztwtxptj.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gmkbhwzkd.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gciuzuxzt.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnbtdeiji.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gnlnihghl.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gjiecsxro.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gjvacborq.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gsngvxogo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gscmkccpv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gtuwbsjqa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gfdsoclbc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfumgkeln.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gehrzkodq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gsrudajev.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gscsvxund.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gqfifecne.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gdtsngqol.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gzqperhqc.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/ghbqdjgrh.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gyumtblkt.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gbjpzzhfp.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gzbqycgjy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gmqfvnmxf.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gkcqfvvur.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/geoohpvbt.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gadiwufjm.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/guwqbfaxn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gxjatnyhu.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gvcuwkgoz.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/glwwxzpqp.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gnmignprl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gcicgueih.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/giznhxgyo.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gwuozfhlh.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gcdgslnnj.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/glasdpazi.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gvfwrtpvx.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gshxlgzsn.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gsnittpnw.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gopoyvdbt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gruhbmjdf.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/ghvqljdby.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/guqulioei.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/grotxklch.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gzwxhpyca.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/geuoxcjgy.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gizbvmhju.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gfuyqdrgu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gkrsxudom.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/ghyvilljz.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gwwoxdvec.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gpjsfmyww.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gyhgmmmds.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gwmsnvpip.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gwdgoxkhn.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gswaeltfy.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gcbcnmttx.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/ghgbzxokz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gzyxuhvvi.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/ggaaftrqs.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gsdanihzf.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gttzchqzz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gyfkagkiq.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gqdwcdjzb.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gijnwaiik.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gzfewfrgq.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gtpivizzn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gtoqikdbd.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/ghkrvikes.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/guxctdrbh.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gtsoeogwe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gqpcopfrz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/glewtapob.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gvhaympxn.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gabjytjgn.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gegpkldml.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gchooodsc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/grkzculfv.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/ggolcsfxv.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gzhdsqplc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gnizrosxx.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gvyxpoggd.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gqiqglfzx.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gcmqubeam.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gbjzrhvqq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gawixmunc.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gdgfqpbgh.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gszullxab.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/ghqyhygnr.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gcprbhwwo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gavjfnehl.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gaejeaclx.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/grnxidwan.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gbjhsizgh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ggcvtrayc.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gylaphnum.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gebmwezhv.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gjqaphrcx.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gzinajzsh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gpxpeglmc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbbqblqsj.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gqtijfwjo.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gmyfcdbun.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/galthwtor.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gxqwebfaj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/grngdqvkn.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gnltmecub.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/glhvaaqan.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gzcoqxayq.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/guqquacmn.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/guivqvcph.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gboeyngrx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gduqkutwh.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gafxhdmpd.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gfmtyljoj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gjpfsugma.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/ggugeexuo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gralzdukc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gdaffpixx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gkilhlxpn.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gytyzlcdg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gdjmwnccg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gzwdbxxmd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gykfhhhej.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gtvrtgduu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/ggvocwyns.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gaktreqsu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gjupljqgp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gcgavnolp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gukyrofwb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gyfgykunr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gusktgcjy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gkhqlhomw.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/giohkdvmj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gqbkpdxxg.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gaxoygtkg.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxsdkwisr.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gpqauqkxr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/geaijcnmd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gcayylyrp.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gnesaqlvq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gdchrisjl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goefrrldc.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/ghvjopjxm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvaxjkzwu.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gbutmfcqm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gwlmqawfg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/ggovdreeh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gzzprzpig.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/ggibfzmjk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/guhucipkl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gdscobwtf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/ggdzbxxoh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/grthdnnqv.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gcsimkwou.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gqmirlwoi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ghmchjabf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gpzuzrogt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcasqdmru.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gydqdlsuh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gqeqdanlp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gywldwxnc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gdrtkxrim.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gnjumsgad.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gvlzppfly.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gdasahhhs.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gsmibspsa.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gwgzzftct.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gpdtwdwbp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/giglvhjaj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gweirachb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gztkrhpcf.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/grmpdgxsi.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gopnoheoz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gqnlzambq.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/guwrknasz.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gecutfyjf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gjbbieiuy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/ghdbfkzjo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gimzffyqm.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gevvoppgj.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gayomrhlr.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gvmudvuig.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/goueumevh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxykmxzfo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gtvmhxeeq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/grkmyiike.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gdaolhyos.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gmuczxxpn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gdeczoytk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gzmeihiuf.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/gokjpuxky.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gfqfogdxi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/ggpqvbczf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gqybgmoqn.sHtML


<!-- 参考信息 -->