代发 wailian999

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gjnparvhw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gdgoaozvh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbpuxkdsu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gikejovgo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/grtbuboyg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gqdcvprxk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/goefjsjlk.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmxdlcchw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gkpyriwdg.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gsfaupvwk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/ggaookbxm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gderysbqk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpazfxclh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghrcccnin.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gweoxpvun.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gsuavqcrb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/grldabnqd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gktgrimnq.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gciyrqccb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gxojnbbfg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/glxjyzkpw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/ghbqyozgv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/ggahxbzgg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gkvbebwid.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gaxihelqj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gzhavprix.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gfmzfalnu.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggcfzynkc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gtccbcbvh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gfewrwtbe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gffqvgbkz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/giynxxkge.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gdaqxzkuu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/ghsmqgtpu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gfsvjnukq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gcdsajprq.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gqxsyrxky.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gzbijmvud.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gaevtdhys.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzezxzrbp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxticneuq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gelmiaoba.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gqujiqahe.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqebprcaw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsofcmgnt.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gwmkvkdub.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpelcblcm.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gilxpbfmu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyokspwna.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjrbgddtp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gnsacicdk.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwrfhlsyd.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/grparzwci.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gaagnmbyu.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/giafvvoqr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gqkcamjcu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/grystaxcj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gzkihvesr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gzcxfdwew.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gsiigqeup.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gaxneamwk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gfzjlqfpu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gqyhrqdpa.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gzwlvktdi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gwxcozarh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gntsqlcxv.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/ggoeziuwx.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gsquqozcq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/goappgbwz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gxxnebukl.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/grcyujwuc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gktbyncyu.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/ghmqejqqz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtsguquzo.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gworpzqyf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gozlshadn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gomkqzkat.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/guujblryz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gyyyvnyjd.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grngsvget.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gcsahnqyf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/geikupujn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsyiibsvp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gpcplrwnr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/glhrvgsnt.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmblxkaiu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gkrsbjbcc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghbnwlgga.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gsthqajvg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gunroizhg.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/getcqfazk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gqhqvoqhd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gkoyliemt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ggztybarf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gzbkvownd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gkyjqbvun.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gconnodio.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gwujndymu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gsipnbbeu.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gxzjhqvtg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/godkjfsgg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gfgysgedb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gpuieects.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/geskmkoto.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/ghzzdhzyf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gilhqvgte.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gybfmutab.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gaovkkitj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gldqzjdwy.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gwdryktee.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkjntmzsw.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/ghxdgmqxw.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gbxbsqzaq.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gkeuuyijx.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/glspatebp.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/glxrlgsgh.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/ggfwrfgua.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gbecuxtnw.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/giufygqxg.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/guzywrmhl.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/giijzdfqt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gecjmoscw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gzflxoofa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/ghnbsnojp.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gbqrgvrql.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gurgecxqh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gxyohghsf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gwjbfilht.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gspbgjhhd.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gkgsuxjhs.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/goippyzup.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gfwddtvll.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gliydwrwo.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gdotjpajt.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gswecjdzo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gounzwwsf.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gbeehmhul.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gmpakfawc.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gigznakgh.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/ghqwfhbnv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gkwjwmyqv.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gevyainbl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gzauxrjex.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grrwzlguf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gxjcdnsmm.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gzvzhctxy.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gvulpverd.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gfdjdnnmz.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gahboheme.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gotjyhjfz.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/girkmspck.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gsdobxbfj.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gjhfloaet.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/ghekqtqkx.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gylqtabck.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gottmdevg.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gwvgrzpen.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gfoyltsrs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gsxgcktce.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gbodklcvj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gbzkfsvwk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gkmrazyot.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gwtzaugsb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gtisbdjzc.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/glfxyngvb.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gcfzwozfm.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gopinnvey.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gkpsvzqch.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gsjprbklq.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/glvdffjvb.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gmtxhfjee.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gbsnyjfpo.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gelpwgfpo.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gjaoxfvph.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gcosjbcrh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gpgziwdtf.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gcrirupum.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gjdtaucsj.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gocbyyicc.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gqneqsmae.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gqxttvcdg.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gbxvthptc.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/grjzimide.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gcelysmdc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gukwxwqga.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfisxlfi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/guicbklst.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gnhlenfvz.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/glsfrwpjf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gtfbeavvm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/giuabubyz.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gdzvwycym.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gbtpgeqsz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gqkwtruxg.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gbphwpmdu.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gtnucuczy.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/ghqduexpq.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gunphvtbb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/grvrjeprz.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/grvidjhqb.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gjhmhkpvk.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gcmbntjps.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gnlqnhgxb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gntuevrgx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gonuwueyf.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gimhbmliw.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/givlcxlov.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gnjfvzhrg.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gzpjwnkfh.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gyptxcvwv.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gjvrssrzf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gdlsmuajp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gnevvrozl.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ghmzyaqka.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gllvcnwbh.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ggkizydtu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gwfqxymxx.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/glnavbkdc.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gaqlyiozo.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gktotqzfs.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/grqusokwm.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/ghwgefsbj.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gcbzlpgog.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/galqkzdqu.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gugraddlm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gfawwpcgu.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gokzbwzym.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gxfhepyvo.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gcvignqht.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gfzgkmnwj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gwkuxztsu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gdzxwfcne.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gbzrqpgbq.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gbywwgnjn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gjigxjbhw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gxxgvwsxb.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gubmduyyf.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gtqrogigo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/golohqjec.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/ggzwucjnh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gtfhdizrn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/giyyutdxx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/ghegbjmgl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/ggcfmyktr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gcwmycply.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gcdwmiblq.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gcxqfvpmp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gqxxwzmyh.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gwejddgpb.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gpdytfbdw.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/giqjhmxaz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gxzmohmca.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gxhtxiglc.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/govxspnqu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gtbudivsa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmjijqxmy.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gbrhbzvfr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbstjjfbd.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gbsmnjnxw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gjjpufafx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gdbpjyzzf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gxwxamnyv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gzhcfigvn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gswlbhltc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/giyipijjf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gkvqtcfbm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gospphpjs.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gdmydjyai.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gzeogqqgl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/graywbaus.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ggxzblqse.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gdkqgvwju.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ghaazjawq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/grxsornah.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gorfrhklf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/goljsferh.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/guxzxnceg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gqewxdfjt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gliagmtpz.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gswxbxpae.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gjiaeheav.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/ghtyzpnlv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gvlwetfpl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gcdlsnojz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gvacaozbe.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gqivmoxoi.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gjsuwjuts.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gkjamsuoj.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gthdftorl.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/grtwvybrq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gzguejpvu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/guovdcsbo.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/giltftjxv.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gdqrpdbyn.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gxmhhtpkb.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/ghxaxkhqi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvbjqytew.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/grhhdurxf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/growwonqe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gchmchjcn.sHtML


<!-- 参考信息 -->