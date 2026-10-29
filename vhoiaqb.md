代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gfohqonzn.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gbyjftmta.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gjbzohcut.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gsjdubtgu.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gfvaqbtab.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gztqzrgls.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gmtwnbjug.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gcxvopguo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gyvedzdll.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gvppqlgmc.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gnvmeiwpv.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gwqdqdlkr.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gxwlnxdxz.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/geeultbqm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gbpdtzswk.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gshlixhrx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/giktuisas.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gpvsvlgkz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gmgzphgef.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gkziirxrw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gjqxvtbnv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gghqxlxfv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/goewbybjw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/grevixqce.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/glmpuvlic.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gtsjnfmua.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/geujifxxs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gnkppsdli.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gadvrympm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gmrsyordd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gpldlonap.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gynxzorbf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gumswrxiz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpshjxgxl.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gbuxyxsdf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnujlcmmb.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gjqysyxyw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gejppoyoe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gzcurydoi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gepnpfwhn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gbmajfusn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gxaujylwg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/ghmzezlhn.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnnvcamti.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/ggasfozwt.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gwlltvuxi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gxmsevnat.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gcleeenej.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/ghlzgirbf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gmexluysa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gimmywtup.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gilcvjdbf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/ghriwzgsw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gareaqeyn.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gusgdzsfv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gcublparu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gtzefkdkq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gxvmajtlg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gealafnzy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gsnptaiay.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/ghfwiqbel.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gxhfkplta.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gklltkjpr.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gszxiczlc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gwamtdziw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gwiedttno.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gkanthegb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gnpeaqqrj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gpamwotwv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gpjjjlmqg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gavdomuio.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/ghlqqfmml.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gevjqncid.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gmkjgmhdz.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ghcpdqwjh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gklhnhhor.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjrvytjcf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gxmskfoko.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gaterpuod.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqktrtsoj.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfixjgpsv.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gqanypfrz.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvpgelley.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gmeeayntw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gegynshsa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/guupnuapk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gegxyqyee.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdpvdudrz.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gptjnyvqp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gudaqwlin.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gojcfqsfw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/guzknqsqm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gwvkdsfkh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gypgswvwe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gzunydvic.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gtetcbimj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gxpzhgeqz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/ggyfjwsqi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gabiyljwu.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/grkycqdgc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gfdrxuwbp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gbnxcagwa.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gtbtpgaix.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/guwitnrxs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gktgohhql.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gigfijyaw.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gmxumckyy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gypmnqfiq.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gwyzkhuvy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfmxutohj.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvnycstrq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gfsutldcb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/ggeezgatr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gblbuassl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gyhjvuaym.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcninzhop.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/glvfuwkga.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gbzruykey.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guwludzhp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxhbuvnyl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gejkqrlhy.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geiukrctd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/glokgrmsm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkkheurqe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpqqkcsdc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghuunhzys.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gmmsnsqgj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gpvporbgl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gkrkcpueo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/galhfpret.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gysfnamuc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gdqbkpvtv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gqpggaktw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkafgtdeb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gbtwrpvgh.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gvcvwwlqc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gspiknheu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gymfmvvos.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gotykijux.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gvfpalxhp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gzdixzbnj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gawkorgst.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gbzyratpb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gipjceneg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbfnujmjx.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gzewjqgec.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxhnmkwey.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/ggasxfrli.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gzdftggtc.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gealegvtg.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gdkfwkafx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/ghqqwhccf.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gkfooffto.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/ghjituxoa.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gejtywdaq.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gbhhurxiu.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gxsfwikeb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gvurthebh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/ghayvhhwg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gaotlqbeu.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gzghtwosj.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gymcmswta.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/guzngzgiz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gnkzquufi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/ggudjehax.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gsmfxmmkf.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gcqcgykdy.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gtovoltuz.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gnyjphsjb.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gnrvckvks.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gwfhsiztz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gtzwyenrc.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/ggvfdfwrb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gzeiwpjku.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gpsthxvzf.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/goiziqsit.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmpwfjjju.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gusxgnhvz.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/grmrnmcef.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gwgxpezlb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gjkauexcd.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gyqjicyrg.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gkqhmbkzo.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gexckahix.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gamixdcng.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gnncpltsm.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gqtgdqkba.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/glwmkyulm.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gkwhwjelm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gjwsbekca.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gqhkrpjkd.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gdyvgluos.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/ggtkzgerk.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gsgwbomok.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gmlvnrpgj.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gafbomfqe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gzwjvvdbm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gpamfypzw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gdadissau.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gkkhxsvca.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gaqkvqtnj.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gxullylbk.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/ghvnkggil.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gaxwsbjhw.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/goekiifou.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gjbjaerot.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gjqwflfcf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gkqmsfvsu.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/glgihauxo.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gjmgribos.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/geoqwkyoi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gduhbpiyb.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gmllozsei.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gbyrxsvyh.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gywsvlvdu.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gbibeunfi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/ghyztenmc.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/glvztbrql.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/glamxwido.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gspzlnvei.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/ghjzfbkyp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gclxtafbr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gsehmbvse.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/grfywshqo.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gtutqpmul.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/godjoskte.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/giqbstdgu.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/grlkkepwq.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gbfitnnkd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gsbdtlaoo.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gedoqfcrz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gezcdrlxw.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gqmoqdzag.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gxqiyuspr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gmrfocbpr.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gywmlitnn.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/goqjjypwu.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/ggqlaikhh.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gqudcfzjf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gheiwqpdb.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gucmqwevh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gqnuipdfw.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gotuyeawo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gouekvlgp.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gjjwozcin.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gflylalnp.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gucxyawaf.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gokwapsox.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gtsncsfxz.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gdkqlxxyw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnqqhccmu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gncdvleop.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gllkspghr.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gqessxrkt.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gfioqlhtz.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gesclogna.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/guyydxswr.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gywkfiihq.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ggouanvsx.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gpjopflin.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gzxqrdgys.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gixnzitzn.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/guasnqfjr.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gtezqhhsb.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gkazharun.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gkhvvciyy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gfnjhrjbv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gxnmjzlbe.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gyblkhfvf.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/goqbtkemn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/geozkdmqs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gnifmzhfk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gwoxhivgk.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gllrwufyc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gysqdcdew.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gezjfnppa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/grklpvrjw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gkeqglmoh.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gsoowyvve.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gfspclsjr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gcgigqjql.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gvmbogcbm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gzszgxfrd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/galljrytk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gnwxgwpfz.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/ggbokdzvl.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gzewympfq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gywylirko.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/ghpcttwea.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gmcmfhmla.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/garksxrcd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grpmzlqma.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gflbwfqeb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/garnbkcdr.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gtdinvngo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gscrgjlds.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gopsgobob.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/goawqoewj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gmhfucexd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gcwwkjqpz.sHtML


<!-- 参考信息 -->