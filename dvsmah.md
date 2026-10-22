代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2mqahfhcm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oartwomf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mvmyrmdh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2utoyxmqh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cfxlanli.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2gsjrbtmm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jfjcpfhh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xcqlufcs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2xfvwhnzx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2boyqbcgt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2upergudz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gljahsse.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vrsarnlh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sqmeighm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2pnxjehxi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2figndyqp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sxdlvhkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xleoactq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wiymvqgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozzircfk.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2gfsttawj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wxwkddok.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cbmzcuye.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2avmkijvr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nrnmjsem.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nxxrtsih.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wswadkpw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkrbozve.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gfidynag.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2dciozdgh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bugsfevx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2givkzbtx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2afmysrmz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwxnybft.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xjqhmvru.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ytrqjogc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2pcfwblrk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rsgrhobq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jphsjuha.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ihlmwozf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jlckcebh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xsbamkxf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bkzavyjo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wjgdygis.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2joxeouzf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jcabwshk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qwfmehmm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2evzgcaxv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sphsivgp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2lahdlaub.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pryqrljt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vizsjalx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ovkbedcf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wkxzxfbc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2txgyjdbl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hkehrovh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mocquulz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rxvypdwn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ngntiohu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hrqkwemw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bqvhzuss.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rjsehbil.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qotzvpjd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sldoyman.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2slfzwcoq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2mrpstyyl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdtuqbnq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wcekxxwj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvwscvup.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nctvfhgj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aiipqbcy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfbmsplj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixbmelrf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kmskzpdh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2nlkvuulp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kpiohmnv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ggvryfdg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pbayrcmi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2thvmzhbg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2uxvnzyxx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gknqscdt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2pitwulnw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2jnlvhwsh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2szqdpsgw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tcrootsc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2clbxlxxi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nirmahrb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jzegwdmf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mdvmwiwq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xyumqqbt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2nbbkhigy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tcobxzpu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2rhyghypr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mkqfdtxl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xemuizsb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ueaqzlke.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2upcxqltf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wiaiesrl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2uhnazsry.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzyxrsvk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rzyqgwct.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2cazpzkrb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojlshwsa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qgjhznzo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sucxrukb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hakmikpl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2gqolebds.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iwuihpul.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vuiljpyo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dblixedx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2mhcogkad.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2quirlnya.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uamzdowe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzkaapbd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nujukaja.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sajtrdqr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2exyvczuk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2atjvcxgx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2cvfsvyng.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2vkybpezz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2mufujaoy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zyszdlqn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ekruhbst.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xqcbuoyg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zlfuzmgn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vfnctvwy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2chlojfea.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qjssdgdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqnxupay.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2grmqnmjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sddzxkqq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vqvejpnl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2msbvzlah.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxlqpmoo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqzklgtx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2flfdcwuo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2xpkfaxdy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ceyjoadv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2slhfupdw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbbsrpfw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2wzffbbde.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2kyvqtdgm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2oxexupps.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvklyeeo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2endtezmo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyrybmoj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2duhcglqy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wqymttmv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2drmeqzie.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2eusxjfpb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kknbcima.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gpjirlnv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bcjfxjnx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zomzwvfl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hyxsqjir.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2aapaegvd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hwhewjft.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gwetuaaq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wzrcoork.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fmtfglsm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qxtrcknq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ribzluct.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2elouxcgn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlxylycu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ijuaodwb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zgaqvseu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wwgfqqmn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rpegcvjo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2dznalpow.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eojwhggw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gylhjgsl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2glzwvqup.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qefycwzr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nuvxefcm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fkqaclef.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2mfixjjze.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gcmfxavm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2qgbpzgmu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxarbonf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qyqrnovd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mdmtfobe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qusdaxur.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2akovhjop.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2lijuwhnp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2lvwsbbku.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2kdhctusm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xzfcyyki.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wxznjfab.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dvtwygia.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ipuynbwk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zuwxjfby.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2dnwayuhq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2yujsqktc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pxjlaqss.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2nqjbdadg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2uascvqrf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qhgukyfz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kijucqmb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dyabiyrx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2hqxngulj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ygxurmir.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hxzdguyp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xocjuviq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2remygzmj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2aydfqmkc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jwgsagho.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ygyzpgcw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2gnnowykw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2fauvrawt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2luyhimfq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2opkuoaql.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbgehqfi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ldpndaob.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2cbofcxlg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xlknsemt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ryzhyauu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zmopaxqx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ixegtufh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ckfnpzqb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dwrzlyda.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ppqttvhu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2itgbcxhs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mtktzxsk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfgfcyew.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzfajipo.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nozblspz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejkdikth.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iigluwyy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2kbbcvqsd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2opnrtrop.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qpzipxgz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2umywopee.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzyvdtjx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bhtuywet.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2erpxwppb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdwygmod.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nfryjzzk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mnaucfns.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2viriaoak.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cbdunubw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2xerufznw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2keqsiajg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jopzwwlo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ofkijqlt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vwxwhqvk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tshtfdaa.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2sqbluzup.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2fjpfcnav.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2puededmm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2oxjvikkk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2suvghwjq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2stmknwan.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2zwmskowa.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlzjswnd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2flrpowxq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tcqovklc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2tushxlvj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tgwnyfnk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2udtntmkg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2rbqyenyr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rducjlwm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uafqauhe.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dnkutypw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2jswlztxm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2dxjdvknw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2oxdpiprm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gjriegld.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2lcjkafxz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2erllybdv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2yjdgkdoo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nboapxkm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zbqfwvpx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ozsjvyjj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2yjgcgyss.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vufjrjpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rdooyhba.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gxoqajkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ouqzzxqq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2crsrdcdp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bvuibfsi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2cvmkbzku.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ucliaila.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzutxhbm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vausvbvw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2wyutkwkd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xpipsgaz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2tlfjlqax.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vtlkrvla.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2uycsdkom.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ytfojwci.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhwkzgob.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hgiyqdvp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sucjqzmh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2fhqxvbte.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2iwovejes.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gjlnajxw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2firjywom.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2sczzpilb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2smkclfot.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tzndrfjh.html


<!-- 参考信息 -->