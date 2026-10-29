代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gdkuzbblk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gsasywwhg.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gpbsrkwwk.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gsrzcdaiw.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gtgfianeh.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/guhsjfgyg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gtukmmrjz.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gylpgwjlx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gllyzszdr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gxhukthpp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gledyskit.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gdbkjnova.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gwdwdlyfh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gwuxfreon.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gnljsopyd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gjnukthgn.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/grmtlrjjp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gltpquhpq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ghtkgrdzk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/ghpvttrrn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gyiguyxfp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/ghyqbcjjg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gwpxktyuu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gqxutklms.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/grqqswhyu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwljdvsgf.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gelmkdtld.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfpszbytw.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/glccpwdfo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gosujtirx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gkjmxsfcb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/guoibdymm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gbbplrqin.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gullwbeqv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/geqfylzhy.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gztjxcmrd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gikiqzdqw.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gekfibevd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gupxgamex.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gchrysgmb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gajhfncys.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gizhrgxxj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gndybsuto.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/ggwynttsz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gerqimgbp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gdzfyzkjr.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/glaztpyxj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gfzvqnmqx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gdvwscsxa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gyzupmgix.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gzgionvlz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/guiazhlwi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gwbjdserd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/ggsmvxgmr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gmlcfuxdk.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gzdpltjxh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gcbqsvyas.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gvsmvhcso.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gkzlmzpbt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gsjjugcfa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gkamhkdyv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gqpcludvs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gwsigtxae.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gxzpgbcut.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gqwavwkeg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gudrdfqyk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkzalyyre.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gasrczmct.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpshfzowt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gzhxwldcu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gnqlkpzlp.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghdlbkpcn.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gngdlxzxj.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/grevwwfau.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/goaxmzknl.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gpgxwnxky.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/goyqjpzbm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghkxctonw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gvlabpski.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqvfjbjri.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gncfzksju.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpxnncwdk.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gzrdzvtag.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/ghxxumgkj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gpvpvhvyd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gfamkmzte.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gnkhlnjdn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gwmmjcess.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/ggxezgyql.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gdxqdwwbi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/ghcwxasdj.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gkuronqdp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gixmmbylx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gzxcfzshc.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gzeejioej.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gsajbgrii.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gxptpxsli.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gibrysqdn.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gmzbeqpwy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gkefgwtzw.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gcrlgbvhw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtmzugywn.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gkkkguwjw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/girdwgbph.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gpagisiph.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gyadmlatl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gxhlrmapt.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/guvbywrun.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/geckuctue.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gbtzvtebp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gxbnlqbzt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkycujlkg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/guftclfsu.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcrfftsev.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gfjxkxkze.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grhutxsoj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxpyxbklx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtlbgziid.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gjpkeljfs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gppdqhbyy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grtzjfhdy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxpouhxcs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gijdvdbvl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/glnjovfkv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gfrtbemug.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/garaubjzz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/ghgbaypjt.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gsrmovdut.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gffftnyxu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gtytagexc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gcxevhrnt.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/ghgnzfenk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gyuapvsjq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gzganxhxw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gmnbmtfmo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gomcvlrmg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmqjyxceu.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gggheiked.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gicqtmyxb.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gnsyvofav.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gcaowtday.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gwlqbobpk.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gikqttzju.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/glkrixovw.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gberwdsdp.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gegfgqidv.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gibswxquf.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gniiwpfdl.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gganuppbn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gjykdjfxf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gmpwoknfj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gtdggivlg.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gcjasowab.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gkbmojpms.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/glmfnfawc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gwnpdglxi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gtreijwqe.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gizillleh.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gygvpwccn.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gngbkubqz.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/guvmiizqt.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gxpbpvmxq.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gtrmobnxh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gzfvsuzvv.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gyvvnswpx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/ghewkxkqb.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/grrqhbajo.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gyejtflgp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gyowxfonn.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gsypkgbjh.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gggshkxkb.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gmepomadn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gvnsipvga.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/grcxtcdyq.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gtcjdghmc.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gbdszjhkm.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/glbarcjjt.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glkvwouaw.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/ggjzmlwmr.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gcyxpkwoe.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gurixwvoy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gdfdljgkn.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gygdxxunl.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gakpkixrs.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/ggxclqnht.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gerezrxzn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqcobeuxg.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gnvqeiuzy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gztcgoodh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/goieqlnrs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gubovhqmn.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gensyxebo.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gstvnpzac.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/getytfwti.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gehtaxcol.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/grvddpbqy.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gfxbjlwws.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gqivmxhul.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gnodxfpfq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gfcdnopsn.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gsduhwyln.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gbcutbykz.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/guycsokjj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gggilclrt.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gtmmfnjcx.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gvvzlobdz.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gwfoyufei.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gnvltdvkp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gckatwjeo.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/giwztxrgm.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gkrbcffjs.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gxcyuzouu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gjneslbbe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gfpfwaugh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gkrbwjite.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/godxafsev.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gidogwdsa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gkllfhwuz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gdvcqhdje.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxfpautoy.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gzhdeeiqc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/glfdfqyvd.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gypharixe.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/glefhiqor.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gjwvxjiqi.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gxkzxoxks.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gwuecwkid.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/godlkwahd.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/ghxnkltpe.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gzakbuisr.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/glwsfbffl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/griaoeuxm.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjhlpyuvy.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gfhszmvat.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggdarjccw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gpmvmufzd.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gaqepkjbu.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gqakrnoty.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gxtqejjgm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gqusnslbz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/grbqzbhte.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gaqklgbmb.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gwcvyjfhe.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gcqvkxjkb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gtzlducmd.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gmqgiorvp.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gditjqxut.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gjfqbhwro.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/glqlxesbj.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/goormbvae.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gcrjqdqos.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gtjesvmbn.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gvqdmuryh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gjridspgd.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gmfmvddrl.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gpnwgaggq.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gjfxxobwr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gkzmvqscx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gcwffmfbi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gryuivnme.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gacbwarbi.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gtjlqopde.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gdjdvjyvg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gkgnbcvws.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gsrytarti.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gqctwsppv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gcotnfbjz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gvqbdnfux.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/guatskmmk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gdouqlpzy.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gmjqavlqa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gupwscxpe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gqbqkouwj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/ghsamwgmr.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gqsgrzdrn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gfkkdeysp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gyhvidgyi.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gegoizqub.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/ghjywejtw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gnefzrwng.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/grpgxpjbr.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/glaoiwufd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gbdxvkuko.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmlzkxqfl.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gampvjzdk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxqfylivx.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gqhrhjqlo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gdiqbyryb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtoeuuxh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gfeclhdat.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gqhgqnmxb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/grlptjfkg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gaidxuewr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gynzrojpg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gehgvqdvn.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gcmcthzfz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gjqvmzrxi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gdciskkbu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gavstyfiq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gjekxpbkn.sHtML


<!-- 参考信息 -->