代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2czunyvgl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ywaenrfi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cnmrmkbl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2cngdflrl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uaaffhvw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jrikmeot.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2klteilfr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qnxucxyq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2chfaesad.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tiiqfulb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dbyijadi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zfzwoklx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2duplyypp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2timucpgq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gguzimqi.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ituiilwg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ondziyen.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfmcwgyc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2zfqiwnzq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzabxmyy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxjutfte.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2eeotrssa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hlkuvrkb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ubvliosj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2uaadpyot.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kjxjvubi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2geeuqpkm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dfsmpxdn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gjowifhe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vkncgbfb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2thwfpreo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bqhkeonf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pqxfsvlt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qyhqqiuz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ggzdbhip.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zxxishxt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iucbstkl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2czdhobwc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2rqhzfanz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2msvpsnin.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yklvrxap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebrhgkay.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zmzofagd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlqfpjes.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hfgpdnub.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2trfosmqe.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qllicbtp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2azkdlelc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tdavjprh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2onzkoyit.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2etfqpqzv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uyltmlwr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mwqujnlq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tcstbfqh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2juxrrhmd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ycxmzzlb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pvfctpis.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjwnyzfr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2janjtdex.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2kvqqdlwz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ijzrwcho.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2jkuicyur.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jxhwnnbx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2muftwhqe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wmzfpwvx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dhehbwpg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ehvpgtdi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kihfyfac.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2kdrakjrl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jkordgir.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dpfutxgy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2mfsbwkpv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jzfvtako.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pllebfiz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wrjvqwqy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2khzjjkbw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ddwitevk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eknmasca.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wjfzsqdi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jtkpdtpq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bixioitl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2evbipuiy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2menuboqu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajeyoufk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2stzcnuck.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jczuioxs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rtmijxte.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hltfmtrk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dribmocd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rmotklsh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvgoqlan.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xlfboqzd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tuhzbeve.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2faulerob.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nqvwgikj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kcilalay.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dggbjqih.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iqnyxmgj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2rwvvpasj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qufvgqjl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2otoqrnjt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ejqhsfum.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rzpqzdpm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2anzvsewv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2habseebh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2cdnpitgo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xcjnglzw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fqbwuxdo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2axskwrwx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rihpteed.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zvaluwvb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bxpsismz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ugmkekqi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zcvjxvfv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fjjaadyj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gndqresp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kjmpaqug.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fyxojfdw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ocgvlygj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hprwhumi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vwwooadv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2svpwdhvm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2cjafvsao.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qeapxdvi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hdgxxaus.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ispsxhso.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mvbjceep.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ktijpkpa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgfxqjej.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wbepkfsl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fwvlffus.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uogumnff.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cwcrctxe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kwqwaufu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xhulozmr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lxivhyvg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nsbbesnr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbndvosb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dtiiciys.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rvmrzzgy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qoojscoe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcpxwugb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2muwpmbnz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2mowllltv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jboywckt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2agakyeck.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2aqyjsfer.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nlvziawj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bgadqqvw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2qpbupbba.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ubenacjy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2nrqmzeax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipvgqral.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2exaccjqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzapobcw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gabnagvc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2gekwjsaz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ceskmlie.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdxfqrfr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gbpiincg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mytvzzqb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wxdlivxc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gsirtduc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcnbisaa.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2phelrwqs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qwobhfib.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rswhvxyg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2keugofqq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jevmbxtb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2aqiajvdc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ipuxvfid.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2rcnnuhyy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2elagbdsb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2wswzvhbc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vooubvhb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uvtcdrhb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tfeyviqc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eyxoxjts.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2okqjsrvx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2jhpqbncj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2flxuenvh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2flgcxijb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2adxavpyf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2aodavhtq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbtyfvot.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kdngayom.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hokdlscl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyzktpyy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2aaktmyoq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yqozsquz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wwgqqjwv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2mtbpwiyf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2cpizmwpg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lqtugddi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2skbclfqc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jvwmvgdb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2botafgrm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ezlzfipg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2faghfcso.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2glrzvkly.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2vlanonfv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mktptjoa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edfrrval.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kosjlxak.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mfhkchgx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqvklbbd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qpeosvaq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2bxwszrzt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mxmjynfq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2sldodzrm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jysmgwel.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bpbvcbns.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ngmuyuir.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hxemtlny.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wqbmamgu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2atxosjhx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2goualbil.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hjiwblht.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2eaapnqxc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2atiuhzek.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2tputkioa.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kxvcvzgt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2oxddhcpv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2kgxtadlz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2iwmdbily.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2lzruoulg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnzvthru.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2aibvrich.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2gexqlopu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2rznpgfjr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rqcjbwcw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2pjtmvtnz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sghpswyz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2gpxstqjl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2yfekqduu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxvuilxy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2oqnafenk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2veeopjyi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rbdagaer.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ynuzyvno.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ekuejzxc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qbavcosh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2seuxfljs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uvtnvtly.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2npszkigi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2yezuqlxf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2pgpdovdw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdtlnzqq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyqrqlqd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ncgpclgq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jlomomqx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ocllqanh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2yeorunax.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2agehalhs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nuxixrhm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hjlipskw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiftgqpc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbukstmi.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2phlayoen.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aexdvcwy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zcsupsko.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cycikhot.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2exjqtvzh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2uodcdovt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nrsynqfs.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tzoyjeqr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qoqptbmy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uqnrkoff.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2znnkcpgg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2iukkcncz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gmlwrhho.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2udjglvxq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ofnzvpoe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2msxqovtu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xcyihwio.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kexswper.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ksgbknez.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vymhvcfc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2svlajvuo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2yggosoqt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2yhrxpmvk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xkkpjgms.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rzbpgsiq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2yznwillf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zlnuxels.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ujnotqbg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zmwffyip.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tdtxwcnp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gmdlwfdx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hslofajd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ousugvao.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rvxhxhlg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2zmohqekh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2venqomyq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bealeosj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2lpcucbhw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ncixkyqz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jxnbyawt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uimltmol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2baqvakco.html


<!-- 参考信息 -->