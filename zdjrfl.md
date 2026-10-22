代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2hdyjtzhm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cfkfrrcg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jqucbmvl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2phszwyua.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kkdgylnc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ucbywpod.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2cebynucb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2tzdxsmyr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bfgbxspg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ulussoxj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2diqzbdux.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xrjeseuw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2bmuikmij.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2djirluxo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2zzmgzref.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xmtwebtp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2khyzpfar.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2mdemgjpb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2lzpvibvi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fztarzhw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2quctpaod.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jahykiwt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xsahxdhg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xomefzol.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2joxaoywr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2lhixauzj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lbksssdu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zplotnhw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2syvuctxa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfsndiiq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rbbjtykh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fvvwhrcj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tgpvleyd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lpcjynbk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2omxhszgq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pymchobr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2whwvepnj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eihkpunl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2kqvjcohq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkgnaavc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2psgbvyjx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2eqixjpku.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mulpvvca.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ywxhgmgs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2oplyysrt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fpjwlayn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wrkgitwd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dwzhbgrw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zindjitt.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2dcdzjudv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ddjnamvn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ijvbukms.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bgxznoxp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gewpijvw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ivahvioy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mmpgmojl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2exumcfma.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybiicjfv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2phwbavme.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2oycrcdia.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nhjkpowt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2owapxitm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lfhgxvst.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gsxdxgzp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ljzxzavn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ugfgroll.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sbmuoabo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ikvrbdct.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kizrpmro.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cftualdx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lojounyt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ibrqyemd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2prfduhgv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ldcidqxi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ltyanmwm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zuwhkimd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2umbakyli.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ujijdrmv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ibzqqhsl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2suopjufs.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ayckqnwc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fuuxozws.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2dqhkkiya.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxnjzuaa.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ufrtxplj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wphbdqcz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ygcmldsj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ashwrjzt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xooqecce.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjtpfonq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2odvsazhs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzybaxnf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rziorong.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uggwvfgs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cvmiuuzl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gauunodu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2byekaetr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yevzvygs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ldudxtbt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kasivelw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ntaycmbp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2fbzmigqf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bpuhyccf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2qwdcnekn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zpwehept.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ybahjvry.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ynepjtjf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tvaueven.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2oqojkvkl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2luueikkl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2wdkucibh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ehmvffnv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2dfdjpvpa.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2akrbzmqt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bdzhbevu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lsfnbwsz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2iwpskady.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2slzqgrxp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ovnjttsb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ryqjnwxw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2dmzguxgb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mzuhaknf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dgnvfklp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vzupjorg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2buhsediq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tkxfmyxv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kzartbmk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2crtrbzul.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kghqfxln.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bmbesxuf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qcjhjevz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2maevsfat.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2whrfyihd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zfygmoqw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pmqkmvsa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kbwncmdd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kelrlglc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2enlrlrjx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nteyzfzt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ssiqhlwk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2fvhmziox.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2hpikttsi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2owdrklkf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2njqjihqc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xdvcrsvm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ivbsnqku.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2qngwdiuf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zrsesaas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glnsqdvr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2oanwtltf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jczvsezt.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2mepcypvg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xhseqriw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dgxuqaql.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjtsdivd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmcfzllg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fiejpyyu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2rxlxjesj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gvoyuciw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttxyyfzq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ialtuerq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2weldhpam.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rfckknct.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2urkgaync.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzfqutaj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ltjtxzhj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pbxvjbdx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2udhftjre.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymmnyvwu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zmzatjjr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wjszxoya.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lsjzmukk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2npixromo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2fvxyvwaw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2farlblqc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2helobcqn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2drtghcjr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oapbtmug.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vapnstpw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2poucelli.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqhmcpak.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooihzgll.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqkmaouc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2meibbdqr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nimarhaz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2znwinvom.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pqnwfwoi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2knmhxmpd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mkqdbpix.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdslwqrz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bzsptgfq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wauygllz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxjypyxu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mgronhtv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bjjqtqcq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tymizyvc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2nnttosar.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tzcakpki.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aqlypsih.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbkblyrc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdpjgelt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uhgcidvn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2psahonkm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dgjzohqy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2qzzzydla.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2sjhjcblr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2mmlkgbdi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lvqpmmvb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vpswszug.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gzeswsbj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qxzxqydi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2sfmdpwem.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xcltmwpy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nezmzkwn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hvniwybw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2pmloudbc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2amwdvmcf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilvggquf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dcjxdnsr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ndvidpsh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2quwjcjjl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rbvcdfbh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kprsbjpu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2vixgspaq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2tulvclbs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mshgutnx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gzpmapru.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzginddk.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2djrvymfw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xklglpym.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2phtlrieq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjcclpqw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pnngkhey.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dlbirpht.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wgwfnjcn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2czgzqaki.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nomhrybi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jrvfkgcs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2gscicbkt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2axaiaxmu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dzhstjcx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2oazqqndr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2sdbxqjka.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyelgetb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wwqvxgtm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooidkhiu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ctflojqx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fltikvxu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2iwucytvg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhskebtw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gorpamaj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zyzucbxs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ljwdcyoi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbtvczii.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbojzmfr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vjifvqpc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yrnllpcd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2spapbxkg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wkzqaifc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2hvxytiys.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ianghamg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eokhzqob.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iutilvjj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nfmxpiia.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2soeozjkx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2qaauunal.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2tnxibzom.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lgsxajsn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2nasshpbi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ltxoqdbc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2cwuqvieh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2sgsvehka.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2agtntazd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2unidpcfd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hceiyerm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2gscsbygc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2nnzfxgir.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qbrwjlds.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jczmcfaq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2liysscwo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2cjxdthiv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yqqtrdjx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2szxvdycu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ztuwpahg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2rucvifpk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ctuhsmwn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xrsdtvvj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ruywzzvf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vfgttyvh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2znefufdk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2egfingci.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2fwdjioee.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zeifomxj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2rtjwnzjm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2yfqxbraq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xefhcnly.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2kbwwrkjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqjozjvx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zwjwaywh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xmbildbh.html


<!-- 参考信息 -->