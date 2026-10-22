代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xjbjbxpv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xigykuqn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hnqclkdj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gtvpodvx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2twqtgekv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2vhgigura.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ofcovsvv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ixgompms.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ubwogtiz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2frzkuicu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ocjxysgt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pdcbhveb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ifhzhekk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2gsmswgvo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eofspmcu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2guttxodb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2zyzylxho.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sdwxkyhh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gertesnu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2awqvkiel.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oepyxdrg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kortfcxe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dgnmktky.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kardxmqg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pnrbuewv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jrtrzvxn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dlnesmqp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2okahkahz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qcwrdxxs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qnbymirq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2fpipmbvp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2esnjngca.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ocjgbaik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emyurhpc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ujrkflep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klmywrdj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xsnohddi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kjkvxfam.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nipjznsn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xnkbiimy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bzxobosh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gbndbxoa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zgplcnyb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzuezmza.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ollsqjpl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2fxkbrhke.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2uoejpfrr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsguvgbu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2prafklll.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnomnvlm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cwfqdssb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ighyboje.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2mmwdxlpq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yycxsodx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2oglqgsyu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2tacucpuu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kljkdqmm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kubsdytv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2siwxbzwz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rjhjwxja.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2txeumxyw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zfvuibzb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lmahwjym.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2yoansbkv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bkskhqps.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2almylczx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2flpfwpqr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hnpbdpuw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2biggtwcz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qihvwciy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ewkiozst.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xtrlsafq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vkragoql.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ihidajua.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ucalwdty.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2canloulp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppofsjln.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2osvowdyl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2xqdpziwz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lbcbtwko.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qeuvtngz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2nqfyecdv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2svdiigvc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jgtzjsfp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rogzcuky.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pstnmjkt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wrbujhyj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mnvcjact.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lsnoecxr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ofzcjxme.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2oflkcpzl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mesndsbm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2lwklzkvb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2uhylxjig.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zgppbqnj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wrjoepzy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2oimxheex.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2dvulfbkt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2gbfrbelj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2jxctvgie.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pdgaoduh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wsucqgca.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dmwvubot.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2btmoutes.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jbzrulsy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2kdunwgcf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2tbffycgt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bzrkffge.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2yrodsuzw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnbfhpkp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qtaxxvtr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mbvptgca.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ntpmuvnf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qrphdrii.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2pfdvdksq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ihwuqlnl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xvlfzjhp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2supsdake.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zimoihgu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hmaaycww.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcmatyli.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxqcupwv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2gvrrxoiv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cllfapbp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnswdkus.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phzhqzwa.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2slmuagtp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ysveyrqz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zdkotknb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2idzcueql.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gqsksevr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2svqaceyb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ogknqatr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cenxukvt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2mfffogkn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pqfhgirm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xetbmwxv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ltlbdvbw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2rtqwvwlx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gdbvhmxx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nguccwno.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ithkmrdb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2cqjmeoli.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rhauwyuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdxzwvfd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lsccmuax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpvejdmv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2szutsxhy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bkfefziq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2hbcyznni.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2miknfjoy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2uihhhzsn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jikgepxb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2exequcxl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2mpzcroii.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcencure.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hsrvvxdv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jubwpsdo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zgamwmgy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hbkgfkcs.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rjuefisx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gevzojsi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jpcdywix.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ryhhaewl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpwkobgc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2yzslngxm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ubvnjpiz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hkwiuqjc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yoopvyha.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rxdnetil.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2bezkacwj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2pgvlvriq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2puviybcd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2thnxqngq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xhgltqng.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pngwpolh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pilpaabm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lmliqaqn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwgfzrgr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2grmvuqfy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wwdrhkkv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jtrjtdfj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ebhofxyt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2eexvicjh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kcnwwoyy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2juvcursk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2begzksyx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ubfkeqll.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2irsakaxn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2tjxkndod.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gwzbjlkl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gefrbcns.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2aaogwskn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gzzbqclx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2thjlibtj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ccdjplgf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rplbrjfa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yghqonbz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ddqrqggx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2hniownxi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2bsroonrl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fkzmhlls.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2mrmwncig.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lyskglxu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2urbyyexn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2juckwmzs.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2emzqdgth.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qksdhyby.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2khkuhsst.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2frhuobne.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2dbitjabq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vqelfbll.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wwutvrvc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2cigznkle.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dyaqiwag.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ggcedjzy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2vxcbnatq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2biwchgby.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dijxaqaz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2kazkvndx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2jxnitbyv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2sreovgim.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lxaflvhl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2iwnpmjbw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nanjqabc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fjnengos.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ntcrswdk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2roldrodz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ugldcziu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hoatjeeg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zaddfzvl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2eswmrxzr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2edgkzgby.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vanapatv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vvmkynqx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ebpsayoc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2annuwplv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qyippibz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rqsrouhq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iughgbmt.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2abdwyjqc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2grhadhxs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvzwcupx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uanwzwgl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2lpugbusg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjccgqjg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lrexzzse.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cjkohucz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpwpefez.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjgvyyno.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2maposlkz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yvxqkewv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pujfrqiu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xfbvwtyr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bsombzzc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rwrnegai.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2slfamzkm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2acijeenn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oekgcmix.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jovvcghv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rheizafe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2suuuyggq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gtawsdjw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2fgqdwxlh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fkraqjue.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ctuuqtsk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kynjescn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ytrhqysl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2gmxhdfvm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jbccvois.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2lyaulrtk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lsnsxpew.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2rnvvhdqe.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ifkbgpmj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2jmkwyygp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mimfyciw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2owrpygyo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2chnyxucq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2hdywyjtz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2saxojbkk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hynyjwvm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pqjvugik.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2skdcqmhd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2jbcuarjs.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pvjzixev.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wpzdaqlv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nuhzvhks.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2fjmqdokh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2saabgiul.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2bpqxieou.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zdzbbmoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ducbcmup.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2eemyvhil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wyijvycp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2sjojkavf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2shfvqzti.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2rroybaft.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ecvznvvr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dprhamqr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2efqaghpm.html


<!-- 参考信息 -->