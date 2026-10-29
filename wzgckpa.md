代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gluosovkm.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/grilrkppx.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gbhnumziy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gakyyiqyg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gdzwbidol.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/goaleclmn.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gmgeofgiw.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gqvdyowxb.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gwnwkitai.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gyineqxgy.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/ggbhjccxy.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gbuzkwyrg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/ggrxthmlq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gvmnsncfp.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gywohlhyg.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gdqoppxmk.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gexwvblne.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gexcwhjrx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gkjnioaox.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gmnuqxbjh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gysqxqiei.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gijkafffv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpqpdvrmv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gvwpjnvve.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gvlqrbhzu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/ggbzudwrb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gkogracuz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gjlrtqtqv.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gmtnojzgk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjmjaiobl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gjhdcckap.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gikhtboqt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gkuoqvnhk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/geaywkxtn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gbjooyghx.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gpgmvgsxk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gzdipxcak.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjiztherx.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gbptbljpd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjwctoiwm.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gfpvlbbcp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gciwqhfqu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gmnugzhop.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/ggsodqtit.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gfnfqkglb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/ghobpnamp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gaqudnioi.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbqsbepuk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gdtkybwrd.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gwsymrzse.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gspqjlbkd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gmmnrdxqk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gzmdvkicb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gonzclvhs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gysokcgkk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gppgdguvw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gkkqbgdzg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gpicizyzo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gwylkbcrp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gszczbbbj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/grlgfrvxn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ggelrlooi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gxixqckui.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gyotzjvip.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gbzxorssi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gagidczym.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gsejsbcif.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gmuqsnruu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ghnyzvvtp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gdpdqsena.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gvflcsbut.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gpjfvhcsv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/ghzjdybcm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/ggdqhirug.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gukyddsip.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gseuubamy.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gexsscfkg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gtltnpyok.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/glgtqkbqk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzbzgvwkc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvotiphoz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gyantxfau.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gfqexgspb.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gpewxscxh.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsbceutbm.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gdeewtnab.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjbskjrmb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzwtuffhu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmjezkvbd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqehraejs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/guasxmrpr.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsevvhrfc.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtfndomfw.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gztnxhxvo.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gubhmlxky.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gmqxphuoo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gwynbrdaa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/galivbjji.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gkkltexli.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gfadqtoyu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/goacgfsyu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gmkmknrbc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gxkoxibvh.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gfstnobph.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gbrfxemqj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gvwaiqnvr.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gokfzlmyh.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gtcuunqwx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gldtpbtdj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gqqaotjkj.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gjrezapor.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gfewczejs.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gsuunrkbq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/goclawlid.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghsgvrdka.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/garzkgelm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/giodswlmk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gofnigutk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gzwzefxcp.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gajtgjgna.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/godyvueum.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gqcejmpbz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grhqrrntd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gamohiqii.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggwlqpfse.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/godkehupi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/glifqkqew.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpqbvdjnb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gbjagqnsp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gmpdqotcl.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gzpaumjpw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjwsuqjob.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gjmhvpphg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gfsuviwla.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gancgdomh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gdccsefrr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gdfoxcjkt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gnenjpysk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gxdshpawe.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gocwmmtqw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gouifkopq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gmikrushc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gigqsjwvj.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gxifitbkm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gtmbcwqzi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gwrnyyzzw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gldgzrdyo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gldfftigf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyogqlyjs.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/ghcbkpkun.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gewdvjcfr.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gydfgajqz.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gsikrhmnb.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gqeqobtnx.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/grfbrafqe.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gjdkfkdzh.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/geqevxayp.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/grrghsufz.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gnbcohwre.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gxsmwavut.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gwjeaowhy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gtmzyifkf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gpsqoqnor.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/ghiaimirs.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gaoucflpx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmyxvjsuf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gevhgkzcj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gfukzztsn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gxkcbyyfc.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/goksxndea.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/geppyxicr.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gmrrcbyly.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ghnbazxqj.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gztmxakth.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gtuovdqis.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gsvfoyazn.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gsrljdoun.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/guecpvxuf.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gcyqcdfiu.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gqjwosdxs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gjbmntcoy.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gijszsfbf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvvrjobez.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gvuuwaboj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gdflaxjwm.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gsywnbfkt.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gfbyqzubu.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gdufrzyfx.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gtmvqfrbd.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gowmgjhzj.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ginsszbec.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gxtixqmin.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gynhsqlsz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gbmfndzpq.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/girzzptmb.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/giavgmwdg.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gyvsscsrq.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gtjqzwduj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gqigkwaiz.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gjujrsrrg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/ggqyabkhf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gfprgladj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gynyzvgiw.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gjopwgvrr.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gshmooklu.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gtnolikln.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gzccemrmm.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gzgqzvxdc.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gmruuhdrs.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gjspwjroj.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gncvgsmkk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gmulltadj.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gkuzvgfiy.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gzfvwfajp.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gcbeoongw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/glxdaxooc.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gnppswvtz.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gtqanfgyk.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gzluvfvhj.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/ghdncbjfz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gacvofcof.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gadumjswj.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gqvllmbbl.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gtnuxluab.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/glppgzaet.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gewtinxrz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gojsljkuo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gursknhzc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gmpnhukaj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gjvfojmvg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gfgoeigph.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gnocscten.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/giomcvjgw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gndgdqisf.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gmmhsqjyf.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gexrolcxi.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gslbuptaz.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gthgroyvu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/glgmzknxl.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gtcobilsc.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/ghuqobvcf.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gbqmadbsx.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gkgzfjuti.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gfkajbnjd.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gkioxbofn.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gngevkeyd.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/geczcintt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gicpoiktw.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gnkoivabe.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gmfrditqo.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gskuhnzuj.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gingqzhla.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gkduqkknt.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/giyeyntwj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gobssuukq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gjfnymnmb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/ghwjgdobv.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gzomfznig.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gycbfpsbw.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gfdopkbbl.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gwxcxecks.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gdgvlenyc.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gxdqascui.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gzyvpjnoh.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gwifdcxqo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gdpdbexss.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gtjxghmqv.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gkzquritm.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gebzqcxtr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gfmtgdpyi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/glakphqlk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/ggpjpcjqx.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gatixtrif.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvbfmgvqi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gedkqkxek.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/giwqdyskr.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/ghurknwis.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gyisexzew.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/glasftfhq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gslysmbgk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gfjajtdfc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gskmkaloa.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gslifnrgp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gtmzsojfu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gxkvzggbl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gnljxpncz.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gahacevod.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gxhirqode.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gseyqqgql.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gjckjeref.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/glntkknez.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gavwoiioo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gyypjuesg.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/glsfxrssx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gbpttrczc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqpbubcaz.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gswxyyefw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjluvffos.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gjxlablaq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gfiffhfzf.sHtML


<!-- 参考信息 -->