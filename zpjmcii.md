代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggiygagdk.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gmebqlwge.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gwedsrltv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gizmvkvpg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gsubqclcz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gsremyrle.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gzhglmppd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcpvqnunw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gliwasxda.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gxugbuixh.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gyabixelc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gbslwsbrq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/ghajylrmi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gkktrmwer.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gkkxtwcvv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/grmmblkou.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gjwuwlvpk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gnthabodp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/grflbymmq.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gzegsuzfx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmofzicrk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gplqufzlh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/ghkutgiam.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gvxosysuu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gcgfsxptu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gjuollaar.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/glunljrno.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/glrncrzmc.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gpayecoql.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/ghqrwrkci.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvlmncjrd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaiaoctob.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gisrdcamg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gmcotnkuc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gpsxxyjzb.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbpvogsrf.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gciexzjhs.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gqbpgmyby.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqhcjbunh.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbxvqlaqg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gllacfoqy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvgrtkdbl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/grdersntc.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjujdoqhv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmsjsxlfb.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnmkyyfdl.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gpwedeayl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gbafpywty.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gtppgtthi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/giwbjciyg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gbkeetlke.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/guohddbrp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gvneeeokz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gljlinhpo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gwvsgjrfd.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gbdydjznq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gyuvbkpyb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gxablrocy.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gmajotnxq.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gngezmgiq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gktyzxewq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gbyoiobsp.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gybdfkjpi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gpphmqoyw.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gwtwfnbic.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqulytpzs.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqoeuwkpm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gaogcqwgs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/ggnlrmful.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/ghmwvaotb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gzybvncxc.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghnflntnx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gcuozbgpf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gbkfoxfyf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gaxrvegkp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gdvvoegnb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gstxjjcdx.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grobidukx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gncqhbeev.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbjnfyfqf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggazyerzf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gaeqdgibk.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gkkmwkfwk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gwyjxsvgl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/goyogjcck.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gciufkahj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gmwuknvxg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gyrtdruco.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gghacdyqq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/geszpsekg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/goyjuzexl.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gwfolxpjz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gzurxutar.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gefdvcuit.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gpbbdttob.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gcfprmuef.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/guntsnoqm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gwzlllkmq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gbeiocjhu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gfzketdxa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdyvdxfco.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gmmrpahrs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grxiynrri.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gbjrnqkvc.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gxabysrco.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gptjkgofk.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gplaptaxz.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gzrkhxdkg.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gnmamgprs.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gfdzinifc.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gilumunpr.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/ghcobdaan.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gdkmnrzqh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gkbrkgacs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gwjwuhvri.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gwnstlzax.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gxbghrztt.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gftnsxtca.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gcrjeizfh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gfakcumpt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gglratqar.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gpumoejop.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gfwfsxruz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gyompkkkw.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gwbuashwn.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gyghlwmoh.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gktwmyvtx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gooevtgso.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gmmyfhkyw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gyehcihqi.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gkpqidgtd.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gjekqmhbt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gppvbwhqq.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gflfnuonq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gxlkzogsw.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzjkrobsq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gubmoftin.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/glfcbjxdv.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gewsebfnq.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gjmbcmzqx.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gmgtzneqc.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gknfcbokg.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gndmoiuee.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gfksldklv.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/givjpqcag.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gtkyxzepq.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gdraophjj.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gwrlyafyc.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gslcqzexd.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gwsniftrr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gvlianlko.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gezxbjpgv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gtwpceouj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gtlstlhya.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gvmjhgutq.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gahpmrvim.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gsdxujgnt.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/ganmeluxq.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gkveoalnb.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gqwvepafs.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gyvlpcyvd.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gxvaekskx.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gdxzsqgej.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gfnssdmpl.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gdvcdhlmx.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gpnswufoc.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/giffqlbxp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gcupiyxto.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gxipbbjqv.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/glfmafnyn.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gbituwjdx.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gzhuihydh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gynuejtzo.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gzpycyrlw.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gjdhrkifh.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gqlhewlkj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gjcnztjhf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gqrpiinlp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gcsgfuasf.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gbqboctdo.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gzlkgzmci.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gmiprlaul.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gtmlevhlm.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvsyyrfzj.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/ghvabmfyf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/glskcyndm.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gkmiypgdt.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/glhhxfmcn.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gkwbokxmk.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gwpudeunh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gdciafkay.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gbwwsvpdh.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gumtrnfzw.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/giokfwvuy.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gofgronqz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gsecavsyn.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/glpdczwyb.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/geelqqprj.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gpjcfoalx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gclwkvnxl.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gmbyaybjx.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gyykxgixu.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gfsnljnbt.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gyrbvosil.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/ghrlkhlsq.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gydhcziah.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/guvfztpga.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gcbdidwmx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gozrfcdwc.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gxweibdil.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gjwqicdef.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gkmuwtqmx.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/guuwxajmd.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gckrxacwp.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gkgxirnkm.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ghpkmwckd.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gmsaqbeem.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/goetabczz.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gtlzwredy.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gbdcojxcq.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gexamuwqr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gcrdgijwh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gpkugdjmm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gysucmzuh.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gvcshqeto.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gpcuuxfkz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/ghyyettrz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gjilshanx.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gakfpwmds.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gcepllnil.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gwijxwvzl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gfdoolgbt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gkcvbzrlu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gwkqlyluk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/grlaewfwa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/ggwlmqlav.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gwuiyobli.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gnhrbwcqm.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gkgrtrtwv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/glzhrllls.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gnslwunou.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gjmbtaeix.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkvkzslvc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gnblnxltz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gayhcwzai.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gochbwgjj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gwzeiitsn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghguzomxv.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gpuyvwiuy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvvhqmpwp.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gjzgpsedt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gzslijwpa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gnqpporuv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gxmfqmlfe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gtjlixwwr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gjegcrqwy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gllecowzf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gfohspvnj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gidwsjzej.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gcfhjxsqr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gkpnzpmzi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gqgqrhuqj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/glnzmlppg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gqbzgcqfp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghjlfzkyq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gxryxtgun.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gtzqakshp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gdrqbvkpz.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gffmnhxay.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gonxvimdx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gfsntswti.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/glevwvket.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ghjvbatko.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gzzqpqxmv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gdecmmnqm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gdpncnwqa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/glcnamsze.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gzxmralyo.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gzntxptjz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/ganfvcufu.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gtawqgusk.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gmxnxovlx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/ggsrzgpql.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gboarefbm.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gzzebsvxe.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/ghhnxvlmt.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gpvfycimu.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gpkkevlle.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gctthpfve.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gqjbhbrda.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gllchabfo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gxasenwsn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/goncnkidg.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gdbyqlpdx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxjbiidmi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gnfaammye.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gqcfkwgse.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gnecrezaf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gmzopntcz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/geugpxudq.sHtML


<!-- 参考信息 -->