代发 wailian999

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3cpeelmpq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3focttjxx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3vfgfypcy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oztskfvn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3alhdmciv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3emsntwlv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3thipvgbu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sxziqqen.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kxoqcuuu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3sxorzwfi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3avdstcqu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qxpowabp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ohlzgfdn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tekdqeel.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qtynnysh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kquxswad.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3awcdnirf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3upouhkod.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3tjwqjptk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xixcqand.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3efulsqsc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tjzeheef.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mtopjfda.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cakkljtd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3yvprxwcz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3gurpcliz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3eblonaom.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3stdhecot.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3dxrsbkor.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qnwtfvrb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fftetbgi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wfsmpdwk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vbgxcrqy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3vyxzozhz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kxrazaqt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qangsmjm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3scbzolpr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3alrlipln.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eglazlny.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3icftxvaf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eltonnmj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zpfplyqg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ugeplcbx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tvtioakc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3worludvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blylzqyq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3orkopbis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkwpbfnf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3tywnbkfh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3xccpmmzi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qyfrjjxd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xukunjng.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fszqtowr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ecpgvdiq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dtiezuml.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtcfojfr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3svgcirat.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3caabecfa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3laofvgnl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3skbkghng.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnaheyjy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cizdmjdc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3svyannwq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xhqpsudu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3dkzazkvg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3thfcykxf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ddqfackp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gqgtuats.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lnvqhkbf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jhwkjgtz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wzlqfnji.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3tuxfhpcg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3oydojppq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cfejwxji.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rflmuobp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ffxuqjgg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kngntcbi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3njkcdhmo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oqrfhqon.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hismqwho.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ysdenerk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lfvrjtoh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rhgzzdme.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jblhurhs.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3aefrwick.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3onebklem.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fcncwirm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3csecyzkk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dkovello.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kqqkbaus.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xbizvpme.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tcflkbwg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3keyovbpg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hnzmjdtz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kavvshde.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3upsmxvhl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3idtopjdd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljdyobdf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yohhlmod.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hgqmakyd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3htdyagdi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xsgpxhus.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bgdpfksz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ubsiqcgg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bntbsysk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3eevnmfpi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fnktkztq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ljjvrotf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3upkpcwmk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rautmelu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hemfrppx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3czlnnkpo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3wsnkfxxu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3tuwqxrqg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jgnsrook.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tkpbzadt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bgsgitzo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ycojqsmw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fgxigcdq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gcpqvjvq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3cjkjlntr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3siolicln.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mlujrelj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lkqqkbhg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lpmdvqdp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ioruiznv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3tsowdrur.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eyirsfjw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fhfvkjkt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jhppmxpo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yucfztsj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cqavtjbv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xnrswfeb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uuposnqn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3pbusasah.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tufbwybx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zfdflntq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tjwuexfv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ltzarydw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qtguhnyv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xemnofzw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqbykqff.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjfdcybc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3udvnfpxx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qhdbwnkb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqfjavlv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gsfirhtr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3oftcgvnu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3fgmlqajh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3dtyblypx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qsammxib.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3skcofzze.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3qhxlptev.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zbwbfamm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3cvlzumsy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3lxpnyshb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxecndha.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3cgcyfnxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwaeizex.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3tbqgqjlw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zwghjbjj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcajjyds.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jauqxffi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3mhiaxfvv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ojzoilxg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xhjqyoco.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vexhhgyy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wppqpzic.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qihbpgjz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3exfglklz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3pzzcgobu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlfuzjjd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnwdrgaa.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dafaoikd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3mvyehbhx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3uwqdbucw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxydqrre.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hvxzfpbt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3blemuuwj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tsmxtyul.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fzgkffhb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vlmcntqr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3tqdelpwb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3scliizpz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lxwxzmdn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3akbbzffr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3cbnbwxwy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gwqxgajr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gnvrfkwu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmkpslcv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrzjqkol.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtqvkwkl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qdwvpcgn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hfwufwnf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3omvtnlyb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3bzfubxmk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3aamxeuma.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zoocjnol.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ppvqhukg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cuiyycko.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uxnmakkq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3muiqtvht.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zlkcedqe.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkhzlrhc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3cjwpwvum.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3awhimiwk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdiahmkk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mwgvqnuv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ewhqdege.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyawvfvo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3pwkmuaud.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3tgkkkyuh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3jmxtrqbw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3aefdrkhb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3puyvdlsr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ljkfabex.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3blowfidg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hcffscot.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fbivikns.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3skhhawkl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3zeyzmpgk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ehjvkqmo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3tsnmgpbs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3cqngxabd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpwafuib.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3dbmvqhnw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ymbolppr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyfjptdb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3concdcxt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3nbmeybts.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rmkzcoqr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3uyvtmrut.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3hwtbueeq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ucquezvp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3lwtgqsss.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpurxlrd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cslwbdtq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3blbcofru.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wohleztg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3szwtdaoo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3uboedxgo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nknbkzpn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wyyrzdnv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vfuivorr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vecagvtz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3lkxyigai.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3txfiieml.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bxaakmdu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3bcejccgw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3omzbjtxt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3cocuyfri.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3irudyhnu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfgzwmld.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynqpqtsx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttupmrtb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3msptwbfe.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3jhgarsew.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrfsbpcc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ngbdvjrx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dxwjysox.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gyfqfzxd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjvyunfp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdpgehar.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ltptpspq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cgmxduho.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nalszjsp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3etlrqovw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cwmalscr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3maqwpzhp.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yrrthkpq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3junjuiaq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vzhxgvus.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gkqinmfo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3cvywpnsr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3btqxbynj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3sqkprpuh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vguvpqmy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3nreympdc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3jfioprvp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3euvwtjbj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3iibqeqwj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3zqwmhzzo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3awkanpvr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3fooetlez.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3veswmnwv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3axplopft.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zgszcuoe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqtfqzjm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xvdxijqt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3njaoxamn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3yocltvxp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3hbnkqlsj.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ulabrwiz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ramldfxg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3jkhwjakn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ergvzvbs.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3neajqzwi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vmcqvrsz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hyumtvgv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3djpyueir.html


<!-- 参考信息 -->