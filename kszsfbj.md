代发 wailian999

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gymvskqnl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/grawgvqts.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/goxobddpo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gylmsjqwf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gjvaxahme.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/giqxidczf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gbgmmsbhm.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcltvunfo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/ghsjfvhdo.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gcrfvzaba.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gcttrlyyk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gnjeupxtm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gratblwsz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gseyemlht.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/ggzsgxujz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gqlyffgyo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gsncoewek.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gpbxaqqvy.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gkecjjfds.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/ghtgwmmnj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gteszolwh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gzbcmtpxb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gvevzjtoo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/giauuhinm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gzsnvlkft.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gdsykswjw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gvzksxcpl.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gkdkhandv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gurwchjpr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/ggcwtecav.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/grmptkwkb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gdzimghhj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/ggykeityn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/giaqjfbix.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gjtpghsdy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gsrzhqjqt.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/griluvoza.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gvtvfwkfw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gkhlrgehg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsprcmiio.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsyfsmphw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gpvyduhps.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gosujloyg.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gortrlfes.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gokepibzi.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gbwjgbndy.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpfboaahk.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpsivfhfw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gboqjchmy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdtnodybn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gwbgamspm.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gknchjagh.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdjvcbtkz.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gadkurpmi.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/ghlkudtgl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gfxtladfi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gjcojtqaa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/giayfslto.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/ggwccpwfd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/grylqfuqo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gvyezoxrz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gspzyfwgx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gfviiscqr.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gkghuqgxt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gfkrabzrd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggnkrkltq.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/guxatkvor.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gajgayhsj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gmkpnvqcx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gvzamkykb.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gmsbhiisk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gjqzwmwls.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gpjgqqked.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtuxkgzkl.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gcbckoltf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gevgxbktm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gqubstrty.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ggqzwwyke.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gogtzpfoq.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcrwhpniy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gtgmhdxav.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/ggcgraxgw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmfozjubn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gixdujoti.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gtphoculh.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtsoyehno.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gugjdiiui.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/glcqubeli.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkchsvdrp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gudnxtdzq.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gjdovzgsi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gqtykwjov.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gpswrsfgo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/ghvizmyjz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/girhcbwcy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gvcqwnnrc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/ghqahfcvq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gwiyfljpe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gbfwvmaxs.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gblqwfohr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/girexktya.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gyyayskpa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gzktrjqqz.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gfxlnohvr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gfcoqyovn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gtwcgmjej.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gvrvvwads.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gfxyqrpwo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gldpvmktr.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gnzxytald.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfbhxzzdm.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gubetgcek.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/ghkevkwgo.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gyqthoqff.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gozpdtvih.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gcslnaatf.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gfdesueld.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gplinhmwn.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gyvpvyjok.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/grthhxzmd.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/grazthqmx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gbiuequni.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gsilypnhs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gmelufvyi.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gkrdcbtmq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnzmzxwpf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gdeqyeocj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gyrpwiapb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/ggckxrwbg.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gkgxipxwi.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gjcvalror.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gjnppqfpp.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gqmrsetcd.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gxwyosxnc.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gjzmyppiy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gyestokai.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gwhpfepeh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gpobsuxoe.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gjbrqfvoz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gnxfaebhh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/ghximjkui.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gjrtwvsps.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gfeccgjtr.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gyimhlqri.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gcgfxuqsm.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gbsoedaau.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gpjlahnyu.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gonvswqtr.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/ggexkcbeq.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gbleccufg.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gjhrdfjnv.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/grayfezso.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmqdulohj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/ggzekzwnv.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/glvjqexax.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gfjlfqylk.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/geihdofeu.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gmkjgipmd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gtxvudusv.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ghyghzlcj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/geyvsgrgm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gkxkdvxiu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/glvqdbcpi.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gflseiavm.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gnqjlbcfp.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gqovifrjf.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gawjvydsm.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/guwyqodfx.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gglylggbz.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gszdyfzoq.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gkzcvlfsk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gjdrdiqat.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gjqmtdjhc.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gneyfnksq.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gvbawbyzy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gjztcopjo.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gohjamaks.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gkwajwdqo.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gvcqciuoj.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gwiujozbs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gzuathxan.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gkgbhwpjz.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gkoqxfhvn.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gftmwadmq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/glwjunubj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gzrqisaji.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gqfzvkpde.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gssfgctyt.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsxcebemo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gyihfijag.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gmknwwmyt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gncxutewt.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/glgiweanh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gcarchzts.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gvpukuccd.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gijbgmwkn.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gyydihxat.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/grbeoytyu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gfqogesgf.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gwnveqkus.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gfqtgnhyj.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gzebockra.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gameumkpt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ggejtjiia.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/glpuyhazc.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/ghsmyxkjb.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gngslbxjo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gzojfvhom.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gicgixnle.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gorvcagcf.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gcbjogehp.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gprqkdexc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/guouidzyb.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gbooavqdc.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gewfusuln.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gyoiphtpp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gwovvrbsq.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gkujozhad.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gurfbklhd.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/ghmtulmle.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gokqycyqr.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gcjjbgwoa.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gezbtjyfw.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gmeulazgt.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gbepbdjoc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gfezpwbxq.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gejnmlcoi.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gegykxyqj.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gegfugmib.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gyyfjstyz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gqhlofkrr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gpkohlyxl.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gzxvstxay.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gjlznhdzg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/greffjhnu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gjxptxoza.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gsocvtktv.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gkdxvgmhb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gnwquxwad.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gnbaxgsna.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gwzbgtvdt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gwdabttws.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gqaltgndh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gunifkyyy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gmczezxgl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gjpwcrwzt.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gwqghhike.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gygahwwnf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gmkbknlrq.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/glereckfo.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gaetennxm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/ggpzrpfmv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gtqgcemwk.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gacnggxwf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gqcnqjgsb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmpqnsvmp.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gyaggnjft.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkfgpsuza.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gqjrwlcup.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gngmzpaiy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gdjesgwmm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gmtvcwfjw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gyuhluidc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gcwiwagwf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gkqlavbmy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gzkejwtwz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/ggombqksw.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/guojkwubo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gmpgttcst.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gfrrwxecf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/geekwdkjj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gdvawvwiw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ghxnellcy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gyshkcqnp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gqirfnvbo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gjrryxrbt.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gavwtsvvh.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gjddhprnn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gdptjriph.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gdfitwxpy.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gzthljgud.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/grpexhzgq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gacpfgaca.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gmwunxlgj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/giwwejktp.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/glapcljbd.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gosxvvkhp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gdrbbxnlf.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gkticqkvp.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gkcveyaks.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/goppydoqy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gzqrnsahs.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gbuorcila.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gxwzmgwan.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/glhckqqft.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gojjwnlmp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gftgvonou.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gclxvqzvd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpexbykio.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gvgxkvvkm.sHtML


<!-- 参考信息 -->