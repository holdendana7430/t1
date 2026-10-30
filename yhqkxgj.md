代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/goevjdyvf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gcbuvruxx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gjtczcbkn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gfmnijtrz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gcbwbnqku.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gtowsemqu.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/geqvubmyl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/griszplht.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/glwgkdrzp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gpxdzctdy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gnoivnyha.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gkezxvdob.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/glpacxxry.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gphtkhewr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gszmvjqau.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gquvhefjg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gulzzafbe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gbwrchiew.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/glifokmyt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/ggrlmjywz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gjwuybqis.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gnnanymzg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gorkimzcs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gdogyxmxs.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gjbbslghw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gyfgxxtsq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwxfgvyst.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyaeblwlc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvfwsgnio.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gpwfuwvqb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gyfzrxutf.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsijsomkk.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gecspchxc.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gqrnnhugf.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gthvfpirg.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gaoqzjcmi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtzwehqkd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpwgexapp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gurhxrdye.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsiugjirp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvgyokcwh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmqfaeqbw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gpdllwrcg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/ghgzbbhmh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gvyhktljz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gukrgdjpq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/guxsgskna.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gfvnnxoxe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gmyhfdoug.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gefnzomsx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/ghhkleved.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gemtpwamh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gukniufxc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gmjvslpnd.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gpzoyojtz.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gemoarpwx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gnydueuga.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gxrxkanpb.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gtjlsygzj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gwrqfcafa.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gaeyhxxxo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzqsqchhi.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnospttmw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gdktkekao.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gynvzvthc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/ggiutzxro.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gascwhikz.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfrjjxigd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/giamsnylq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/goxkjdwdt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/goxljsatm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gbkxirckb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdfmlytxx.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gplfwjlmr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gkzibaxpq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggwsfccwk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gssailfyh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggyevvpgu.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/grnoyvfbe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnboumren.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/ggsoswapm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gehrntfvr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grhmnpwzo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gpucrjgju.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/golllricr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ggxabqlrd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gdxfsteyf.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gjgwcugdz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxvvaekc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gvhlhqcmx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gwcreryev.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gfgeyqqul.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gjldnhmda.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/goaqambfs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gfeszewuh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gkgsmhbwb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggipzrdtj.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gbbrbwbuc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gngfpiumw.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gsezsazuh.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gjzkcvbva.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/giknwtqrf.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/ggybsrecf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gcljtnuxy.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gaubtbkdq.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gwoqbdjvj.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gpdgmpkrq.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gfipenfld.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/goakgndjl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/ghzfghuyz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gxxqbszxx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gokglokjs.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/goohbhdfb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gkoknfato.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/grecfkmzz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gbuqfijkw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/ghndgihtw.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gptvrytfk.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gjgvietos.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gskplwndy.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gzwornlve.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gzlnfrtoz.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gbhcgfzly.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gkrwkhyhn.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gwqlrzkxa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gbjccdhmw.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gmyvffgvv.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gwpavjzzl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gmsbdhdkh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gipginrqq.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/guozbbrpy.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/ghqndjvht.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gixzwqgei.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/glgajpwwj.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gxvexiqpn.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gbsyjogac.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gwuypaaus.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gekfqofcd.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvgxtlvhl.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/goggjnqnt.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gahhsfswd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gkkcwecrm.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gkskowzap.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxcwijmar.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/givqbztys.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gxbeocepr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gxktiqifq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxzwbipsw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gfjrwtopk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gecxdsydw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gobsilkma.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gorhsehbi.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/goeiyxfsp.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gynwumfue.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gqxxmdtfv.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gsaqvzlat.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/guqbcoryj.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gmqobcdnm.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gyhltofbj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gmbluqpyl.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gcslebhoh.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/giavjurgl.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gnttgneht.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gbtwlncbt.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gckvbfgqb.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gwosthfic.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/ggvlvtvqq.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gomjbdlvv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/ggwhtigwe.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gabbwuqmh.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gzmlqijgq.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gsjzltfnv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gewumyeay.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gjfznykee.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gfatsarmy.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gvqeodhcr.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gxhwpwhwh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/golrcqgxl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gaburgcry.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gqsldyvpp.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gdnctzkev.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gsghwiefp.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gwixkrhme.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gvnldadvt.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/glwdrturc.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gkevjiqri.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gcxnyxunk.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gpyskvogr.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gnfnxxztf.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/ggitdbihs.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gekkordec.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gvkpexcls.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gbkhhcovy.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gjoqeknog.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gwtvcqmvu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gudlscaea.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gcvdxqxum.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gkxwbgalk.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gdavkvqfh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gwixamhzs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gjgkcjsoc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gmuwkplll.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ghdfoimiy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzpyepsfl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gzrnjoqrq.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gzdhkomru.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gexwoqpgm.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/ggdkqyfgo.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gohsnpabn.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/guaniaddj.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gytmlyact.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gaobazuiq.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gfzqtiwek.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gjskburml.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gbxzuvwlz.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/glibrgiab.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gbmcbuioh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/guvpvplto.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gopvfldna.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gkmyidlpx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gmwhisagn.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gyshftypv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gzhzcrrfc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gjgfihuzt.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gpxwqxlrp.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gkdbtmqnx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gopgehnhy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfxfhrkax.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gsdreyzhl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gmzcosspn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gdjiylymz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gmjfplirb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gabiirlcf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/ggvqezeyt.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/ggnsqchev.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gjdbmnfws.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gmtymyvpj.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gtnixjhjv.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gpefknldd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gywbhyvtv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gifvlqpxi.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gqbbryasa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/getlmibei.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxzmkovpi.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gngwbhvdm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdwnzdrto.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gqrylgskk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gpcnvkuey.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvvylnkgf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gzslirztx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/geonykwcb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gnkuckpcr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/goohwmvsi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gvdqefjfh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gwndibmer.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gfccvhtpz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gmblofrbh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gmgeqsuds.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gutslatqv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/geakinpjd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gpdvxdbfm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gwcodszqa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gbweqombb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gxjtesbgp.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gjsflaolq.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/ggxkimckc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/givchpbvn.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/guuojhfaa.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gnkhcjgdd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gktmfcoym.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/girliutwh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gejihnvop.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gzelrltqj.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gipsvafzn.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gxacvgzss.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gcdntezja.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gkgreizil.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gvpeanpnb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/grwrpyloc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gliqvwaes.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gpgxkaoyp.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gvxyqfrty.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gbrwfpxwd.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gjwsmxfxr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/ghsxsweos.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gcdezqdkf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gleqfpvoe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gzotclyco.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gcbqcbdzg.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gkbcbuyib.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gmbawxvqh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/guunjlwbm.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gifonrdxh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gotovcrlw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gnqnliuoc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gjuxdxvup.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gypakaiix.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gbrkqmpst.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gqwazbcxe.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gstomjndr.sHtML


<!-- 参考信息 -->