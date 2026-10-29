代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gugifzrgl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtgdnoxdx.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/guhrkjmna.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gehpddxzy.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gyffqqqjr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/grypokegg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdioyozom.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gkxocksxo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gcgghuhsc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gmlypwavs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gvzqeblqs.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggnwjkxxm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/geuontmpq.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/guqweuywd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gnrqcpdrz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gvaolbmuv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/grqalxpuc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gqdyseihy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/givcmmkqo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gxvkwglsa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gwvxrktdp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gjgjregdf.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gsmtpipin.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gtylqgift.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gqpupoyhh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gzcbpizny.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/goljkzmhj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/ghyeatlfj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/grrzjgftf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gssiazgau.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gvoivkvbk.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/geprhmiwq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gtscspmys.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gybdxhljc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gqjymvmfa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gymfusaxz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gygbqeueu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gpkbuzwme.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/glxxsmcrt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/giyksevcx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gpotkcmci.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gakkcwwvv.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/glcnwzzxf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfjnjsgyc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwjxltewy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gafqtwjyk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gxhtaetzh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfcgupdrv.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfetgmsff.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gwvhzezfz.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggxurehhs.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gikcyzeie.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzdaxiore.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcfxpsdkw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gnbslmqsi.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gehobqyqu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghaysdfgk.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gqsnvjqxu.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/ghchfiduf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghwgdtlds.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gxsxeflsu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gxlttqlde.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gjgpaomox.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gpgylscwm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/grmhzewqm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gwizshseq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gspfelovp.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gvyqpzrdw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gmjelyuyq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gwblfbxaj.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gourggkse.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gmzvwipek.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gcuzmstze.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gmjqfhmml.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gpxkxoqfh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gsprrsbxo.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/ggtspbxbi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkfoqprig.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ginjaxlvb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gglppvqht.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gdopqkfpn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/glrpiqjgd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gyenlehaa.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfequgsui.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gmhprmnfw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gveuiplgl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/glkvtpeop.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghssznsip.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/girorjgey.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkfhqqmez.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/ggqpqhdkg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gizqqaoui.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gkvddgvjw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gxemclevm.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/goxmqzfvs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gzdvssiax.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ggjkcuayq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtipdcijz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gnuzkcfgj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gadbhskjj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gphidveqp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gkrfdilpk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gvkfxzrnp.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/ginhbrcvz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gsymswrgb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gjbckejkm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gjfhxzlsy.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gorxmuvqn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gohlisgmu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/grlynmlbu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/glajftzgy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/ghrczmddq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkqdprvxf.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gdbsmdiqw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giuhlhbzc.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gsmgytcvd.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gepnkjghg.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gabqwpmaw.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/glozpjmvf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/glnkixowm.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gbqjlkvtv.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gzkxbiesw.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gurkklqkd.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gsytdgbcs.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gpmowgekq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gwjositge.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/getnqmaun.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gbtmvjyxt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gteqjgdrt.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gfxtlcotz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gwdzwymbt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gnmjplmax.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/goyimoono.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gawqwbgcr.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/ghjqibfzx.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gkmkmzuhh.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gtzjixugb.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gfkcbojbq.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gdatkwohz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gdytjxqff.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gxigcmzjv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gvbznyzme.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gujwdusvt.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gkxummljx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gqfqsyqlq.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvlxynpbe.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gtnhiqrap.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/goqljlznq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gowjfbpyz.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gkkxbqpbt.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gdsxyluuw.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/geetpeaas.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gqrlyxede.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gnuhowocq.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gafptxbhx.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gkrhivlbu.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gjaypplev.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/guvikbeds.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/garweichk.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/guhfjqexw.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gzjehchta.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gquzwxamg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gaalrzfsu.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gakorbzgm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gjsdgkpcf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gpszrjzas.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gtpenntqz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gptqkylzf.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gjioghhbm.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gdkpskvad.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gcazijznm.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gmvvzzcdc.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/godzuqljc.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gxnfbalsi.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/glwqknbds.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gerckbopd.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gaxoexqei.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gegckbfje.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gvcudcizq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gfhjsmdkb.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gjaevrgpl.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/grafgwoso.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gfvcjwrbg.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gqknurkve.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gnmxfnrnw.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/guerkvkft.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/ggviqnkia.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/glonvqqvv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/givtfysqe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/giakeyplh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gdhknurpz.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gqujtoejo.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/greidmhlk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/guntnqtso.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/guqvgheez.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/glkhsdwhy.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gjoabxnjl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gqgytmkgd.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gbtrywlwc.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gnjujpgla.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/grbylfcnc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gcziyhiaw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gyxatlzwa.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gvucsgmhj.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gkadbvlmh.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gcxqccjrk.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/ghwayguju.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcjanvzig.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gcmiicrxg.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnfnuusnk.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gaxluvrch.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gdkzhzpin.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gdfesayxw.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gksvtmuxv.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzyzxjeak.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gvjwdocnr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gblwqgspr.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gsnunwvhp.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gghuktvtf.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gkakbsmae.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gtedhfmjw.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gppqjwdpt.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gxjhzscim.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gbmaqsgjo.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gobgvzcdk.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmazhcomc.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/grgfdibzh.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gxvomdwpa.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/grcqeobxm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gzamudkfb.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gvxlvqyps.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/getckgosu.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gbsygpwhj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gododwadd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gybggobex.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gtqopoiat.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gvwwfxdgp.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjcolirxx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gyfhatvhl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gfebzehnl.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gxsoxonrv.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gkgmtjoeh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gbmmbuzzd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gusnoqzvt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gqkfzztek.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gvcfwpddb.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gozihcmpa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gaooiokju.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/galdtxxfx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gxpqmilfn.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gyvoiutgz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gtbjwnwvb.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gcgfbqvly.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gdehwnnmr.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gksckxdkd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/glpdhhgop.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gvqcpgxid.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gmtsoncne.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gnoduflah.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/goqtjrxwz.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/glkhobpzo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkbqjtoyn.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gwpqkpsya.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gjfhvkxlp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/ghofdhsmx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gyohxbxay.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gglwpikbc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gquftrkzp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/goqjjhrtc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gnorvbmtv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gblxkyrvg.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gvgqtzemk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gjtqwajui.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gdshtcahq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gtmylswvo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxkshhikv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/glzmbdyaq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gvjjjsyzg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gkboyqahk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gbvbicbcv.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gojfjpkbp.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gbvadjork.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gpnxrmzxr.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gwgwdcxby.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gxeickyzh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gjaltlzlv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gxuothqot.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gfslmlqcc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gdiyaethd.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gzcbjbpwt.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/garqvbwrx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gqyiplhjt.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gocpbbhmr.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gzhwputge.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gxzyownlx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/grdjxojnb.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gyvgewcer.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gmzybuttg.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gpkbykvbp.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/goyykobzv.sHtML


<!-- 参考信息 -->