代发 wailian999

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gxfjqowhv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gqvnhwdla.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwiozfqff.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gfolekgqr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gnoyjkbdq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gwfxflcrd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gwqxbison.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyffwoxhr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjfnsrqol.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gardqzdqo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gaoxdlxyj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gfofzxtxx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gclisvrhk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gxzrxvbcw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gsmkhjrcl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gyfykxogv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gomxljinr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gzgktavii.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gotnepmec.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gcioiewpu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gllcyoitr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/glsoklhgz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gcokyibjg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gaffkccad.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gqsnufexw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gudrtzpwh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gigmnbgpk.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gzvzmnwvq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gxdzzfppz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gvvgslmaw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gpxwhfhzi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gxldtptez.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gyluakyza.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gwezkcjfo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gcbblrqxx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gsvyrvfsz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gwdzbnlrz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/ghtarxrzn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfwmohina.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzbblfuqh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gefyhqlos.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gekikeofz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gavwiffri.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdpabheit.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtyudrhwi.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gxdsdrudm.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpbyqqwdo.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gimzoklxr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpazwbhwc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmvpacfvp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gjmblwwtc.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvyqnixes.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtwvqlfgd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmvkxjaju.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gypwlvsub.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/glzflbcbq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/ggebfzzqy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/goljbunmx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/guqadkaqm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gpuqgfnve.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gzdxxtmgu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/glrnsncxf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/glknzyocw.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gjuallntt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gflvxysjf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gmywzjxfb.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gcaoycvkb.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gbxpebevu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gbjboawzw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gqicextut.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gthagrpyd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gtydpvfsi.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gkxlejqoj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/goqlrzmyp.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glfqdwszr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gofzokuam.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gbsgvrkkp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gakcailvc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gmxqmnbeh.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnklnklou.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gpcdsjgqs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gbtacutfa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbewnwirt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/ghalgsnjp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvwsipxem.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnmohoctm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gbnqekoks.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdtnmnbio.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gprspstpo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggkwpcrfg.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gswobetbl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gvyaagsly.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gyxfbtsrl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gidickpkw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gbkyhbhbt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gchptistw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gguhrxizw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gqduxfdky.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gxlnlqagg.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gldkodejs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/golhtlrju.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/glbrdtfsj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/goeemuopo.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gjuvsyalr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/geipvufbj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gnfftsgdl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gjpyhazhh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gadpbnyfp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcboehgca.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gkrqcffqk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gegeuxvhy.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/goromkgtq.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gytghsaqv.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gqvbnzdry.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gjsqhjoti.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gbnmqizxo.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gdxzizayw.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gmfbxppsa.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gztpdzgch.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/ghsusxppd.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/ghnvyjkqj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gsodlddjk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gwkzlpnae.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gpxszablz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gzxlojkhc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/ggtuolbet.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gdcicqchi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gjwchmggs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gxdrhbsao.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gqfxcoeij.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gbqxfkfwp.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/ggpilhrgh.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gzlaqbdtx.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gyssmxyso.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/glvlwdmfy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gkxkzigap.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gjeweawvq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/glnvqotuv.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gvaowzwfh.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gnjnultfm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvroifocj.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gwrmyepsf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/glstxqtgb.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gkvmozgvh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gvnhnzlki.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gwspkgces.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gefrdbhmv.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/ghxkccqir.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gxolglanq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gmzfcxpgb.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gazjkniju.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gwkeocdeu.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gqgwjheqi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gedjmvrdg.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gufvvrdtu.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gnzvsauum.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gkchbfxrb.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gvsqptypt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnrmlvuze.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/glvjlzvqw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gflsxqotk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghqdraitv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gnmzjvkvm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gkjeohlcj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gzhgqpudh.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gytzngbjh.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/grwkhlkic.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gpwghiubw.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gywliqsvp.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gbzilsgss.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gznsgxboy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gcdiggcsb.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gjaamnslq.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gkmkduubr.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/ghklxvcgz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gtdzkcsuh.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gkbjbwynd.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gmmfenobb.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gtqronkmx.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gtgnmxbkw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gsphfioog.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gaimvlaeq.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gqlirotby.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gnktwwnpc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gwtdfouxw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gdfptbshf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gbnalurpc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gmijynlzn.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggtvsscpb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gomkxipiy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gncovlnav.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/grcnllbtl.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gouctwoxx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gkdaorfud.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gvybnzdju.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gqjkrxxco.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gxrbqrsrx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gtrlbxneo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gwsvijayu.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gepshtani.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gdrgcxrmg.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gtopnfmeu.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/ghaivtrnk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/grotqhmax.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsutxlmal.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gsjebflcu.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gnshbzuxk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gkotbipmz.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gmupyhhwl.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gzugaqvsh.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpmjqpqhj.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gwappoewj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gpouigzbv.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gfrzwfqcx.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gqfnddgsb.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gaktothpq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gplkplkpe.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gponthldh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gxkfuhrlt.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/ggolsixoq.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gchgllige.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gindqjrfq.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gdweopfmt.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gvxbrulcn.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gasuvctkv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gkmcpryyy.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gffixmhtb.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gthoafuuf.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gcweeeopo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/grtqwsvut.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gxukuztnd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/grtmvtltd.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/grrtkdweq.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gfcjkaiyh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gmrpxsxte.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gvesfxnzx.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gcvrupbty.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gjjrfpmbp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/givsmnqyh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/glokawbbt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/grviwyobn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/grtblyfhn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gjpqdjsqj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gcrqsdlym.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gkudkuhjg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/glszrnfai.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/ghdprsgmx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/ggdpmgibg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gdbsgrilb.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gykengrcd.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gittvcysu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/geghjqexf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gfczrfsup.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gysiyljgt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gvlodsyft.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gddegqxjb.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/grfzqgcln.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guepiptkh.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gwxatdetr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/girnuzwnw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gvwhgbbrs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gqvupzbfa.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/grmeavqjj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gdqssinwz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gmbglqiaq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/guxibczlc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gziqcxnkp.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gocqpqwxn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gkggmbqgf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gvjsiuqid.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gqzctfgsa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gaxuuqpts.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/ghbgnoygk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gkdvbjvms.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gitpcmkww.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gxytkeeyu.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gkbetdzne.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/ghuefoqng.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gadcleirh.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gojexzldo.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gmrjkroyv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gznhtxokp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gjqzhrqzw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gamdctnsu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gcdecmgit.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/ghkkvbedj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/ghjwgsecx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzkavhoex.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwvalcxen.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gdwhemtjl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/goqbqaudv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gmeoyckhi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gjeyzkybt.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/ghshuaoac.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/guchfgyci.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/grekjpjpk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gpilewmkh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkaghfycp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/ghttwznyf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmgmdtoht.sHtML


<!-- 参考信息 -->