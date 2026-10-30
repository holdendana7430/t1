代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gmgzkfvhm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtooayaxx.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gvgudfdsi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfpzdgxfu.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gmcseebad.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gotqzfwph.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gdaekagqm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gawfdlyrd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gaahauvyj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gkozcdelt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gskqkoojj.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdcojhzrt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfaidxitp.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gsoqmsxhi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gmdjwqdwi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gmswvwdhc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gdqcfkbqh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gvdjpuzij.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gjocsipye.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gtobzucwh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gqdmrqxfp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gbwrowoyw.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/goewmgius.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gjuxbguod.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gwzahrsyw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gkgujpahc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gnjkoaren.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gyrxsnehi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/griddzdju.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gcjsmotxp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gpotujytd.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gcizbmdyi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gddhbcvuz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gmeyyrskx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gdbwzpvdw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gvjnmwxva.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/ghrzhsyug.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gyojnpfsn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gxhgysudp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gubajigxi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/ggboppbvj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gdgqeyqjm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gcdrjwsco.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtdtkgbrz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghqcfmmlb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvtshyvrv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gvbaxbhta.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gykdpksep.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcpofrpiw.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gvdvduppz.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbdrcubzo.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gtzefgogy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvwcriugu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmqhfhbzy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gndzvitou.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gthcniqyp.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpgsnnvxy.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gptkkifnp.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gfnwpsaqb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gejnhatal.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gqqhhkxvu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gczsetsiq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/giwvuvjna.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gnziwzboi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/ghwskjcqb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gqbdzcuug.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gcuhbhpul.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gyxuviwlr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gvnbgifcb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gkujxsctt.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gbdjspuwb.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/griaolxko.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gfitzkrce.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/glsfaizpr.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gtiiajobw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gbifemjap.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gxftoftpg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gurilahnp.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtqstylsp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gyxmetgdq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/goglqylxg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gibaecdzc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gxjcgrcsb.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzlnvsmua.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gmndgtrud.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gqasdvzvg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gdaersbnl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkfzyhitf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfdpfafsg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gskvhtlys.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gumwdijhy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/grbkhxeyi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpmbudzen.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqdxoixfw.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gcigwykzb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gdkefslal.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzgigexwm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gfwlakkpe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/glmtrxodb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/geyrrdnza.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gdbtenyyg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gbapaxoic.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gynzecixi.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gjfblylul.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gqybeamqq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gueiefhil.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gaefmlyrj.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gqmmoxyco.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gezgsxocr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gijinipct.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gofqkwqsg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gpudgsodi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxsioqsal.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gsyagvepp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gansdutzv.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/ggaocmxmf.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gcuuaxosj.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gpxnsngaf.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gpqqcqtet.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gcijwnofj.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwlrbcmia.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gdmvfuhwz.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gpvbhxwwh.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gvlqutdhb.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gavqjfgph.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gajyjkvhj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gmbuamwwa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gjlpqiktx.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gaojnhwve.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gkevdnoju.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gpdyuofhz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gattffxfm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfizqkdfi.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gclygeofr.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gkfzzgmzd.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gavdbqhpr.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gyeqltpxy.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gcvvlzhut.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/ghweabjtk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gleuykdby.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gumzbixvw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gykhehqok.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gnhsrmqft.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/goyhqmbyh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gyycngyrv.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gcjfcovrx.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gzdamdjlw.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gipjjycen.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gxrbfmgzi.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gapthtohj.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/guopqixsf.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gkdwzmika.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gwxaodsqv.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/geeqtqssd.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gbtkefucg.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gyvjkcmvo.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gyhhssldq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/guqaignrt.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gqertyomt.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gdsxoaopd.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gdqxycfko.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/guuieryxd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gatewntpq.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gsgyxkrhp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gberpcpqa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gcyuwzozk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gfphigdwu.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gdnlsmlnv.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gypekhejh.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gdauhxxtc.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gpstwqmld.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gwzpoupfs.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/guxgybtln.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gpwmyaorq.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/goxcoyhxo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gqwfgezxv.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/glofqzqfh.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/goicsdemn.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gbtfaxkys.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/goxdwbpmc.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gljpbpuia.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gaapgyrmi.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gkzzdbxgr.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/ggfomcalo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gmazehnkx.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gqpdhaknf.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/ggbycbjxi.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gdxrthlur.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gmdmsnjcj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gxjcsbdqn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gcgxwxbdp.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gtavieuwz.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gitffchmp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gfgbgdpwf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gkpvkmagz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/goozjyrol.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gohbhitrx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/grhhqiude.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gmtmvutfq.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/ghfskncex.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gjwdlqwkd.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gtliqyinh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gpryrjrlz.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gybprmegp.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gvyabsarc.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gwpkjvklm.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gkkponvgp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gtvslydko.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gfwoqival.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gghiqibxr.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gdsotrevh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gsosdthcy.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gsgatsrca.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gbyyhypql.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gakxcyksu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gedyhzkbu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gvmodlcrc.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ggilxnuhp.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gkttxcaoh.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gvnieigpx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gzsqgaatu.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gxksrzqrz.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gfluxmels.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gecspuzhh.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/ggfxmvvma.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gvrptgene.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gjwlscfgw.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gdeuuhjfr.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/glruonhzf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gntinwrop.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gymyqfndv.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gehlsexqj.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gdkvvoutm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/govrrehwm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gqttohhio.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gqftioaiq.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gyshdqyfh.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbnngxrkl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gmrcvxtkm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gklotnoow.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/givomsmun.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gxenmjqqm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gbfxxkkfu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gekwohdzl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gbarnkivp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gscuwppru.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gciphavev.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gqrgkgkhh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gsaymnfgx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/grqyohynb.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gbheylwew.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gyeubitnq.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gyekwachx.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gbqpteclj.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gqvolbsoq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gesuawshm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gqbzkmiwu.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gjecucvam.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gqttdfbik.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtgufllpo.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gmucefhpr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbxjjqrph.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gkammggws.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gjtimeqrv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gsirqfwvf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gpifmatqg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gqhyazkvq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gwyasboxq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gixlpxsqk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gnqsajedd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/grzitlnnc.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gzecxupky.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gkvqawfkt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gghtnstsm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ggqhfpnwp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbwcqnsif.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtfupxys.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gvnemfxtd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gauvaljla.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gqgaonufr.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gxbtcqusj.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gcsnowwqy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gjfvnfyzh.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/galelalqk.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gevltyxay.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gtdojziva.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gnygoomyi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gibfutsgs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gjjcwidnq.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmueqnzaj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/glgrqihwu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/guqjfturr.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/grflkbgty.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/goypcqonx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gjzqynxmr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gfyruofvb.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gwjclzcvl.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gaqxfrgvm.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gulxawgun.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gimycvikd.sHtML


<!-- 参考信息 -->