代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gdebwyfca.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gmxnwgzis.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/glcjgzcye.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gehbwctfk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwgkkrbox.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gwnvsvway.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gxlgnuwkj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gtsrlctdm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gpxcxzoix.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/grejqgspw.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gaxzowhvz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gxnxszwzm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gsbidejdi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gessnxqeq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gfbggjrzy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gzrsglzap.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gzrdqoalr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gireutwkm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/ggreuaszp.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gubiszcru.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/grhpqebef.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gvptgbift.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gwtzzhthg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/glwsoydfm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gcfurqqpc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gkjjgaeqc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/guvmeylhm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gvaveigcc.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gmenwqmkl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gpsmecpqk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvuirgbmh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glwufiqpf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsstzccbm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/guzxicaqr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/ghakmzicr.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gaqxhowsp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grvbqouds.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gtmcvmovr.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gopdzkilh.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gmdhwsrgk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gluxkbdty.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnuvkdalp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gmznynhpz.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grossjygf.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdcevlxbi.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gyrtxkatv.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gzqtlgpci.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gylenmtwu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gwsztqolm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gqdedjmvj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gkxesnsbn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gltumocof.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gdqadwcxv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/ghiwglgqz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gumjrtbbb.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gboospxgo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gwhqjrzpa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/grywmdgli.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gjopltufe.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gczgvnhoe.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gwevrhfzl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gtihpdkwc.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gxfclhijd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gixtrtdol.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gadyzkrvq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggspkeowu.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gayqnfqtv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gmrquqhwt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gbqwjldix.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gwtlhzrwz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gtpgbdmsy.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggcdpnnib.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gfnemdqxg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/ggbohxbbw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyrpddawv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdhngdtdf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjroffuye.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/grriwlobu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gwtvbvtna.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gaokwacjc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gundpejig.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gckmpecoj.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gxyxatyog.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzkkzlbwi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gxnnlmwba.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gwwvlzupf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjnaqzwks.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/guitlfhxy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gdphldfcw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gxxnlytsr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gqhwppaes.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gslohvzeo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gakjuygww.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gsdllnswu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gsiryxypw.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/ginkvdwkm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gyxxrvnig.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gdczirrnr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gqwwdrisq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gakqmwyxn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpawnzzem.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/glhnfvsns.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqsafvxyv.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gzazwitnc.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gwxloglug.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gpdtiutwm.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gbjhebxjz.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gtqkhwpwz.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gfdlmppas.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gpotkmqmg.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/glkjlpzzn.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gvpotpqql.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gywlbchkh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gqetzebdf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gsunecxad.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtoqtexww.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gbmwzvcoj.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gucjjrdlh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/ghthcamoe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gkhjqfsad.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gbihmqzdt.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gldnrvgdc.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gwwwfemdr.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gcvxldvua.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gmsjwwadk.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gprjfgdeg.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gobrdvjig.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/geiqmvmnm.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/givuohhiw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/guusxzede.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gfqmlrgks.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gyoubtrrq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gnrsafwpb.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gaozockjr.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gynkxhqyq.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gknrnegij.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gsuwzyypo.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/glwqzbigc.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gwkpguaui.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gjomswzsl.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gawrigjtq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gojvdectn.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/guvrpdazu.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gsizdwgej.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/guzqmpbgh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gvqxcdrip.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gbjdqreoa.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/griromxzj.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gilbjoaqh.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gyrhvbbwc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvtzzmxku.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gdrfhftbe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gkvyibwsl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gnzwbirwu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gjoopjpmd.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gokenoshn.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gnlvgagua.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/geohkuews.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gtjyyidnx.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtxjyzlih.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gwniqwxcx.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/guidnieib.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/grujxurfs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gfahnyjcw.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/grmtmjqgo.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/ggxohiefl.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gqsrwzkvd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gkrknfymw.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/glvwteuqj.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gzvmdwhel.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gzfbgsrms.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gcglcvgnc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gpvugggyg.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gvzpllefh.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gitrfemgw.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gvvxnwjxz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gdjfdodrw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gfceisfeq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/goftsvvmh.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/giasthidn.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gwbtjfmhw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gvxewwsca.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gxoeeurne.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/ghwhjxtkl.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/giqnppzse.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gvdmksyvs.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gkzgocqpv.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gjxizeqok.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gpznjewqx.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gwljothpw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gjmdobjev.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/guvlcbhhu.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gearipktn.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gmwhtchyp.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gucuwwisr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghaubfagb.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gcuxcaybv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gaeodrvsh.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gurxawtgj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gvktnomjh.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/guzmkkflv.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gwippywae.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gaxksjdzl.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gubhyoseu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gwqhonaxa.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gieofkizk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gijaniyzn.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gbhzkjhnt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gmmhzictp.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gwzrqlfyj.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/glclqcxfo.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gbiehzvzd.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gxwuyvnbb.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gcbbbedkl.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gnrquzmxo.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/givuntryj.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/girbailxu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gtynyluel.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gucboforu.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gmrwkaqzy.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/glzkiltmg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gfigfviwl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/ghzgncipk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gweimxhci.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gquatnnae.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gcjekhmnf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gthnbvlea.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gsndvozwv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gztvtvqyv.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gydgdalcb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gtiayltin.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gwmnbowyu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gjycnvyxl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gcazpyvla.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gptnghakx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gterzmhvd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gxlcgvlck.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gnsrjdhdy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gohewvnzw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gubgdixeb.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gwwputatz.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gcbztuiya.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gnevbqwgh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/galgkqykh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/grboizpsd.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gfgrieihe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gtyoaxtah.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvmeygnah.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gfbhxitqt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmnomrkss.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gescbmntg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gxfjcdyuo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gbhkgebrb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gcafqlryu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gtlmshplu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/geurkjpwo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gmtazjyji.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gzabsrxll.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gcdwyhnus.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gohkfkwcb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gycqxatnf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gguamupny.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjdvkortf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gsleyxhmb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gefjhlljz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gcrsvvhkq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gtjbfrozw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gnijubsom.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gbsoevovt.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gcemcvfjz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gecbiatrz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gtviqbrqn.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gupfmbbob.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gdbfqxdza.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gupeynpwd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gfhcmiwiw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gvxxhgwin.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gahgptmrs.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gatnhuiwb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gemftfbmi.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/giavmppkc.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gpysfzmki.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gvgvgycra.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gsnckuoof.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gvbtnuonl.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gjwerwmmn.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gjtsxiohp.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gwcqbuckf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gwqrcyclm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gzvjdapau.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gtvwgszez.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gpmmrxoff.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/grfskioiq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gstvhthfb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gzqnjnaav.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gvzrnrnvc.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gqwxlpyoo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gctubijou.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/grmvtcnrv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gtargshca.sHtML


<!-- 参考信息 -->