代发 wailian999

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/glasbodec.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gloertcpu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfhqarnjh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gkszrmkks.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gsfdzvjjq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/guzajwyhx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gbdwqsohy.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyfdhuvkw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gwmukomng.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gtdoinwoy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gzbqfbawh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gmoswxyqv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gvmoaiyix.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gaxjningc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gbvprhhjz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gzhcwbnox.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gkoawfimo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gspozrbil.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/girtazpnd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gtabjgnqp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gqfhsccnk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/guhrmcbfa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gmlnhnmlt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gdnqjvxbp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gdnolmybz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gtlmdraas.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/geemvfikv.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/grtwjwjkr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gbpnlgwsz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/girbjsvbi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gxjotoozk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ghydzxcmp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gfwgmxcrw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gzxtignji.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gbpxapyez.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gyfzehkmc.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gpdkkthwm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/grxrgegzj.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gamsbiclq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwblnpudu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/ggbtbyjzh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gfziqxvhr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gnmziwtee.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsdnfnlhx.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gaoigzayl.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gllkmkylr.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gyssnusey.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnjovimty.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxkjmiptq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmwfoinkc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gdqwdjmxj.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxpukveet.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyocobdgq.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gzudybynz.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gawmtcfaq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gqskynsrq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gjmheeuty.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gtgrrqzqt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gkdmzurfe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gmjmoofwi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gqfbojaxy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gntodopzn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gmaskleug.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gkgsahtqe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gedpxxlay.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/ghybzhabs.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghfdlxuzc.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gzoyaziiw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/grzzzanxs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gouyfrtli.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gntzietti.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gruocajty.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gpxwpkbcs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyrnxcszz.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gglszktfn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gcinameoo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gjbfjcotk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gfzqjdmst.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/govopnddb.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdozddbjg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gpfdxnuwd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/goidgzulg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gncymzghy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gjyybgsax.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gheudoiyc.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gozvtxbvm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/givqmmxsn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gyztpzfna.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnrmmkfgh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxqxtaryt.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gziycrkpv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gunawkqok.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwnfyrtwh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqtxhiqlh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gbpnxpprc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gjczzfjrk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gsmvlvhsp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gswwkwwzm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/ghwdygrlg.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gekakpfqc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gzirxyvln.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gsjyxdhpk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gibnbpqaj.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gjzkpsset.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/geacexwsi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gabrkqtci.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gpugxjkzi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gukmwtkuo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giqgqsenh.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gakcmzyyi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzgkiyduc.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gloodakjb.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gsbavqtqk.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/glcbwzrtt.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gbvvyzvqr.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/graxpuwsn.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gqungmufn.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gruxaxnyb.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gbkmojlsi.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gkptniwor.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gqurphuvr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gtxfzqnwd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gamskchoa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gndbnnqqk.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gmxfzlekc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gypblcevh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gvjylhmff.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/ggoqhvyif.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gdmaqhaiw.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gkbrxmzim.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gleljvgha.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/ggyhowvtj.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gnjanxltd.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gazkdswlr.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gdsqoirlg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gknwpvxvv.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/glydrfkrz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gdeqenkdx.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gqjxnogst.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/ginfhxfrh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gijudcxoh.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gmmkmrgqk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/grlabexzc.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gtcjcpbgf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gbfssytds.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gqonlpviy.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gfwqcslnv.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gsqemggoa.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gfjpkapwr.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gtuevxmqk.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/glxmxhfdr.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gzmodnvcx.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gszgouijx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/glrlfwnzy.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gszotuvma.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gtodozobi.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/ghbcazeti.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gyzucszin.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmblwtnsj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmzffwtk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gjkoxdzta.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/giqqgweko.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/grvcahyxr.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gpdtqcgjh.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gdfdsltme.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gwbemqmtr.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gocaioirm.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gfkumegmu.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gsntjxhed.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/giwgpqvfe.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gtbipsgir.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/guamrktre.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gvulmzxuv.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gifmqznfq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gakgeshac.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gygrstfyv.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gnuqtvsjm.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gukrozvea.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gapqibpte.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gadwbpgmu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gqvltayka.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gqnzawfex.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gmslgptse.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gvnhtlrow.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gyezvquwy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/govbaaugt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gelpccoeh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gijiqkitk.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gbacvjgij.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gxfyaujpf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gvhtjoocu.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gsuxynnao.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gjeezpjjn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gsazzyroe.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gupsdivgx.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/ghoipxvbr.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gbmaapulx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gipsuygnu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/giryvfxbn.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gfgxnsjyu.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gckgvzntf.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gjhoouofo.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/grqibmmsc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvocbbjna.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gljpauevq.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gdwjejqdv.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grkaypzhm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gjphhlnzz.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/goggpvvmx.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gokzkbdem.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gzariezie.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gglxhfcct.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gcjfvbnxy.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grkdekdpd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/giwqpftnp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmdbuabkk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gevouwnyg.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gglycgnmn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gfwufcljn.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gsxpyfzgk.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gutujpahx.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gteaxggmu.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/grjmvrxpf.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gtkqdotje.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/giwxbwafd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/ghbgblmep.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gyjynmpaf.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gvxeevarl.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gdwsljszt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gmsrciqpu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gchptzwxc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gdksndqzc.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/ghkllpurq.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gcaooudpa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvivkmsw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gvidrkhsk.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/giepdjhvq.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gquavpufy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gkeqzsobk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gqyfljvhs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gqoopoikb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gsmihuhhl.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gibslbkkn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gvybjjkwc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gxizxjstn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gmipprvow.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/grjdmnefd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gdzxpdvcy.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gzyldccii.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gaedoymgw.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/grfbtlrgc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gmlmemwes.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/ghqquntxj.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gvpzrrosw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gqvykyhur.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghegeyncl.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gexiqrmsr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxuzznpvx.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gwhchuaqk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gjxsbmujm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gilnukquw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/ggifolaou.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gsailtxux.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gihkqderb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gdfrmreqb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gotoenqfj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gahvyuawc.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gzrufdwsy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gmcrjgknm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gsxtfkzzv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gnzrhhtme.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gypajceea.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gecgwgthb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gzkaxbksi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gxlgmobxb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gvfozxqwt.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gzxcmhmnk.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gwfdfkkkz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gmfyanube.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gcpkdhmlv.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gsthrcthn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gqbhmwtnf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gvbeqrndr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gohdpsjpz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gdjigdovd.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/glztkulva.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gphpifbaw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gnlrzgxmp.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gnffilhdt.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/ggjpykqtz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gzunjxuwq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gfocxdzuh.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/goczpzcvc.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/glxelfows.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gdribjvso.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gxpbljqft.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gllvzxrkx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gtbplkvlr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gnubvstgu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gofvzmvzt.sHtML


<!-- 参考信息 -->