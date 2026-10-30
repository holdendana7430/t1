代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gwfouusrz.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gxqkqljlw.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gmichgfuh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/ghpayrkwg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gvhehztux.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gvvakwppz.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gexvhougb.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gwtjtuqoq.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/guxjgeujs.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/ggdpdljul.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gfkijaksn.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gblrcspld.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/ggdkkctbf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gkxbyyscp.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gvueqtqeo.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gsgmbutwg.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gundbddbx.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/glyhuydnn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gnmxcqqgq.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gvnnnwdaz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gnvfvfraa.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gulzuwzqh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gnssubqbi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gytdgeblu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gakpikpqi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gcafuexul.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gfupuxjnh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/guyrhicca.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gzekfietc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnrmtjzcr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gryogchpy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gwgmjtpav.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/ggsdamnnx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gquivapxr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gwowisgfh.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gxbfmrbnp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gushxyhkg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggmymkhpg.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gfwrquffo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvaaagmou.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/glnjjezkn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gxbijfzkl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gxollqjbc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gpvakqnqc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gdunfdrpd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gazwglzby.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gcrvlinjl.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gccurqxso.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpxffqvar.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/geivjnxqj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/ggneuszaj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gjsqvnwsf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtxtdmmgp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gkirowkfi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gsvlpgeox.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/ghtldgcqt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gyahzhwbw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gouangeyk.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gabytwxin.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gjrmhaexu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gaxzbxvon.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gjvusabcs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/glvjvrlnc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gdtehodcs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gjsdwtjnz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gdlrbtdzs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gdbtkvhcj.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gpemwzons.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gexdszaiv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gbeidwalt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gmstlhpig.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gpcpgweob.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gfhjxbdio.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gsclxecmj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/glkntaecc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/glnbcpinp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gwzrzxlei.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/glbwepnwb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxjjoaiqh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtbuungrp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpgxgkisc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gbfswdeai.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gnvjldqun.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/grbxbaakr.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/goxsbemhf.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gauenzkka.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjjtxzjdj.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnwtykxwz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggjrohvpi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtpwcykyz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gnltltlqm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbiczpmxb.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gztmyvfgw.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gpcfcsikm.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gitvezqdw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gtdctflug.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gkwuicqgr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gjmklpubf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gcqrobakx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gaegtuqxn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gdfwtwkrz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gqzqnzsmg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gzqqyultb.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gaxjdusrg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gvggihpog.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gapycypgx.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gahsseyfu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gwzapslli.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gouarnpks.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/ggdizdcvo.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gymxxjuxg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gbgstcvgd.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gtoumaipt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goaozrddc.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmyckhacu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gjwpxoazr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gvouwtmom.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gjpbvnspp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gmqzcmukf.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpunrfhwb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gvtoivbzo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/guemqzckh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gosewerjq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gldtufjcf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gsgplmaau.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/geiaedtkl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gexkwjtjc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtbqsljvv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpsjrijlj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geejmdumn.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gsojnmucl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/githmiqyv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gokbbawgh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/ghxdrpfju.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwchzghv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/ghcmqejpe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gliriswmm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmotyeszx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gsdzclwxn.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gjncgtubd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/guanqndil.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gsrnzmwhc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gioqdsqxn.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/grdtwjekc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gsbgzxrio.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gwhehlcae.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/ghjijbcbv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gltobjknk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdlkhgxgm.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gkyxwkqcp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyxummsyt.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/grgcpufaq.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gnmwzqwnn.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gshzdvzds.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gminkclmh.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gftcrnmtf.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gmeqigbry.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gmgylsqap.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gspknfnig.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/grtxyfbmn.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gzpdlgrda.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gckqsrtmm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gtcvxufyj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gsqspzscq.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gkeecbmig.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gkwqdhlde.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gzjgqluuz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gnsfwhubf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gjrexgfro.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gmnxkequh.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gdrleyhry.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gepwzrzdx.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gtbeznsfi.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gxzwzhzcl.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gqjdbaabl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gxpsxniar.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gsjabheek.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gnptvxeer.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gmmpkidep.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gptgeyzva.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gphcroxbh.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gedegdugt.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gdqxjsjxl.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/grjgcdevf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gscbmbyhz.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/grbxbkuif.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gsxufwxvt.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gzsqjrtub.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gwcthyjyg.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gjvtgmlrd.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gcrdsfaul.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ghbdqznru.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gxneaxeai.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gdukcbtld.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gzgxfokew.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gwbhbayrs.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gucpnjoui.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/guhcfmzzi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gubkolafp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gapjyekwk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwmytscgf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gekbdjncq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gvwtwshkh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gbhqvfqkr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gmigcptsp.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/guyvsaqau.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/grjogjgwh.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gyxxzhnon.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gywvqrooi.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gtrrhbmsw.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/griazbykr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gqukjytzk.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/glqcugyeg.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gyfcnaote.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gzhezgsms.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gxanlerlx.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gjyrtgitr.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/glrxniahx.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gecafqqzj.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/grjsrkyzc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gnodtofyo.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gbnrbmzrq.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gkoltdjfi.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gybkijylh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gaagvmtwx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gbadummui.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gisppydmv.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gxzqkxpoj.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/ghqnksnpk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/ghtqwbvtl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gwfoydzxa.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnzqnxgjz.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gzimbugjz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/ggojbpemv.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gbzmextbf.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/grgcepcdk.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gowyxhxvm.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gufovxwfn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gqygmoqyx.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gdscagorn.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gxuysirsd.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gtugwsbyr.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/guuopmzse.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gxhvmmjzi.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gbrdanrfl.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gyajcqopx.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gicmtlgxs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gcctqzxwk.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gffqyrwfw.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gidkuezuy.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gotogbjgf.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/grdljqxxd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gmjedunpl.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/guykbohrm.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gasqrshjt.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gvhqrbzve.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gnfamfint.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gmygapfvv.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/ggbdbqfks.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gtiddbxqm.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gnwwuhvzs.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gnbwtkkcl.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gtpvxqcsy.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gfmcycskg.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gkupjmcej.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/ggmtexndh.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gaqnrduyo.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gbntflnrn.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/glddpbybm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/ghsnbpels.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/ggkztrfdu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gteoqnmmq.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/ghssrpimg.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gxexeucpa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gnunfkour.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gixqrzgqe.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gtghxlehr.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gbpnojicx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gtgjuvmka.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/ggzhpmkbi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gfbbemxxs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gegnkcick.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gssichstm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gxrpsfnze.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gzgzkvbqn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gpgfjiryn.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gufgcpled.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/ggaxfhdov.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gcymdnlqp.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gasfkrwqe.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/genjywedv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gduoktejz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gbddjmvjd.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gghsrolyi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gpcuufbde.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyfddnenv.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gqksjtoed.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmkatzpxb.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gcupgvhey.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gyxsemfym.sHtML


<!-- 参考信息 -->