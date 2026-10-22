代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2gyrwisbz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zviwtvna.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kgeenjfy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mrnxmnvt.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnyttadr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2esazjxoe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wngxhvct.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ekzzankl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2uxxoxrkx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ncvxdvcb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pvkhqukw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tqtozbce.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tqlthuod.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rjpovaqh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2irdiwgth.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mkkjdxwr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2vqwyuzkd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lpdmxusw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ctaviqre.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fnymxtqn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2adypsbrc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fylusqvw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2fweybxgr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ozqscenl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ugifhjvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oacrkzxu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2cjvqmrba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbfqexau.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2acvluapp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2tafwmszg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zvjktrkq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2tvpzwwfk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tzaskxwe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lnjajksk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2scdemaqu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdbzaimj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bomsltkb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jueqpvan.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jkiugnkb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2pzsjdudn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgldldmd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ofwlejfi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2grdkjwqz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qtvwailo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ajqvtnrb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymuryiov.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2uzqofufg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wtdoictf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jlifiwvc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dorjnqkd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nbrnnmsj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2njzreyym.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2gfinjgpb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dxjjnjhj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yoqnkyqo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2lslynbyt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iqppsbny.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2kqtvfmwn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mukulall.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fdbcwuol.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2yvizycxk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2niaksswt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2kpuvpjtt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sndjddoe.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xdkkkxun.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2nmzthjau.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dkljdtrj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brbiwfla.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhlalebj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ymbbnbta.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2hynzofbv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kfcdtfpp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cghzihsj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2rdelyqlu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nrnmvyuy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rsspyvvn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2drceplwu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2canmykwy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jbggivca.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tekishmj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nwenyipa.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xtmxtfsr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2grxjmuav.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sclgqaqp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jigahmlf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2uftdxefl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qforchrb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2lmstpkae.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2pyeuhsut.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hbrsfman.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2uxngzayd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2htddpquj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wqjvhiyy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2unjwsvsf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jqflryem.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cfhalhco.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gfucuzar.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ukwrsjlz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xxfvkztq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fuczngpa.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2zoqsihcm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sztsqbfs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dbbxgmcr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kkcbcvdj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2trehnont.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jghhovtk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2wvhhzrbs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vqlxkbrv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2prfkvcih.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ashrtxgo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnxbokno.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sytqpbjk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abfoyqgm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2thqtobdl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cdyxbluw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eewjlzsr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vlnnfkjs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxeoflnx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lpdsgpnq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kembtsgn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pmzcutbg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jbbwtpqy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcsoymwi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2obzrxhbf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ffnrdvgn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mnytqbuq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2xanljdiz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kzysjqus.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2mcwsmoux.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zqvlfcrl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2idmakbox.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rgmwllrg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rgimczcg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ygsglabg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2cffmibwn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hfyezrtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfdwfleo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2tcywefpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbcexhim.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kkuepjeh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2kewaqfbv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2prxefmeq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yobwcndb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hzrtbzpa.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbefubse.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jjdxebjl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xpvwvjor.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2doakfgqo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2tjhlbryw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2gtcxhxob.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2iuxihads.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jebgwhnc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jztmptdt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pnhdeqgq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2lcjjklju.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2giwrcysl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbzucrhx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hahfjqga.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zgfkpcda.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zpmtuebu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jnzpwlmk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bhmcbdeo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2owxczlba.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vzhrwoce.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uqstltxi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xrpqdufm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2rbnqfhhw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mfndsxio.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2paxzelor.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2izqwgrtd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ppyatlbx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxzeexdg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oejgkrzh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2toqtykqo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tpxqydvc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2upccsxml.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xgfvabgm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzvtxbew.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2epkegnzw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2duoqdopk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nlrywmkt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2vpdakkjc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnjtjphj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gotiuadj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2hyxcfeff.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ohnnaiih.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueenhptx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrcdzwoc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjqieukr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfhimdtl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bvwroand.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kzdsbxgh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2dmijuizw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2zvvikffw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qmoajxvi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2enslgban.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ucidkiha.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fywfqmup.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fejeheay.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ekeqcxli.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2tijaxexd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wurxstfh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qmiiqzle.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2idwrcfni.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdwizvps.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nmjisruu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhjxadhx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2glzamibj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2kqpnkdte.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2hjglpujr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ekajoygl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wnredyjf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yatbqgkn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkmllnwn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2crmqsdrf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkvnttfr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2huinpyau.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ffmxhkwb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2gtfoswoi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ngoevxgk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2odvnrtpt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2eohlmart.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wdzfpmgy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2rrkltnmb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kvohxvat.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bhgihfui.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2acwjbrku.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zkcqcdbm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hfpbcmnd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ppazudid.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2toiebpmo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpcivltj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mqhriqdw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xvkcoerc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hhzwwgim.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gprnorla.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2byiwqyjh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2njvzsmlf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hvevpnaw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wahllgco.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdawwkbl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvbzrxdu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jbclxrov.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wgljaypl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dsqqwlti.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kjkeaxzo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qslvzumx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ksroghvh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2mjieneni.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wyrwzgjs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kywioqnu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qemkchhm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gxcnunrs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qgarjftu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vfrvkuru.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2juhjqava.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pysmceuh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mjzistki.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2pzosadgy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2mscnzzza.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2kjmtfbmp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnxygrsj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gdkfairq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2uevtwqsv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2bwfvgkzi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2npwgoixe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vjemtnsf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2fhnykqir.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lfgsgcqh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xxwrcxgs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2nbjhwokr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ieqkfchz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2fwgbiwoa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xodritik.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qinduizx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2vyzqnmad.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2bsignptt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pwgjpafo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gmikvftm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zwmscjan.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2kajospda.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2etosajok.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gulmqhgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhijwcbr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2simmoweb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enybpums.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2jjfrmunn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ybqmfqju.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2snuuadnf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndhmblhl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uazpxzho.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2eoxlofgl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2wueaaqqh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2cnswtbdm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2zmcsxtmo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ntumrrpt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bokystif.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bifhcuzw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhcqfrms.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pisjanzc.html


<!-- 参考信息 -->