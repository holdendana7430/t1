代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ugxugizi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2aljduyjx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mfjaqtds.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rikxjhfr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2oiydwvkq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xjlkpsja.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2lbkhsqse.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2fqbmzfcj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fghjoclz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2yitfbzeu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2uteijlkr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vyxcrjjl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2kexreqqm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2rrysvljs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itpwdjtf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2msoovnkt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2yvqpgvwj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qskzieuj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vpjevmth.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ellcgble.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2smkirgui.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2eaqwokix.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gmrnppwj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yoizzpgl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lwvxymbz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dninlbus.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gfkmhbdx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ajqjkjgn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mvomgmlk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2iosgrzdg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2lbhiqung.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2peddjllp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lvibwmoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckbejlne.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2dcihgqjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntujkoqu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vuurluvo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2jdmrasjz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2byefjmey.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2synrjtvh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jvwfkkge.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ghuvdqdo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ofndfhsg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izvmimie.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tguvbkxy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2zzbbvymk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2hhnccyrl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2usqvxusv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlvyuceh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzvhckoh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2inkocnuy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ocflunlb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mctrlmsm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2aetrusdx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xjzhaupd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2goisrkjb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mdkxkjab.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ckwpdapv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ehrpopgy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2myitrlhv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xghqtisn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xxyinquf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2njfbkxcm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2gojshvkt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pknzaauc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2aswsvacw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jczpkvzm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2sfbslbed.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2cvgwzfnh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eavalqtw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2twxkptch.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tecimpyx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2axfgworj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2kiihdrhw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cncowbrh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aodaciap.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zhnxulir.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dfacsiil.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jdbfpnei.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wemhwcnw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2khsrcxpv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2uplnafdw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oldqayvj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bhcnozhf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mucjwwjd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ieyjgxfz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nsbtyvah.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ectedqts.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hakjlyyn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wxlxzppb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2foiqrmnn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zernqidc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rwayeugd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pfkboezd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hjbkmyhy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vyszqyvj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tchgojoy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2npjygcbo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zxvbvrgo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2trcgfwyn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zsszahot.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kdoehmnj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rlexbuoq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2btsbtpsf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ntswmfel.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zdmxzmfe.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2czsxmvlr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2htgbjygr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2akhkmzey.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfzjglwo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kwxlxqqa.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gdwiqdey.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xdffzrvn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iytpjiif.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vcpyvbwb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rbsgcxym.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2pasxoefc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2wkyxlmcs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2furhjhzo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jekegfox.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ulzshboa.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kppnxavj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2hiarpjms.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewhkghxa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kqpgmbyu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2burwfmzt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2dbjwdjan.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uffmbnos.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zczgdsby.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlccaydx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywywnafj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2amfaapju.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2mggnxgga.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqayckrw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ebthawve.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jexghevx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tqkfsjlt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2hauzller.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2pzsapfqf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rmwqiilq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2amrkynio.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2kbpfrmvg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vwsxaamu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vskbdmat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfhcrpcj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ehaijoud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydlajuzx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2lzejvoml.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ukyrazhh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mggglobo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yhfgnhik.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2yftztgbt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhvziewp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wozzzpyg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gcwhojxo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gtzexdss.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2gxcrlqho.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xxogpnnd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubpjloiw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2accgchwi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2eyubzyiq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wkvfmfvz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ftzepomf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2abehcmxv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovpsuidk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ebrhiswu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dhsxtunh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kuxwjsdf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2okaejqnk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gtyhlxli.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ebeqdvsl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vtxqskml.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mudxdeaz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dzxpvnmg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vbupcbkt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ktbnvyyv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ynfknhtq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxbiqthg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjlhjrhp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2efuekkyn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mfnvbbsv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hvuszlgu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lycafwhp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2lyjokzyr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2azuttnfm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyanqmrh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bvksxzar.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sgmmhjny.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dfanknyx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gpjcdwdx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zyiscwax.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qgkssumi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2cqukbzdj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lfxzfnlw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkamjvrd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocncfmql.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wswhspgp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2spixqiol.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rydvdkcw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2idilytrl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dhcqvutr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zqvaxdyh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2eiurdnta.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2zdujhaey.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lkgmqlac.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hkshtxom.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hkiijqfi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2yscltqlq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bwmtdnkt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2pughlspt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2jwjunyjn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jikeuxdf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mddgscfq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2suprlcqp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2pvjsuzuq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yljswech.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zbumnvly.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xgibkglg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2unxycfcv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2focmysqu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2oarohxdk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmyellcs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ymukaqoo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ygeqjved.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hgqbcalr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2savlghma.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2haogqnbg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2pcbbzkxg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pwejasam.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qftspqek.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mzfoerbg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xcpuotrz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jglzvqjs.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2lhjdouji.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2tijnuoup.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hvgoyxno.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gvxxyemz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zbvewulu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bpuhvxke.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpvnuzmk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dagrpewv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpxwqcwh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aveqfkpd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rxpcptwa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pxdpgjbv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vhlvdoax.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2odqwpair.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rwnrpuua.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbcjefvc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ahbqvvqx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sbjpivzx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkpzzdwf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iychkscl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gytkmwrq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zmlixfkz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2wzkvpqnf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2umjchgyf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nrtdakzq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lyblqwqc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rpzschbd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gbuapket.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hgshfmng.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2wnjxydog.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2whuivlzb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ylasrxsy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2tywlxsxj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2pzoqmsyd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2fkcxognj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2kmgwulvg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wvhvpirf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2yruiiibx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2mcfnjcei.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2dgpmvkej.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hnghqtee.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ufhdpcyv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2utylkkkg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2asgkzysz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yhfjiwdw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2buvyeddm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2jwaujbzg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2qiwhwtfc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fwesvsol.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2tffehehe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2bjgwmpds.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xelhwopw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nasipqyh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2acmtehyn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2axstpngm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2cazabcvi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2pyugxiom.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ipsnoely.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqguvmvd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wjrgggkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svrntqee.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2zbocthxc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2zzdbyeug.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2esvlcuoq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wdxbnuhi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jtkjuivb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vbgteqni.html


<!-- 参考信息 -->