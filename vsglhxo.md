代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gzdjpmjez.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gyftnvxdo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gzirqxbcj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gojujovfm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gfqmmgxvk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gschhvmkl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gfcaxznrg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gwugsdusg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gcahvdmfc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbclpztau.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gprmuemhc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gratnfqfm.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/grymgteoa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gbikepgsy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/goyijhjpc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gvogxieva.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gmyccnduu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gvowtdsoj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gacmwmexw.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkderwemj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gmaddndsy.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gtvqlvcky.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gmtpgtieu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gvhmxmydj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gmkebhvit.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gokdcjzdu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gfdvbcogc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/grudznhcc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/ghcboqejo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwsmtdob.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gyvvibvce.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gkvxovnfg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gbstlcsym.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gqnbtetzs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gqxhzssrv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gjqvuoqqc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gulyiewyr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/ghsunngag.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gmdmibvbk.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gsjsqodzz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gsuqsfnmh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/ggfqmobcq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gvghcwxas.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gnekmksbk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gxlznecij.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gedydibas.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gdwgvmobo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gdsacynzi.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gbbyodnoa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gasvepine.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gkeehtuws.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbtiuccvc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwdiyzhhf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gyihuppvr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gygjgmqjt.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/guyuznlpz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvvwmqxpq.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gtjuoupme.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvtgytxqp.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwinvfodr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gubcswtud.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpizuftky.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gkpfmmofc.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqqazodwh.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gksvewfur.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwkwivyzj.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gctrfkdks.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gbhvhryka.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gfpswxbwp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gbdhhxchp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gvvqapucv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gyhkkyvwk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gbpezfaeo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gslzhwqql.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/govalvowp.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gkbvdhpda.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gvuccgpiu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/ghxwiwmas.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gymelbluf.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/ggurfbsxn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gifvjmixq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gertepyud.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gelkqkvhc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gdjoeehjt.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gccsfltkq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkrrhfnce.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gtcgdgyay.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gduxgzmgm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gljzblbed.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gofvyamhd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gjzvoivee.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghcqhfzbr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gdrneivqy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gjujmyyhy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkbloxwto.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmgdwfzse.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ggsgjrfmj.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grdsfrvfh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gifwkrojc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gahvrdppj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyjorbqhg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsbdbrhdw.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gyytxffbl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/grojffjga.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnsjxhuxx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gpovcffup.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gneecpxtc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gnethjcch.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/griwzmlsj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpwyrehyk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gpwdvssfz.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gmjvvvyyo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gdiuyckdp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gnncjrwlj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/glfovnhut.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gssfwunqz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/goithiger.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gmkapmric.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gcvszijfo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gnfdwynff.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gubemilut.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gqmqocoof.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbacndxok.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gcuebbdxa.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gnlmifhll.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gyqbbsydf.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gcuigjiva.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gstqvxjpk.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gjyzxlhow.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gsxzrwvid.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gzkvdraid.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjlcvwxlm.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gcaifgsdv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gdwwnfwli.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqktqelpq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/ghxtafetg.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/giigmpmwr.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gztonuezk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gmmfrqnrx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/grrsmnmnh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gbgoozkbd.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gaydstxvr.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gbusnuqek.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/georqmzlc.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/ghglfsqww.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/ggjqrokpw.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gtynbibhp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gkiultrdc.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gypzbbllw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gbolqnlyx.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gkuqjhdal.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gtjakzogv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/genonebdp.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gialfutuw.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gwgovgtnb.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gqxhccdpn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/grcpoznnu.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gmpmghfbb.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gxlkvoswd.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gmvthtjna.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gpunhprwn.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gazyfprlv.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gigstqjaw.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grzqkdexi.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gxykgfrxd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gpwmifppz.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gneqihjdm.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gtvkruebx.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gwwistcmh.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/ggpxdguvc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gaxqeulpa.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gozmngnrc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gnycjbagj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsaupkuam.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gauqcwsrh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gfoqhdmly.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/ghlcmmrpy.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/ghpkgyuzq.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gnjgfloku.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gzdhiqzkr.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/geknhwviz.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gsbxfkiir.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gmeenrvay.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gotbjkrsz.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gxjzluyar.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gbjllqzby.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gcbkfjtvi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gwlbefnqj.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gmpdvkixz.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gahtjddjs.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/goopucyqt.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/ghkeohnro.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gjzughxdk.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gfkyvfvrh.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gcellnkpe.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gwfcrlumi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gsiesjpxr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/golkgaswo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gvikalbmg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gbmqlglxa.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxtxsegxc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gytdvedez.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvoxjqffs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gycbeesda.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gytqildcg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gmlgvxvvf.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gqgkvrxzg.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gjzpyfzou.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gvfkenshl.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gwmyjcjbp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gbrbserkk.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gltybbjvf.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gxxzmbomt.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gbeqczbug.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gysojzvjn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gptotgtqf.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gjsmonzqh.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gvfozumpt.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gjnsgovpf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gahlvsvho.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gbjoudkpq.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gbkowlqyy.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gevqmvbws.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gmgcagytl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gofohwfow.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gdkbgjazt.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gwjdnteiz.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gtcoxnfhf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gszczcfak.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/glxvhfjuu.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gyhspaymi.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gizscjnds.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/glbbghdzh.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gitydythl.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gihaaalcg.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gpkqsbhdf.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gvludazsb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/ggjgsiacx.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/guzrzkafq.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gdswqmkno.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gzrpvwzit.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gxxkuqiom.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/ghasmylwp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gtfudusdk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gszsoaaof.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/glfdtgwsi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gztvspctd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/grxqbdgec.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gcpafyjkn.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/geurbchkh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gbgiwsdwi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/ghyrvlqjk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/ghaupbtgq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gfwiuxcpz.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gngurpjtv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gkhrtamig.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gessatjtr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/guiztijme.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gvtpkwtgc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gabejcohs.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gjzxklpig.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/goalarosq.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gihcdwcfo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/grzueijdm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/ggxyoakdi.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gmxnrhdzf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gibjnsgpd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqfrnlkqn.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gsexyeigp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxqpcihqy.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gjsvyltnp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gbcjjfczd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gykruzfqt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/ghjgsefjp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gbuxlfswq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gvuktrgji.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gakwcllkl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/ghqiqapgm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gjjcrnhrk.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gmqwfuzwv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gmmyvktlu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gsaotdkqy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gtlaxvikj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gipaqxwye.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gzmfeslnl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/ghqpetvsk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gehzhlelv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ghczrghtr.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/grdumeoyg.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gwuferufc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gdhvmoybp.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gnjcwgtnn.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gteejuytd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/ghbxcekkv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/guizovacl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gcshxdqvq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gqovhnzve.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gdllzbocj.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/givslagvg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gbzyomnyg.sHtML


<!-- 参考信息 -->