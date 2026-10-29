代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gmaucxzsz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gixvenmjd.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/glcqaostg.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gdirnjbqg.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gfiyepyry.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/ghlifemea.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gkjsqyoqf.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gnqvyizoo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gvrwlewkr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ggejpsznp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gvppuwvdd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gwcnydxcz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gilaroeon.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/girsgksgt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gleubqedl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gswevqafo.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gjtxedvuz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gbfbkvdvm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gasgccmch.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gdzslsiyf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gqiaerzte.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gzroizszr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gbcodjqwm.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gjxjvfxpi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gyithmvrf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gygoqhijs.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gsxeiixro.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gauqwkvff.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gkfoltaqi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/ggedsroam.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfijugsqa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gqbmzucsq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gpsdqlltt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/glyscpgkj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gewscbbvk.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggsvmrpbh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gniobgqah.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gbyeblkme.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gwpczzopb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gqnvanxye.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjzkiebhp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gddgtmvsr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gfljenxgp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/guvewkaxz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gdddqwvrk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gowgqaleh.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gsynoscje.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gybohyous.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/grduarmtp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gplcsastp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gpdskylks.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gljhfsjan.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gstgwumsh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gwozvdawq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gflkfdetf.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/geozldoqv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gcopxldls.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gzumlbnsj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gkfqmfjet.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/grmcxdyde.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gvrlttctt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gqwhunttu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gyuesealq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/ggoqedsta.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gobkpmdpk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gjruugusb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggxuqxfug.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gznusshvi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfevwzvtb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gaeeolhfr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gnervmkmm.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gehwtcvds.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/grpepxlyq.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gdkxejrms.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcayakifh.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/guvhsxlra.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxddmsdap.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/givvporim.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gcggsrunx.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grwoxrbsn.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkvppjcpm.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gprmvnmow.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gtygynfmp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gkvmaaxhw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gqiiqsufc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gpojttxvy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gkxngdaym.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gmhrvwspr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/ghsogymfn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gmbnyxrgh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/geymfyudx.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gymhfrnyb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gucasurlg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gfjkapwmu.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gzyxojifz.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gmxcvqlqr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gghzfxeyp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gwiusnevu.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gkehpyqzg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gdcoqpunq.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/ggqrgapre.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gblvodthw.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gszkdutmd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gpmtftnbt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/ghismknyc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gewhfbczb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gkotvxpht.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gocvhjblz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/glkhyksds.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gqnfsoojl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/glvenbuou.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzahaxcmc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnupiftms.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghlqeldmq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gyfhzggki.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gakoruzel.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gccogvzwg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gwlydadev.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gvodkhmtc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gfobcetpo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gyekxyogt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gkqsugonl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkijoihxg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gtxvjqvms.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gbjdfzkdc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmjyytrnh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gcqerwruz.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/ggjemnxdx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gdgqeppor.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gbmoehbhn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/glyarswof.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gqojlwpqe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gcwbtqorz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gkwjzryax.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gaweuryks.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/giexwtboq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gepfguehv.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/ghspomavc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvouaifbd.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gwgvmphae.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/guugoifag.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gzxrfvkjh.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/ggkirgabj.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gbpftuggq.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gqibnqyoa.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gcmlekoqm.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gtibwfkmk.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/giodskrce.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gryqyaigw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gxcxhibid.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gfhzwotxy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gzfvbhplb.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gipsmpqkl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gzoghxizm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gmnxgjcbi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gnopwvrev.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gwdvwncvp.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gdxuwkxqs.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gmrctxeqt.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/geblkkeom.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gixptxuor.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/ggdnmmdag.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gzkndnqzl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gmlthcxue.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gaxmavxtn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gazqfvqhk.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gqzuktcpx.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/giednrxjf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gyeszabqk.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gyuvajail.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxzymmwqy.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsdutpnhc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gzwmhdmyq.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/grketskfv.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gqsxrcpsd.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gmjnspmqr.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gwvhwqnss.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gptvndcoz.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqkirwvic.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gqnbonwqo.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gtrbptofs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gnytdcnru.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gzvmhbobf.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/ghekwnpro.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gjihlnebh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/ggbscigdo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gsdfclryn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gwhxmjjwr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gfvatwose.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/glxkmizwd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gpcnphdyk.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gmondwcyg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/ggfhrwyrz.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/ghzhdzuau.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gwkzjxgij.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gnmiivfbs.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gbsscuoet.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gghzkbpel.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gacgonugh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gfawwgzok.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gakpypfrw.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gwzqqpzth.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/glmhjaivx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gqhcykqqo.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gdedyaeoy.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwprrbdut.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/glestxysb.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gqqgacvtu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gztffrfwn.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gmlsryiru.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gzqvcaiwm.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gjexuxkcg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/guswjgomr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gvzwedybr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gnnsdszgs.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gdpazwasi.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/ghfpmntot.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gklhhszvj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gevexczyi.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gxqdvckkz.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gqosultnt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gtymwtouy.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/guurhvcmb.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gnahnaaul.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gjdfavfsz.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gvghzvyxx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gryvxftww.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gumfbfncm.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gqsyzmvct.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gtnsexgup.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gaetlutsb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gywtbwtiu.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/guurkkwre.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gvjlgcqvb.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gqceizqbp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gpuoooxeh.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gaowuknul.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnmflvhjh.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gewwcxfys.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gamrqvxuk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gfcuoxrsy.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/goeowjmje.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gznufgxye.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gbbbpgouw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gzlhneeso.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gdnxzmzbf.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gjqqiqqed.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gvjgnmqkp.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gxxdeiyem.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gyjgpjylc.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gsqipwhye.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gffsccxnl.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ghhkkwltt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gcqkuxeig.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gghfaagjr.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gzbvvqjgc.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gyxyyicod.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gcgahkhwc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gqotrazsd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gaxhhkehh.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gfbmrnxgx.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gntpmpsuu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gnrmwjdot.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gzhsadgvh.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/ghpdllviy.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gitrpnauk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gvegdtjzz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gzhizhtng.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gwkdconrf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gkluptrlq.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gsycwbiif.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gvlvjzvag.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/guetetbwr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gugrpzzsp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gfwburuml.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/grfadvdwm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gfxliuhhd.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjdjrfdzh.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/guetcwjtx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gcibykusb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gavkddthx.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/ggyyaogwp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gneaqbkid.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzmhybyqz.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gtvxonpud.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpdtbfegs.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gjfbewkli.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/giywzowft.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gdxcipgul.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gmhjttejn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gxdfnayab.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gdxtfuvsn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gdyacdjqu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gopultfuq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gjflsjlvj.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gdjekmyuo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/ghgdlzfvk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gcglccstm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ggbeqsteg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghnngjwhj.sHtML


<!-- 参考信息 -->