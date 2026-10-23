代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3yvdkjrhl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abottymd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zjxjmhdt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qakzxjad.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3rylkutcr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ddgrwpwd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvivgfir.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3kpjczoha.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3amaliaqt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hmathckz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jvhtcjdg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ppndzadf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aixutmci.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3saekexzu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vexzljiy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cjxeachu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bynodnpc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqcspikc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ueaaztex.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mhqpeblu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ntwfkupr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gxtqlwgz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xkojvwxf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kathqdtt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3phuossai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbwrnvfe.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3iiirlfun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqzigaed.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lgfzdtco.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3cipgdvmo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dfvnscmh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dtrcbuop.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vusmrynw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3adwhdzjk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3muxyfori.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzojqndr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uzicxfxs.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3uqhkhnyo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ilkusisn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfwfxuct.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oyuafyjn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nffckqah.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uyqqgwvs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nhwyhica.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vlvhocux.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzalmsft.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3jvdpngdx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rrxncxhh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3eopwkagw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3txbsygfu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3efvnyumm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ycxyrrww.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qnlzbgto.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tnakmndu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qakxmdgs.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vkvuprhy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yctokzor.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3miqnfzyz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qfrkzfnm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rmuotxye.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3upwikacq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fpnykslg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ecltaawf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wtrrvxsu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zzdpqsuz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fjgmaqfr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3abpmzowv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhhvdnsf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idyfrons.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nnhlvxxt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wujxbrzh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mmkjhsni.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gofnaxtp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dwqvlysp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3owkrlhar.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ejckpxae.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ufmuoulh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hmuetrjm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3euvefbbq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rrponndq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oopqwbjp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lrlxwvlf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3fnygdiaq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xnfyhchp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3odkjtkzr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pzumnxwf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fzuomvqp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hblaigau.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3fojcgheb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3rhglmxiy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3anxznfya.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3yumjhhpb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3nswvtpkh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xwsmagfh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jynatqff.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wlmwtgxw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dgfiruhi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lvztjrle.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nwkqqfmf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3lqlvkwca.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dgmzhdqz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvuszjtk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zyqxftrh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ooxvbbxt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3phtisynr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yasqzikd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wfvbehhz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajagwube.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3glruvkgu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3juyugdpn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrqjrici.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3giqmmjre.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lairnwft.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fejczzcx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3sidxrjcw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqiyuzmd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xpgruhcs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nyzhnsdt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmadnhfr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ebxehfkd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xghngnme.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwqlvlpq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qujbyjmx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3scouvixt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lbzpgghx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvetyxqn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3unmqkrcy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3kclajfcy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3vcgcwser.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kytddyub.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ptxzvikg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jvscutzj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rjixsrjx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zwibyrlr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dszrlubz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3aoclshwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzbfbcwi.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3loggwyij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zjqvttrj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3cdgvrkha.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3imksxrei.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3etghlpdw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oieazztr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkkyhjdz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3vuypkmcr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fckdyvfq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3locuwxyy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wpqmteus.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lxecgisk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3wfgdhzyj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3lcocrssv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cpkxccmg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tyrgknut.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lbkqspdr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3rslrsbqk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3udmuwgup.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icewzklz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3fbkvuwqw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dpcuekzl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3aojycdbr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vbyrkvnf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3saosmiqn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wqhdqteh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pzyturkm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gxwmfblj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cdmetzby.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3qmrjoyih.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qvcfyhuz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3njkpqgrn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3auntzghw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdqlxutv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wkogqcoj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rvldjweb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oedehgyi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nonzmlzj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rnhbagkq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3brlvckqo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgyqvnni.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrfmcnod.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3keaigoig.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlxaaxri.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3dzeevnhl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qfchbtmt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3humjuyiu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3gakbabec.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ogtipwjg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nfqmfajg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dncdfgke.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wxhayboa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilsxbejw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ffsopchb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tkxcqtqm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3umwwhoqm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3hfxhlsse.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3sqhyuiqb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3eggjeaxm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ziogechp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iwaoaluj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ysngxboa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mlropfnx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3pmmafxsq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gfkmmyvx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3yzqtkfow.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3oisqzcwf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3rfnpnjju.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3lthskhab.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxwfuzij.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsndmrgz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mcebcyin.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3xgrpzsrt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hkckzcst.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3vhvulknc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ogmbkwwc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3lkpurxlp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vnzpenff.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3atndgnoo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3sqxnexjx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3srhhkedh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rxugcpsh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dadtctcq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3npmvmqcp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3pislsuaz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bioxvdoh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xwrmozkp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dzwtpjwz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3bgqkojvz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zcrgyffq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yysctoye.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3uponksze.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3idzeeszj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rhabqcan.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vrctelio.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xexfrhuy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3epqndjqb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3urmtnfck.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gtlbwjgk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mupeocja.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qpxuhtcr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iuxdvltx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qffujwre.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgpvvpgy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rqcuegsf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uoelwpiy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tolrnzdv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ljzoiulo.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gmcywzdu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3stxudyfe.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nqlpkzst.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3saslpazh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rgxicxop.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zbplgdak.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jhuivktu.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qmqquenw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3iraeugtf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wfzbwdyu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3krpfltfx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3mxzojxxw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3snawyllk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ghewzjgy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qbyfvlhi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rljgqkjs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gitzgaxe.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3eglpodit.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3hmmxqehq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ozvyksyg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wodazfqc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vgrhgekz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3lfqiuost.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3iaqahbsq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3idvsbcpa.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ngwppcxf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3fsfdzaet.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3mdulgrdt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dtiqqdxw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ngyyjrdr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wltyplhz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3kswioguo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vdbburkj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zzlrdmro.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dwxcrhzw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3csrufnjj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3mrndphmc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kemfrhxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgmbemzi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hbxeetne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdatxkdi.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3fnbryzvl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ulfskhbp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3kxtbwbiw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rouwgkgd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvruldsp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3abtpmykp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3rudlbgvp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3fzwjriuo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnjklvgi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3znfdthti.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3sapgtrxk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lupvfkkq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qbkfqsds.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mprvdkun.html


<!-- 参考信息 -->