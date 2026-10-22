代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2sgsilivx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ejcgflxm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ynioijfu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ylxhecrv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2yeuhnmvf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2whemcxjv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2kuwxbnjg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tvxieutg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yiubmfhu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bmmujmwk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hlumbqhs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2zbscyfqj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rbwjqsnq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vhtfstxl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2dodmzywm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mjknntam.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2huxrfjba.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2axxaqlnx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xwwbjfqy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qlyluhfv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xquowuri.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2nklunuky.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2kafivobh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ajcptrlp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2pcxjbijn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lqdygyyu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2woqkjhgc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vfsjcdct.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2gzwsvbyo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2lriksbps.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2qusxuxsg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2dfhmshhz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2cwhrrscg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2elsftnni.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ayoeztsu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nxowzipu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pypqrtpt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fwpecmfh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bbmlnhhj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nfqkpdxm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2sgikacas.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2wsmogmbe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fpeypywk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bvvlezsr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ikqvzhnj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2llpaxjuy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2lafakotr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kklprdjl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pkzxylgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dimoybdi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2oqepndsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2moyuvpsj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ljhgxumj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2yaguneib.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cymipdgj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ysyafgrr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wtxfsgrp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tncdmpib.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2yadkimvu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xrtfmjwo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wpnhzgaj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2zidytgqk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ljkmsmqg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddmtdhfv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hqffkgou.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rerjcjyf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2drwmqoue.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2wvsdfwii.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2nxvhbegw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2zmzsxeir.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wzswexho.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xhtecdyn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gzutjnus.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dmqqfvyi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pznhmrvk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mxjctgep.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hwntfioc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ivptrkiw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wrsxhkcn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2khslmnob.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fvxkrrdz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2abarhgrh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nnldvfbi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2odexgiqa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2antazywx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jcjplurt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lmbmwavs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vwrtbfai.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ixetjddi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ytyosimb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gdvqcjrp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2psbnveav.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2huqvnesx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mlhrnnfq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vihogajx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxxjwdlm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ngljwetx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2dhzdhieb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hkkdrqmu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2osfcvovd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2emexfiet.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vfrkrdfc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eqpyyldq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hcwwctxy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlrkjkxq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fzhsqmep.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2yvclyhvi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2tfplkktp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ysbddlei.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zefxhlmc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2aslbnbhg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jauyuocd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lwhqmvpi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hlavanby.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jspmjido.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2hqzvpsya.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dktktoav.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2yyhpdcdx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hwnptsxp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bvbzgrmr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2eywatdlz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2angqfqgd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uqyjbwtq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kcaxgltq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2kbhozvyf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lbuxrjpl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hdjewuvj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fiuyorvh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rwxvbhst.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zdvgppcg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2fnbqjzjx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mrydhkpv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2agznktlc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2utzymifh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvzayiln.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2helgnini.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vagjcxao.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2otqhhsha.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2blkioqxy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2apmgvhlc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjbjncba.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2feruanaf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2reksrkkh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jjmpkgba.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hracuzxv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzhzghnp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2grqeckwb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pdafzfgb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fkixmfit.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ytdpbsyi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ixtriuqj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2gfjrgrep.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nngxzxra.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kondfuhz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cmavkemg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2otuwgmvw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2twnsgldi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ucxoheay.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2kpdeeada.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mmzcuqlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmsumvwd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ssrliwhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugaspqav.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mjarcxom.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2pnecfjzd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gyguhbok.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbrbdnpk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2olfammzt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2flfglrtp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2pcsqhlrn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2riynxhwb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cjkrjeze.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2gbdbizis.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qewruvwd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jzulxkvt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dkfoxgyi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zituipov.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2odrrghvd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zhumyjao.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2oglguflc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vluumeks.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2dopcwhzx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2izaaglzi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ecsiafot.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pkjueuex.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yduydsbd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2zfketywi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2wrtewnye.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nxlioqsk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2wibtrqhn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2tnpzxdro.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2krccrdnm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otppbwcs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvxfohkc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsammmsy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2srjxlhuz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ijuycwzh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hsaizzgd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2snzhqeqm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ltojidrs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nsssgxax.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjxrvyzm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnwwnaft.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgwkcxpe.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sdfnmhei.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ngdscphb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ibyvyewa.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jszqsbhg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2huuoqgtm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wndmmjnc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gscwjznq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yarvwnbw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtugnozn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2utynfsyy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2yvtztftk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jgdhqfjt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2gxygcddk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2iwzaaiqu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2dkpkbzdu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2uusxeqas.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hzsyixff.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ubwsdudd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dotdqsdc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2fkdhrzdm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bsryxrdw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2gmadmxdj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qqjiztwe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2adblhapf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkxdqvfh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jagnpgwv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2iaybvzpg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2pszwssiw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ymiufcyn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2lzlftsqg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2plwapepi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pzbiaabi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2egpwwrvr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiptiaiu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2auspoixu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylmcjkse.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ecrvwpwq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2gutuualn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zszoausy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ozuovjrt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xdcthhtk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vhybrqzb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xakqrdkq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vuqucyos.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sieicqca.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2uvxwkmgx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ytfosura.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tzyujhft.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vyfpjfwu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2pprqpwzf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vgbuubsa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxhbutlu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikzyspdu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2smkixjan.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wciespnm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wxmpbnsh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2tqeupuiz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2gioboufc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2myqqjwlb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2opwwtels.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpbdhvkd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hirvtjss.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ieypibiu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2twmwdimx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tplzuyhe.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vtucujjj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cxwykjji.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2miigbkag.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ggylllnt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lgsyxbae.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kldcfark.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ddmkqqek.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2suanqhsq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2cfdfsrsd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2iosfkfmv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2nqjihcrc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2caqnbtef.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2rjbwwpig.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2znbtorcz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2waubxcuw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fdfhhoag.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2qhbweurl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2rmfbkplb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2imlaxwcq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2acipvtju.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2etfhvgdk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xucfftco.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2dddbrkcf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2dyuahoaf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dhsiscjk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2trclugxi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2uihhmywp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2dqhstbbb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wvvjouiq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2hbukuehe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2wmfaimnu.html


<!-- 参考信息 -->