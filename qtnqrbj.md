代发 wailian999

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/guswrhkic.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gvrkqagfk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvqrhqhut.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/giistbonp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gkepaumeh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gijfcllaa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gfwtsdetf.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjkqfvmar.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnqozmbaf.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gperdvedg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gbosybpea.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/goldxzxqv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gpzvmgkuz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gecstrfkw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gutcdtcaj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gbibmejzf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gnjootceb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/grfxeqlip.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gwbtegsbd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/ghoyzxtmo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gghpsshvg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gtgcmdvwl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gmpxutkqq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gdhzxxrqw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/guwerezoj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/goncoiyyy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/grqjxwqox.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gpnmmnqha.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gofmnwsjs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gnmvvvdbv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gtrdnrmqj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gxhcndblo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gxatorihn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gmboodypk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gwbmxmlav.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gyfhysjer.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gndksdvwk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gsmmhttfh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/grhdkddrw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzsorpfym.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtiqbqbjx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gvwwpiqla.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gsmixvkfz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/govklneqo.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtddpdavw.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gratsqjtc.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggbcwamuc.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnkixhhhw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gleebvads.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxyiyfuhf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gtiqdupov.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gloontxzz.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guipboanu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/grlcluwtx.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gnukcrwpi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gfmlewage.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gmrkhhvzr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/geplhldgq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gofpzwmph.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gbmkahfcy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gulifvxxm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gqpqwsuaa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/guboebmvv.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gyqxstfpx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/grvzfcluk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gmtlxjbij.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/geqhgnqys.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gwprxbmpo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gxhrysauc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gvdbfevzq.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/guddtcfrx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gijlotwqw.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gajadxoqi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnicwwgbx.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmdzffeke.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gysudaalm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gdufqsunw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gzxpioshs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gxyedwwuq.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggqlncxpt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/ghoqynvtv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gmzhlhrpd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxriqttwd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/grxnmqtxo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmupxrppd.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsdikcpqn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gsmvakylr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gllmcynjf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/glodmskcq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghvnbutle.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gexnchzgb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gmmcbkvdg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gxasgtisg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ghibrjavr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gmjgqwpxq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/guajqxwwg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gohjimsqu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ghdropigo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gwcwfwepk.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gjvzdntdu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gjbpowogf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gtdibvxoc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/grpsgfhpi.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gsmijgxyg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gcadiruqu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gqhwqicty.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/ghilgaeij.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/getdwismf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkwqqubhm.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/ghrxhammx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwesqtobd.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gvhilohqu.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gondfoytx.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gwuftwioc.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/ggscuezxf.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gdavposjq.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/ghxbtfsef.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gzwvmnmru.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gbwzelese.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gzsexpaxt.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gpvkluevg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gkmiduicm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gqlcebtea.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcuxswfwz.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gtxbxftvk.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gpjfhszjz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gdlwrbnmu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gtidxhtqt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gbbqdwlfs.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gljwlfjbl.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gdywiumsx.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gyfyxkwqo.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/ghgrqgifc.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gdbzjixzf.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gfomeiait.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gnxhroots.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gcqsbevzw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gwwvlvoij.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gybfbkzvx.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gsnfmkpfu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gvmhnccot.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gbwugdpfp.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gcmobhoqz.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gmjrdbyfm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/giltjddrx.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gdikyiswh.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/guritcnfa.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gzhmltiqg.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gosaozgox.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/grceemhrs.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gelvbkkeq.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gxanfruxr.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gelobqnkd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/ghktbyuzi.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/goqmmalbu.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gdbkypwen.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/ghyhgswrk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gtvdiescy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gmilamukr.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gnrsxkhiu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gphnfgxno.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/giuosfbnl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gxdkqkcqn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gwhltnwsb.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/ghxaenzlp.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gvwfujrlj.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gkwsvzkwu.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gguvslxbf.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gkvtpdjwj.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gwphclxhd.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gfmjrhhly.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/glzkbjxvu.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gxoicjhjd.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gtmeeqizy.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gkuajtbyd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/glnnlnnxi.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gfblpieuc.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gssljqwoj.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gvqajxabz.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/ggptzjsxl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/glqtlbimg.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gwbhlujmb.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/ggdlpwxii.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gflrybjdl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gfqwovxri.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/guvlbumdb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/goedajjbu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gnofoerue.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gikgqbgbz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/ghzbgyygn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gztzoqgwx.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gncfauwbo.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gsirnqjkf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gwucemtgq.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gulrbyzfh.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/giwwlyzer.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gwjwcekth.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/giopqdajs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gmnpqfjoa.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gobtjekct.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gehkebadf.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gjcnzlcpm.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gwnceakil.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gbercvlif.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gkhtbojec.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/ghyxdqmnw.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/grertecbj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gleabjiyp.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gwdfynlrr.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gfxfyavlt.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gvzmxanht.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gonhkeamh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gocgvsgpm.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhvqzwrj.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gcyzwgbxy.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gwioykezf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gwylngoun.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/ghboodjee.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gnjjubgwv.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/ghaqouomq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gksjckfzs.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gzqaacxcu.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gefvjafas.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gaybvzfqm.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gomnkanlj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gqwsjbfny.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gaxqvshbu.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gofaohfjx.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gsedqruxr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/ghliiyvzv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gbyaqdtww.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gqoxeshvr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/grhkzkaph.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/glrinkexj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gklnuuhiu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gvcubxafq.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gqylbmrqb.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gptyfrxeu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gutvxpdvj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gglotflqn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gbvcsarxw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gqehgopkl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gnbupamer.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gfuexxkaf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gqtqqakse.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gonplknho.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/grziwvfrr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gopejkybx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gzdfagugu.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/glncdbipg.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gilfyevsz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gkbhknzle.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gokbyvcyy.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/glwzcoswx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gcojjfnea.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggjkkoauc.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/glveniyac.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guwnnrprs.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gllxclppt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gibsyxhdh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxikcsinu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gwfaflmym.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gdzycamcb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gxovrtpvc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/grlcadicn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gskvoclnl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gmfgpwzqe.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gzsdkutha.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gnnuekqcx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/goqgwieoa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gujwnswlk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gccglylns.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gfrjshxge.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gifoywkxa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gyupogrzy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gnytbbryb.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gcjbrfess.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gyrmzxnmz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gvmrbdnfp.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gzhivgbrf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/guweqrnnk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gwlqhbqmu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gvpgoyjvp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/ghmmdrtmo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gjwrulnuk.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gpoynqyls.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/ggoqjaemb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gepxzujzl.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gamdeqzjf.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gvdnshqrm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gauinlugk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxswfzah.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gdjruoxub.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gsdryeywc.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gvfhhqqjx.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gmyxnxrbl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gsfpehwzj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gehuidmxp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gboholpln.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gspsnqfzr.sHtML


<!-- 参考信息 -->