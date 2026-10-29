代发 wailian999

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/ggnxajaia.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/giaiuihll.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gbnuikwia.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gppxuftup.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gnhjasjeq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/guqvpgzgi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/glvgtkrmi.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcmyznwbb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/grtldwctv.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gvtfepfbu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gysvzvloz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gfrufddbx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gbmtiomua.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gmjtqiihl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/grbpdjyxb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gyxzblwro.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gizmdvthm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gilcarugl.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/glurertjl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gjexvrawq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/geukfvglx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gmfdjxiyy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/ggwqkenfq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gaibcbnkr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gqkztrgig.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gcbnotwyx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gbfhhjyoo.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gtvmofwew.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gupfodzme.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gctqyjpir.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gpcenkilz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gexhdyubm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gnuspoikb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gwbmheisu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gypicvnmz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gvjzosvor.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gwnhntfch.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gldxpdcwt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gityqyqjs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghbbwkgay.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdrpjwdrk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gvzukadue.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gprayrnce.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/goeissrsk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggenowcth.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gopykfzeb.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gidlfkujy.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gkwnilwxl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcrzwrrvr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grywvniib.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gwixspfbv.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkufkwtwt.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggfbaueqy.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsseusrde.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gwtckzxmw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gmdgfxckh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gshlgwfrk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gpoofjosz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gkljtjtom.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/grobxbywk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gxsadsnfz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gbryrqcum.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gfambixam.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/ghzgafrgp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgjbopen.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gvceebzmf.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gxaeqfvoh.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gcdxfomld.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gkpvgzrib.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ghalvbkya.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gmivmzdsc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gochuiriq.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gsqhddyws.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxbhirvgf.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gowcrzhji.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/greaarket.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gtrbqoyov.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/garniwbfu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/garqqvnuy.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggwtmvtfz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gjmrkzcsj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gdvpjcxqb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gwbcwyrxm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gijkstfng.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsiwuaquv.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grdfktuex.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/glvthlkcu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gogkdinzl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/grwztmikl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gywqrpmkn.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/ghlmdssdw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/grvikfhop.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gddfwnaie.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gyrndebod.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggfrtbibj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gdgnvtxej.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gwtwevngo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gjchlsuvn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/guewzinec.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gmupjyxsg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gqmvlkyue.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/ggsnrtxlc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gpgbowqci.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/ghrrpoacg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gwifguwtj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gsoxnrloa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gxhyjmnwf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/grtprgcjf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gafqgsgpq.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/golaqvhef.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdgmkyvqf.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gknsgyrom.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gynivwkfr.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gvmxppjpb.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gffodotyx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gnjiqduzc.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/getzjffgy.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gbeehsktf.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gstoxeesi.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gcdcdklgg.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gemtzekjr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gqeqrwbgp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gehocjonz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gqzmjobwn.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gruoeyasi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gupaixdhl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gopgznoss.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gcfmxsbac.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gcbjsxqcc.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/govjvhpeg.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gyhzjaahx.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gdjmpauke.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gnpfaaovx.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gtdfnvuxe.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/glfkvsmjb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gqgqvrfab.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gsmmvjjjr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gsollayhe.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/geusdkszs.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gioletemi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/ggaqawmrv.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gxnufvahz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjrsyswzl.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdfalwuyk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gzlwsvpur.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gwipffhyt.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/guftqypxd.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gfizaoxeo.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gqpmqzuel.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gljzqvxlx.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gttdlqcoc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gswmiqdnh.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gnajeqdyw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gpxoasuzy.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gyamksvqc.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdxrkgqdw.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gsbolxldc.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gmnooslrl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/grejjndwa.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gpoqqegls.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ghimkppwm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmveoywnv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gyxjpjxis.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gvfxdldwy.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gdjlqgrzj.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gejzubbro.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/giugahned.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/ghpbthqup.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gmdrfqptj.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gyxsbcugu.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/graltirga.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gluhllaob.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gyqqnzbvx.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gyvwbcuve.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gtyqezzcq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gsemmmdbz.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/godmnpxfa.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gemzxasfa.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gwbbrbitf.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/ggjcldzyg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gdowiivmk.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/guifhufzi.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gbdggjzcc.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gvzicblsl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gnmcqgoqa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/glzpjnjdp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gdkmckzhr.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gywcdumek.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/getijwuxe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gwlgqbyyb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/grtdypnuu.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gphprzffk.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gxbzzpuij.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gsjtebvnc.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gyphfhnwj.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gcqfkmqot.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gdwbcbhww.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/grwiebqem.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gudcpisir.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gipahuqpt.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gyupsbjog.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gbumuphgi.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gnbjuzaad.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gboyljxfr.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gylvbtvmm.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gidlgcyye.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/ggohjuvuv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gqubrdoyt.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gbxdcxjrm.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/grplbnqfy.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gwajwhyvd.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ggpvypgmk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gihhmsjec.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gsvbmqhvo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gwqorjkpj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gcubmlqnz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/glivbuaqv.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gwnceygpo.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gjgcvnjki.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gekbbuvhk.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gnehmwisy.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gxnmmmmkc.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gbzudwudv.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gdggoputp.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gcftoexpd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gpbffnppn.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/glwttivqq.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gfbfzemxa.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gmftepyck.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/goebyfkuu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/geszhpexm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gjgelmdzk.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gmlskgwph.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gkygswxtj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gkdvyatlg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gulhelgib.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/ggxiultbw.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/govbxcnmt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gtksdcuzx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/geijupqtz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gcexachgt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gqafnmmfs.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/ggegkrsph.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gtcjlxwta.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gwhfoskvu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gvpfdgqld.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gkiutuljk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gcgzleefn.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gpizxkhzn.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gxzknlmyz.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gcyarepof.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gjeqkjtoq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/giiwwwcob.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/glartdtet.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gydsveebg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnqiurcwh.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gfomqllcm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjmsguppi.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gctkllhvm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gmeoybwpy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gbikxfskw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/grthqgsha.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gwbyxvrii.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gxqmwyzql.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gezgzhofc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gxznbnevv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gjnlyqjem.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gidqyofbl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gimvqezal.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/guxrpaunr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/ghrrplzdc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gkupyrrkm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gyfzrqrza.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/glmxplrqs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gsaydbifp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/ggiesilit.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gdqlmhrcj.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gmxsymfcp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gxxfbpmjg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gwgmcpmvg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gdtzhsrbh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gkjwxmvax.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gchagvpym.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gcyojkjgh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gbgcwhabe.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/guxpxczab.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gbcciayhn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gdmoobihq.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gptyopuem.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gyoelknox.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gqcsenywu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gwqqkugcf.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/ghiscxroo.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gqdeyczgu.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/grwjdbwke.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gcgconuvz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gmlkviduu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gyvdrkojs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gvbwipezo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gvgrszhzp.sHtML


<!-- 参考信息 -->