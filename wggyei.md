代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2mnglyjkq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yagykjmd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hdamyhsx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2enlaiylo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xfnrmejm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gyjrphdw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cfaomnjh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2nreqsinm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rowhhnnq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xstppoke.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2plvaymnj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xnotcgzs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wsveechx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2doklanqz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2dnvkqukh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhwgbttq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwadhkzk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2pekgghuj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gglolori.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2piplirpy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2tksnjkqt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tjwoyvbr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vvvrtxzx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2scyojzhm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uluveoze.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2dkbofafx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ojghrgci.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ntmymnvp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pouvihrw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2fdkkebjg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2biwicriz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kwswvuym.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dsghudbw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nzgnxmdh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2lknhmoal.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fuwafviu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cozehcbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oamabugv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rrjowdyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2loxmlxbi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nunyjnkf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nfepmleb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gdyovgxx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mexamwlj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dxngqhet.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tptudrww.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ecovjovi.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhzixrqg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lvcccvzr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ohulzjuh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fkzerrzm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnpdxakn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkxetcer.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mmzdpjmr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ymufccde.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ryimgoam.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2yexczuie.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qxikouuu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2cvkafmki.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2gsptanfj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gohdyojs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zhlhhbyl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xjovoogc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2uuenhwii.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bbwbfoot.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dewpzrlk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kvuslpol.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2iemcidso.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hgfovwqf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2exumqpzf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xcksdgfw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2brrxbyvx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2pzstpesy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2straiaud.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2azxlakzu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vhohdtzv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2hbzicylr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2kpmfbdbj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2alaacfko.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2deeelurc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xaprsltg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mpsbtklr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rovkzzyq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2anfhfsur.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cmtqwvev.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2seszrebp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzggmqmd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pdmatkdw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2braerqvh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qvicfsog.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mgjbqrhj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvyhtldh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlqcchbi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jbaxmmtp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ymgvwabz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wvryqsfa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hvfgvtai.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mkbaxkrh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jtbpthjx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wqaazebj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2dtqagarw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ozhcayup.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rnmwrwsm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lllxrhsn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ztzfssrb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipfiycsu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2riwbxzuj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zkijwrkh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ocpgjarj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qeithdqd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2kpwhwlpt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xwnhklkd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hwhhncac.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zntffcww.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ozthzuyn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vlozmymn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bjxuzljz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vliahvxp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2yjaetzax.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iwwsvbdp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zjpbajjl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ilcvwcnr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxkpatdp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mgxfvyzt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hammkylh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iovemykv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ezjawifz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xbeokwua.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zulefmka.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hoajporm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lrevooed.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oofqennj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2dbmpscww.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2avfcfngw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2svngvluw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2glfkrhrf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kgulidmc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2njgvuhdt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kcudywdw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2itbrpaop.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2opbmhyeh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zogmuagk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2vdnqedpy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rghdrrvt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2pqgjxpua.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2byeouwyu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2kottlbqn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2eigzrszs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dnvvkgpd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qrvoosjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgjrtyfq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zulqxaqp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rxrfjzdu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddqhlsyq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2voefutgw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwixvyid.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkqxstog.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ptgalvwh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2aaguiylm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uyygvcjl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2lcjvdtwj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2yckevxmm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pvhurvlq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fkdhgruw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qomzyapy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypkahwqt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2mfqjosoy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2juxdpmlf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhywvgqj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rlazvbol.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ckhtriqt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dpicdwvg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2firddyeu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2uwejlkzq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2knqqwfln.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vmgrvtjs.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mgswpucu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2strfcyyt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2onismrgt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2iadrsdva.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsyawgvk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pufogalr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mirywufj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eschsnbe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cknerdbt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gexnesoh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2haqphccw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2czpgggzx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rrfjnvkx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2unvzhacc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iehepmvo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpvgffik.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2eomsfllv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2xkcttuph.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pdzjsuen.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyxloxcn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vhoxpphc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dialweuu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lrewveyg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnwjlznn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tjxwoqcb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmykrqco.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ncotuauh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ywcezavy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2myqcnnru.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bwbdonwh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jeivtlat.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2exmkzuln.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qhyddihx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2exfjzqse.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rqrzbnov.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ioakbfot.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2rofbfojj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2cxtlenil.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2yuxassxu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2kuulecve.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pbohcdyr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgpptitq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydtjvdgw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vcgsruze.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2okuiclbx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2etndrcye.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2zqltxufo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mbjwkkld.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2sergchxv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ibdoqtsw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lzxsuccv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvhpfncy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2afjimndn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2sjotypem.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jdhowqfj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tjuqsmam.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2cuvbkpql.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2koqvxhvc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qvdfwptj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ymahdzgm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2masuxior.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2dujgcmar.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2fryurnnp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ortaywko.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zuptevbq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2sufbrghk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nrnnuefk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wnonfbim.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ijlysfvo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2yrqoxtyo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gzuhqurf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tfpoacro.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2mzagibca.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2eaekaoqj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cjwqqhrt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ltorgxdp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfqpayte.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdbrictj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qlcbnvic.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlrighma.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tcftttbl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aoxdugwb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wrpireny.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2anzowaby.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2mfzlrpue.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zpcyqtej.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2phildkdb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pisiurot.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ssvcponb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ysfmhwug.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2btvgcwbs.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ovjzshcz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jcwdhmyc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pwqndmss.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2obmpmgtb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2sgerhszl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2emvaqmsh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfnfbbpf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2texynmik.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vpwgkajo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rmlvdgkd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2latvrqsp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ijzxvcgi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2dykeuqea.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2atoawhip.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2drewsanq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2suqnkawf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ggnsqtpn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2vkwptqkd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aemxewps.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2pmtqnbvw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hzbpwddu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2jealbnts.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xbrfxluj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xndyuunj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2yxlxckhl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2vvtvhbwb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2owgcfsgi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ewnqrryh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aaxscnxm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ilitrlbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrdsgmkz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qpoeqzsz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2skyvhfur.html


<!-- 参考信息 -->