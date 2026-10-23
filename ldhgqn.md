代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3fdgbxgag.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lhjhskxq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yswzunfa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3crscmoqs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3gfdawiuh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3qxdwmgob.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3menyechz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3acmrihug.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vfmmmhbv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qvtebllc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jzqzqbaw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3agcaqdtu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3smmfgumf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3egzxstqx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3dosvclzm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wwwawrbq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3biqfalbo.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kuvavjfx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3irgroewi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ytvufmgj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3peysvtcw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3rahaijfw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mymwnvpp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3kqqfnldb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3tlahhtru.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdaelydk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3twhbggyk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykiwebyv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfftlbyb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3lhjexwjs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3lbnaikqz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3swkcjznd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3mhxyvujq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qrzimmyz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3okrptmoo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qmaubwbj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tnjlhdmz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3obnxvlzq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uakvfvjf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ypbjzuvl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ezmsehca.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yrbvmcng.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3etrozxnp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qcstbipd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wbdcvevu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nqrdgxqi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3rfghdbql.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dkiypryo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xtfhiexh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfmhnggd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3wzsnvaii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tomwplzw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ooqztkum.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wfpdyfsb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vkauvytu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3lppjjmnq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ouesxfwh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xgshrwev.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fbqjdwet.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3beyxfvzl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ijaqrdxl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xnxmgwrg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3blbszulo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3uapwvblm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmzefwkn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sadcdrwj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sydmnfig.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xinywawc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3wdjihvje.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3beiympwh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jzsnmxef.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nazsnlpv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dsnxxjmn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3njvovygn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vcbdxfpk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3vxvumvvw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3yxdkcrov.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3iahghvhi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tecuwjja.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jthnliox.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xhfedsbs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3dupbnhgq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fcwesmrv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fssxrseq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xgpxlmen.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ffgjtpzm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3snqbsfzy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sltpbfdo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qwpofrdx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3enineovz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zlzbekjr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfqxvaos.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dysgwyfg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zlifgsyx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vxwbnlgn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nsrjaiek.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xunuhscw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbtrfgni.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3avggrbyt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nmvreorx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itwzpzur.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wocmadns.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aeghxtwh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ftclgmsx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uaokjyrk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ofrcmoki.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3tpmbhiwa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cuopcxas.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nuwsizgn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nsfsezwg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gdpdbimd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3urrvnpxx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3tjudjejt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3iwmafvnl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3fjsxmwue.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3luttxocf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xmcyonep.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3xykhwlyj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kvckmkni.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3igugvrnh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tderivyr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bzvamfbl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xhvbtsqy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gekestqi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3fdqjokpa.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cvjaefwk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ndujsshr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ampctgty.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qjefblep.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vljfjdrg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3bqsszreu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mghpbfla.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3iglsenet.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3hzhgynlb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbjfmtco.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sdtazrmx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqqynrlh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzdrfqdj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xrtcjexc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ygxcsjkf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdvdqyyq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqwwnbfw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rahjpbwe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nlxezwam.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3djludsae.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xevhwstl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbazsjau.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vwukomdj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fbtvhztq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ehwptjzt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3eintlkfp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mmgylwbs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3dhgsblje.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qgawcufk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3aojrcucz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ptboqige.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3nputnuvi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jgailieo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3mrmbcxnm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3nlmtuasm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtzgiqkd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3curceknc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhgugqkt.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ulxsdlmx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3tufryrhr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3aeekptil.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ajemnajj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lehyojoh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovdbkarv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zixjatkp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kkuucclr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqkhxjyp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tpmrwyym.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3uotjpltp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dkylafas.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bduqdjgy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3izaeqsuv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cbwjsscj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ydohcqjz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3jiwyqvzf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xasecmtn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pashygdq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3azckbveg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gfgqlzis.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fwvwqfak.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3izqpcoha.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gyicmswd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bpmaonht.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xkulfjob.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yxhirkyc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bfzthhdh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yvenrztx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oupxanly.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vfocghzj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bhgsduez.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hnghxggd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pohixqet.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3myqvdnau.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kvvoceha.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mgxcwoeg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3exywzonl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oifjasxa.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iaexslfz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tlfcrxnx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnupzomy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ucoclubx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ffjubakc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3pixehmjo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3etipywog.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3olejqswg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eskcjeya.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqoddrkh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tyuiiqze.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gsqysdth.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3wjyaefhz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dlnurwuw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gpozsbos.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3utxmvacd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3buvzekwe.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3idakclhy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jabstvxk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3whsvjjmj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eqoidqhx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ybsxspvy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gzquiqfd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qtrjeqxr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xouhuxby.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3bofhisap.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jaaskohg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzurkhhx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jsnojkij.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3agmlqlox.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rqsxbgyl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3iwsbkytv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtxfeftj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3nudsvghe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3corfgnsu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3uxfzryiz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3phblojpb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzuodbtw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3bneucjzb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ylkrqbxg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tnfdzjqw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmalrmee.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3cfrczvdh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3elvqbtrk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rxpfpzqk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3kelfmeqn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3niawhzsx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nujzbxwr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3jbbfucwg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sxegtlxe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3wnfjvqaf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cursiyhm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xiipqaaz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3imjjhvfd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxhgzock.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qceyxzqa.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ranbfbkd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3djsnndig.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3oygpslef.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxwqdykz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3rycfqhrd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pswzsnmd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vhmveivq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lclqexvp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3caxrmppc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzbrsabf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rajjmlat.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vhxtesmc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ozopqkrm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qnhukoak.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zijqykuk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tajuorev.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aypdyysm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wspafgib.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wzdzuxfe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zqkwdjwu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qofsrxxp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3xjpqoljo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3gznpjmpk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vtnpuqiq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bfbiebne.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3liqxabaz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3onfufmpc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3tlcefwwh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3lekdtebe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3kuwzwuem.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kqskqbid.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uwqciduo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3riayjbow.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3finzikaa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3pnenzyla.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rncefaby.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3nabhuvil.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3byoiamxa.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3jqjyabtz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pcasnfjt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ayecoskw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3fscedzeu.html


<!-- 参考信息 -->