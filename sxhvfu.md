代发 wailian999

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3uwiyzwuq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tgxffolc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3bgkfqtem.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wfdimfvg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vmkynvdq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zkfvfyyj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qvtcgqiw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lckpvvyk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3khfbckdb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3nfawsegu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3htebvsjt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3facafeho.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hjyuinpp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tzxiwvnt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jfxoqedm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3lijwkffv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ozcpmjkk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gdfenrjd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3okuvdkzq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fwzlqizn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3eovolpfb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyzyqcvc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3vmmqtbyq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ieulbchh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmwgcnna.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kcjydtte.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfncabpt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3gslxvfsz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3xqnorhcg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jlhvucpb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yeaxxvix.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yercswtk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uwnuzysc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ujzltqqo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tkbphcrj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hchcnobh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ucyyhdzi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yabarhfx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zjeerllf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bmgakwhs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oghwgntv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cjvuaqfc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3fkyunomy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yqbjqdgu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3iejgrudu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntzitbed.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3skjtlykn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yggxiehb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fggrqzlb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hivlmgyv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yfdrwkxe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mnnizhys.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3chwermip.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ffnoduhz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3mzjfowip.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ywevilbo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xdbqzizp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ecixxntv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3zbktoojx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlbvplyj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mohsqdca.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwvbzkvf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cgkhntxn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3yrxkkpjz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ksuviqsy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3mhzrvcvg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3blfybwmf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3estyggrr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cnykwaod.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rpbqnijm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3asrbmltc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3oknercqt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3kwgnfhia.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3eanwewbd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zusjsbjd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3inihpsxn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hvsamfka.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zvqpqeaq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qwxnreko.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uvihhxmv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3aakedymu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3venqafbg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3szksgtpn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3knhzecit.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rbnurznu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fgjnqilp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3weuaunws.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nszxljys.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dghvwueu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dpjzozzd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dkhdscxi.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3awlomxzg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfzecdqk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3henmoyiu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3claehhos.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gasqhczg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gznykugp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgpfscyt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3stbdzpzr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ejydcijc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3inkukgzv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iwosfavy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3eborzxko.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3aqdmfqec.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3yjmzmnzd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dbecuype.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kayfzwge.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3iwniuxpw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dzrazbde.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3kzvabgid.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ptwqwgvr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ihxsqqnv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3twkzmmck.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwgsoxou.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uclessap.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ynqrzonk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3sqxdfwuo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3msinwaov.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bdfgcrnq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wvboyvqj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3hhklfxqx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bvuxmzbz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aumuqmyi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tqihothx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vijedoyx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3frqcgwck.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ejrvvqlh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jenmebyb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3eikmzhhw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3hitbpcjj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpnysunm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3huscnfsm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3scbbgzkr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3evjawcgh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3xoqsympx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjdpplxs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eyakaxva.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3texhwrxe.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3fisbcsgm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vtoydyvc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3wnijwfth.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svvubbde.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yavendwj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ccpjcfdz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3uugybwir.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ufuxazfk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3cfxmvvvl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3cyeevqds.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qjyztktd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3sgbsbwkr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3gsjsucbc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xmsrtvew.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3eojqlsfe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3eceadkwp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3oqlcgzym.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zkullkel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhwpccda.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3iujcquve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3suafafcs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xlepmdvd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3pgbndivn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3nygzrjcc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ykozfvng.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lpurvshb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijdtwarf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3sscabkly.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dhozosdz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrijfvym.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3uymuvesf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ibjepupl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3bxpolaky.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mwzkmqwf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abcqyhjc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hpkrveqf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nttlajzc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3itdollgd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3muwzvzoq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3huzexncc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3utcgdzth.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vvozbqku.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hrzzvyxe.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fatctoqq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3iueaqqhz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3gvxwpzwf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xjlzvcav.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3rnioqhrc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3qbekuaan.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mjvsmbxm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3urdfbmnc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hgqotvie.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwhsypbj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uhsfilub.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ihrtazez.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cccnmsra.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wlunemjm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3exqkfsdj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qmkxibwo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3smqncmmm.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sjlwrybq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vmtndbef.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pbskjpez.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3rauddpfs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3qmqwoaop.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3uyytlxfo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3uphueppn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3wjoqkaol.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxcmblqe.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bhkcxvcq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3olbgmdky.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqgqskmo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vnkegvji.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rpwedsbx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3vqhnxyfz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3pcbcwztt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bhxuowwi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ishleghf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iahunvil.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bdcjeqmm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mzdpoqzt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3wbwsaigy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ywagdyqp.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ebjtwrxu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3eunnxvrr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3tzvkuthk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjxywmky.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypufzmdd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zaqtcelf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcgkozmu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3suocobed.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wuxwinpm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ashhyhwh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3xpemdbgq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dajtwioh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3cdfcmdny.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3felhlfrp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3mebyswuv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgwzgoim.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rshxemrf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3wzalspqc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3awhnlhdp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3pqvhyhgi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ohzvlpwi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ihxbjdub.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3suyilvgr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pordtcfk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ygwdedsx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3skcmrzug.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nscqblxe.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xlokjzdz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3wyvqsbac.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rfuxlzoq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ouhhykuh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hsttkwht.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3thlwphop.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3plvdqaqg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zmhrmavz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3nvwxgygx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3znzaugqd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cirskfmu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3varyjlrk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytxlyrtc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkmujmrl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjgwdsci.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3exysnqxq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bfsxuwll.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bbsqjeqx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oesogzxl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3kckejasb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3jkcmpfdj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hwithtgb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bjksqizf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zsipxend.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3oafqkjpn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dnhnifvv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3lpoiqggb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ycxarfpc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3idhdumbp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3coxopfqg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3adznnrme.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3hnnrzywi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3wcckpyui.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibzfxmjp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jgpeqtsp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3pasdwwjx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3qxhbbwrk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3rxswtttk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3fmcpncpr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3vzdvoykk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fjecxrqd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uyaxxjny.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3xvkbfkwd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3iplrcvbu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lovdgyns.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jrjgwlmi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3huftypri.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3oauvadfb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3mvcxjtin.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3guyjhqqg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ushjqurd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3cnfbmrsi.html


<!-- 参考信息 -->