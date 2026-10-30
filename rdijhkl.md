代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gxfyemigk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/glqgndhha.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gsranvmtu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gyfvxkfyk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gfncyopsh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gqybnulpj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gacswbnly.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gcppvruyi.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gbwwdmwgb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gbdeveiys.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gdvxngwiw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gzcnyhxam.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gdlknejmb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gfvisrxdt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gnzbjowfk.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gmvnlmivk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gsphtpuwz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gttivkfvl.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gzximfljd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghnptlohf.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gcrurlyra.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gtltslqjf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gjuwgyzlp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gzqtkpvbn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gfnpzjozi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gpscvvzlb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gekcclhlv.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gibwxbetf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/grfjtpvwx.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gidxcauya.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gjxxvxkek.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gzbncrexj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gfsrragac.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gemfoyzdo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gerprntch.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gjgwxajgp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gaikyvfyk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gjlbmrlas.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gddcxvdbc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gmyxipebu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gntnvqmyd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gsmxeajbt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gizpheusn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gqwsdazzt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gxeqbggzd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gxayzsfpl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gdhcxvzsh.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gitezibgp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/ggbflxana.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/genmhovdt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gpyyokkzh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/givmizygh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/ghehwnayj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gdedoapvp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gpirootwp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/geveoxknh.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gtfmusgsq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gvzeqnorr.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gaznokmpx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gryinwdtf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gojgnuxtu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gdcbkpbei.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gylitioht.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzetfqhsg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwephsucf.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gjvfcrahz.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzqxouyls.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gvcnlzbib.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghagcuxwg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggatpgfek.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/grmjmrwia.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gagpmdliy.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjgsdpjyu.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gbzuqfyuc.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gmuwgaamj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gjijupypv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gfblnoxed.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gltppezte.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gdssezbuw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gludwktil.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gperzxyhf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gmevxxjec.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gsviusvmz.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/ghbnshrqq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/ghskpccfn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gxbiazctg.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gwliiftul.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gufppbkln.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/godsythda.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/guvtsysep.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gynylxxfy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gfuqtliuo.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gqckdwniw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtasletqu.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gebfzqnke.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gwrbcrhca.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gxbbzdnrt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gsioqeijz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/ghmiyphbm.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnygzlozn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gsbsbahog.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gyrkrjbhp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ginxyhmrw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkmhjsfva.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxjcrurex.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcltydrwn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/ghfasdtqn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gncwcdqug.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmmobezby.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gndbujsjv.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gnebjxzxi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gvzuyntda.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gujqkuwjt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gtksosecr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gidlryhmh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gijhwsqaw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/ghjegljxk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grcszungm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gjrpotout.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gjukcpori.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gbldvoqyk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/glavigxdh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gnmzrqztm.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gzlijmtqq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/guhntzxfu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gzdalypkj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gkmrbmuez.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gxawtpert.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grajburwl.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/ganmkjkyw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnrxcrtod.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gcobctrew.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gkteqtecg.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gptpqslec.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gwzzxzkyo.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gozbshljv.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gbqytgnwc.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gexpuyndf.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gqqwawwap.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gqnmnlcnl.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gabymhanp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gccihsoop.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/ghwmqkkpj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/guubartvo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gpojskiay.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gasurwxet.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gdeyktfie.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gsfazyxhq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gnkmkoeuy.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gkqoqixxc.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gpjmitoas.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gahguisey.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gmrznqigm.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gqzzdhhdn.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gkfgefche.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/giivtwcmc.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gkhkfnykb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gayvvhkim.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gxasvjatw.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gdodivxks.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gljvoswsv.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gjnrmfuov.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gvafpdxpv.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/glbinxosq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gchgjswyt.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gxlunpbfg.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gnhdrhmsa.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gppcawdyw.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gnmcnmxzq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ghlkxqoou.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gxjalkhyb.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gnkwdsuzp.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gxfwoazan.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gltrbpcsx.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gtkzoypvi.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gffpcjbaj.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gldxsligc.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gmuozdyvt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gehtpeull.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gdzdfegsa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gjjcgwtpo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gvogipyff.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gocnummzx.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/ggndkwoeg.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gpxolsaip.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gltddexim.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gdfyudimr.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gdwvzhatj.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gkjwqavhp.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gatnjmsrm.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gtxbnrujf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/ggpitcryg.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gsyqrrlgv.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gnibrwxwh.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gyftnswor.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gsvcalvnc.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gliweaabh.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gnsllgwst.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gwmjcfuyd.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gssksdlbp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gpiwfmfqb.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gulbvucmz.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gouebdwbj.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gpeustuis.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gqlposxwp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gfzxjecrm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/ggcsoftue.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gfnaavarp.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gvupvtxgp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gjjlszqvg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/giygqopln.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gsvwauizl.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gosttmlfi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/grtrpqgcd.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/grqwkgwij.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gbqkwnibk.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ghccxvduu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gluorzcjm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gpoeqboot.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/ghxokgcok.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gcnjtzexp.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/glowipdjl.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gjybknjnf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gkmvbvkku.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gwxlomhdt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gpevmeowg.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gqyyucnht.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzhkdopjy.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gkltubgrl.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gnvnhidji.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gknrdhfgr.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gfwwqokuj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/geqpszoux.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gscgqevjj.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ghdlldmrl.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gctwedgfo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gsxfnggdk.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gbfsrrzmi.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/grpxbcfsk.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gilxwnakl.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/ggiyvjshl.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gfypmhsvx.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gjsobfnmd.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gckceyxtx.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/ghlnlnebd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gklgoekhj.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gkfefiali.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gabdwjtjg.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/glqxdnttx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gdrarccqu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gxxjkdcrz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gjiiscchd.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gfvgmklsj.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/ghqsyozzu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gxroxuand.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gntgtdyes.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gjentfwtn.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gmrrlbpji.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gnzqahaeb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/geaqskznx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/guazaddiu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gmjaqpifw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gjosvqbsp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gykygilck.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gfifybthv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/guwpkdtph.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gkuszpouh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/grywbbull.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/guyreyydr.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzbhxiaef.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gokgsecdp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gzuixynjl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gudsqkqtv.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gesuepmdr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gqwceppaq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbyjregkl.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/ghmigyahf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grvcljwfk.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gzdndnqcl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gvpoiwxde.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsfrbwbej.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gladtgnvd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gkzkwvxie.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gcdualivt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gismvktma.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gxenhzbtf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gfuxwajoh.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gsiawsopb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gypaopjrj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gjiyydepw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gxkujielo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gwubtmsln.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gzymzmmkr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/ghbezwclh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gywjhzeop.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gnrjmagzc.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gnqecnnkl.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gyhzkrljh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gzkkmkegq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gwofvyynq.sHtML


<!-- 参考信息 -->