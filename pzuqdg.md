代发 wailian999

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mmzjecmn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3visvaapi.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nsptbzmf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3tfmnegnn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3nzgvvndb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3desudwqt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3pxipgtwq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3trydnfeq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtcexals.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3stjkpbyn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3crmlyitj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3wszdahcd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ipgdyywh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qvzrqlyp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hmzcytkr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zjdpgcpg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dybgrwrq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3eolpkhlg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wsgyqfqn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mgacctvk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3tvqnxzek.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qkvgmtoz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wxarjhxd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wbzqaadg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hejqzduu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cngviylq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3fbrjeypp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rcwyurke.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nvwzexmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvjflwkh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3tgqyclrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayeoadan.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjmiddyj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fvmyqegd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xalkrour.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3svgtvvsw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kmluxncq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qjewshtv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3zjromxrn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bppdqplv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zbscdxve.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rjsmbiga.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3iepdbodt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3hdctrctg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fgdoxvmc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kxzknxsx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sqqozihs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3oojjnfsn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ifqukdir.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucydiwfh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zgqiizov.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cdywtscg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3igcvyeyg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fdevkrkg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nhrpjtoq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kiuljlkg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3omonalhp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nwovvacs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3byinzvyp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cxfknynd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3illperzv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3xlqzoiom.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3warzqfcb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mwakkxsp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3roinyfxo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tcsagdcw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ddxjlmbo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tecqhynv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3obdbkmqh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3glilyexf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iaafhtbu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxsyzlhe.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rdsebpsu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3npsghlzg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mzowrtik.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onkqpgkl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qavnrquf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3dninxzdv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afcrfnqg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ygagagwy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nnzghmaw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3czbwnsma.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jcdwjoth.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxqnomtb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3radyrhpy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hiqldxgz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3azclcfas.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3otuotphv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3teemcadw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3aryixmkk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hfxkvxqz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3iuxximnl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3oanohogo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3botivvvb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3uisolfsr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3aeddnqtm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fdwnzypj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymcqaggm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fcyucesp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zupchogf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pfxwiqsg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ihipzvvs.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wyhhmgfo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3easojqil.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mspoares.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjccivvt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yhifwowj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3izgymwsk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3scqicvps.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yahgbroc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3gwbjqqbs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uysgueql.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fwazvbjk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3niwzhjmv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3siyulbbx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tulhvosf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgacvepy.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3geyvkyeh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3npweymqc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lqwfwmwr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3noypragz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gdzrfnpj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3cdaxmfal.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3arrlpier.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3oetfvadz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qdkcmrqu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmcxclgs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nwkjmmjk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fxpytpvh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rvtzzscu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xyvbmbya.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xfwrhapg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wzflhznx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wvdujsvl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3guwyezdi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3jkokmwwe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zwbblapp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3pjgdtmvf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3jkfzvpxi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wtuhdzir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddtzijpe.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qfemmabq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjaalzwf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3gqrkalmd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ibmhkicj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3nwiwhsnd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpjpixbi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3neokkihp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rttybvsd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3fynxpnum.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3eswdxjuw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iramxmlk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3adnnshio.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ioklurfp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfrcngqs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lqucidic.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ysjsygjz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsimcjrp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lsldhafm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dwvpoohs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vyptgews.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3oenuxcrc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jswlaafj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jvrztodx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xafceqpz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zogvvtcw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3kjtdhbyc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3hkesscxe.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lhgxtttk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3neovcqnv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3fanfihoc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ifyjbapt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3igemggkk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fducemtj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3flcfdfvt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zqtlzlle.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gogeztob.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ljmpuvug.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zqbtvaqp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3pusnyagw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3apfaqnkv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3owkbhust.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yixgorks.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcncfmlw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdhiymhk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3vnpdfqgz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cgfqghue.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdxpdlep.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3hpsaerrw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3dxbawqtb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3avdsvuup.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwtwiifj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xfrkywit.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpcoaoqe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3axvbzswo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3cimtuyip.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ryyabcdl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hnnoodxk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qyouvatx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pjbjzfdk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3abagfnke.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qzornacn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3okjnkofy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qqtvmpny.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3nsjhurin.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3quvcvayo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3cleyumzl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pwhbpzty.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jplqwvms.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3skqzvqse.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuuihedr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mopniktc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3isdqhqpd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ndrftlrz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zzivhprk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3szmrkerk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3vnkywonu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3rlqxrrpt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ufzdnztw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3dncdblks.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3uzlrggoy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3onbchxtg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gvmfmxja.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3oufiaifp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fcswhmmn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hkpxbwjx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cinaborm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qguubqpk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3goiafwwe.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ukuyvwmy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3esywyiqf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vidhyvup.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mmhdcsff.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xmppttfs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3uichjbdd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kbusgiwl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3odtmbumj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uswqcrto.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hopbssmz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xpvaslpd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ulksrmfo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkdeqgiz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3urosgbiq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wxtixuga.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pludhxoc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3opcyhfbq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ukhmnjze.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayqcmmgk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iifcykig.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qkjehdfq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rumgrdae.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3uoozbafu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3oqzkmghw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fohexnfc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3finggbii.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tlfnnxng.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3alsuwwkq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ouhsumwm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rgjakstb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3xvurdplm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3biqjygir.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zdqgsose.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3otoyeqpp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mqsokcnp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zeumwlqp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfeeuhwo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3htmgrxry.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3deywyqbp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3szmhzesk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nvlilxvx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hriohfgf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3uosnjltj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3pedmimey.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3sxcgavmp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3icxorhmt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3pbslqmyh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ohupocht.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzzuobkj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3okgiinkj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3gzsmbhuc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hahfgyzf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cnnvdqfn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3djgsxgky.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ponblpej.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3oruellpp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3tzwhsxaz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cmpxbcpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxzthgyh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vnipxkhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vrqrotym.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3krvaiqhm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3jwdrtgrt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3uftjgaur.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hzedfyxb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hspudqxi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3lcgbiste.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3vqzbvgtf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3uhczwuzw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jplvvgup.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3aoovwwic.html


<!-- 参考信息 -->