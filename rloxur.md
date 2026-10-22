代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ipzxpazs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbkqfoej.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rihffjeg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gcbdsett.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2iwfojkqw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2umcgakul.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2wzhkjzft.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kwwdiypu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2woaytfcr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yfejwrcr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xywabcbe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2apsqagpc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rzyngvzk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2cisthrns.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ykomhgzg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wkyrstsy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lvlenkox.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tgwvyogn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2onsptovr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pbtfnubg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2moqctizx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gdtwlaom.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2alijxiqf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tjybiaag.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qsgevlkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aiydmoys.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2lwaalvle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vbkokfcf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2riooifgo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2cdbxlesh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hcjtcjqj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2kyyhiqvl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qjrocxjy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hshnonqj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2apcofhma.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2grnpwkbv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2stoilvcv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2omneakaz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2nmtpjxds.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dypsfmyl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2apnlwwmw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptyyzyad.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nczgjtpb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hpvzzbbz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2emgkmadf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2zxcoktqk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2cnpkxptc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2algrfulz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ttjaqjhb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ibmnsxep.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fmrdiifq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zqrrysil.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ghlgjkoy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dzachunl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wjfbrrxc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2guabweaz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zctcwqjb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2mefxudgh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eytuvalo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mhfgcxko.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hxvdcxcq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wqkinwmy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2pkcamkzj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ykhtoqbh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ybmnhuji.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2unhhomxg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mgzusxas.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wfuminyc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ryswiwon.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yswggdza.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2encwgied.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjtoeiph.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nkxjcguo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2yttfpack.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xncuvhrl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2duwbbnnx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lcffjdsr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xhpdauug.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dekluuwf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wkcuywcs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ptikkell.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2olhqedgj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2qkzryfnk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2imikrrjd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pgbqgqqs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mfrvdwam.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ceiylaay.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2fwjjpwqn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2nbjyjrlz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ihljvrbc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2plwmtfcm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zfkhkphw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2iebzhiyo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvamfdjl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bdoytqco.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uwcfzhym.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ydhuavzl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xgsarvhu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2tvumgcpd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xyzkcgte.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2phpfzjyq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxvewlmo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qywjrjxc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gawlxnox.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2aypizmhj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2aychsyrr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2egkdskft.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2socinxkh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2nafywidu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2nkhnusak.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmoawbjv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kirzdxjm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dviyisze.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwxkadav.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2yomydhgx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgezjvuy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xynmpmhm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hvfoatrv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mefaltzk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aoemngsz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wsbagnxb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2biskytqo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjwkldiu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zmuncbxk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zbbmleit.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nuqsdzal.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wvaikhrr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nvbhrsce.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2bfuyepdc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2bxfrbwxp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fqgeuslq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tfhiacas.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2tovjscft.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jkvyfbjj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ltdakljv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hyvfcepl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzsxortr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kvpnxcfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akzqfkjw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xxpruziu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hdnhimdq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbrrjiai.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wvgwgsxh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2maeugdwg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmnuidji.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mrglhkou.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mbdpsjgx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkafruzq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sweskina.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2omwaxxgx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2fslduisc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2trdqphbh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2otyqzhyf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2atbohzfu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2saanyjla.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2caqkijab.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aalqydru.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2opnepxqj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kfhlkaxp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2chbejwaa.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jlykzljp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lvngytea.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2stcfmqia.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2aonkpcir.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dnypxyuy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2uikytviy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2fvqbqufe.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ogwhokoq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wurysibk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nblkwepd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbpgakuw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tahhrjiu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sajvcqxo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kvyvxquc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tyxbzvij.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2frryipoi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2zagdnaxk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgchsrhk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wzyxvtmt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkonpbgg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kbjufesa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2phquncaa.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wgztzfmm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2njwftqcr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wrfelxvw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2okyqnswb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rhlvnygs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2thnxfiot.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibvpdguq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fobznotq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qdopzuhd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2lceswtpi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2dobqdvzv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2nprhxpxd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2bctwyirc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2uwfnebyx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vlnfvzwl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wohviezw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dlgorsmk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ftiafrdj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wxwtcnzy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ysyjotbq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2czywknnz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mcgoimhs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2echeduhd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfwbmhzw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2wqngklwd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vihcsgdz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hzvhzsbh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rumwajhn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ockrddaf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jnivusgm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hcnikjew.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmbbtprn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2icsmlyup.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2njsfrhrx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2fniwkkku.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2nvygbvpk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rbfuqiry.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cojfozuy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2sonnjktt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2etacyops.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yhwmlezn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2tjughxqw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2iyzzvlwk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ptrcdszu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2iuduevxn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zcbkxety.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2lgthwxsw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2sonjlxtd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mqnvhtak.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cpltwyyf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmqmlczc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rjjzjglk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bloqtixv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qjrbxbdj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2damdeoda.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2okvaswsu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2litqzxew.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zpxoscop.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yvvudbtu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqvborso.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tquqcqdf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kglarlac.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bixeszcu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2azineshm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xuxdlgyt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jmhafuxu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2eelggjym.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tiibkttb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bjznmmcg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sztwgmff.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2svhofnqm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2cxglehxc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fhphfjyl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2zsmmkeec.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2mkfyiptj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2matbdpep.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2wuqeccjn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ykxuxcwy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2tgmkhwpc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tetedzcc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2xhajotzq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ttaltkrp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qysytruc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2glngxmpx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2hlljyryy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2fxkfotoq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2molgljqr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2iyyhkdgi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2cfkakgfl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2onwggoki.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2icwswpsd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zjhqxiyr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2nwtnxikb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qidbmaus.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mxmmvcmn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2weejnsup.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mwyhetae.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ucndwqbp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2okhxxgtp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ncfcpvvk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mfabbahy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwyebnyb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nkaoexmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cavoidaq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tphusorg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cbgmcpep.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ecgfkgiz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2thelhqtl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kualijnj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncwcwxwg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ykikilmo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ywkzgygx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzvkipic.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2lfwaiwrs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ahhdpobc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbhbqueb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dtovkbck.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qaqznook.html


<!-- 参考信息 -->