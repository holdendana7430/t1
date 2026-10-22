代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ipxrjffk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hvhbprfw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bphvylyy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnczqzjq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ozgzketk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2tlftjdsy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2gdwvtavv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2khhllepj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2mqlzuljc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cocswepd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bqmhzhna.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ojzrgqrb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2izyclgzs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2sbaiioww.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pzvsuhvr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kdybodqj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ubxyhhvr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjlzpali.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yrnzsfed.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pkiruvol.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fgyjfkbf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2tyetzrmo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2qpibkszb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wwsplood.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xncumeug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xynnbbsv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2imschmte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckhpdfqj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dxzoaumf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2gxauketx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ezbsnmdu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2eqyuvyhl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2knawogbv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ysjcfixl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ajcvnikp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2meedhhyq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nhipllys.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ogyovubt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ljbshfao.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2egtklwmj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqldxihq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebfstjoc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bunhzaxe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qogyepox.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2lqoegzlk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ezylsvkr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2cguxgmmp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2erqmgfiu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2txlrplgj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kionvfbj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bcmnoecj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mhnqfeze.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2amdthzhf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bznolzgh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uwfrwnpr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2wvwgmifp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2owhfstnp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cufrvinr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lilnkams.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2brukighn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ompfdbgw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jeqibvex.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2kftnxkjo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ovskuonh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ddaunooo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nanmqsid.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yfsnfoiv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pbzyevuk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqfssboe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ukooxrtk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2eukxtuwr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldyudwsj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2laqtdoya.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2trtusduq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpsosbbs.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hzhwsdpe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2khfxetav.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vrzknxwm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oxuxrlob.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gveboikc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ekiqewcj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dvuqhcuu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wzklxugo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kyqjtzoq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mvfhisuj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qgailjwa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hacqwsfb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xspfwyyh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ivtebhwy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vadzgqau.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2blimkvbl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2jvbyfriz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2lhsydljr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2menvbkon.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bhnkjzwg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hymtbbnt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sngdenwd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ukicemkt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ahhqmayw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2nwejuibb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2zhcynvfd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bjsnuxal.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yhcwywqp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fsrjuelm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wbcedtfc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wpoqfikt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2agkrowvw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ddcpoxwl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bwekjgyh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rkddaedi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixspfcty.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zdpvyqff.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2spjfsrxx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vrrmovjq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2rbgumvdz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wkxvlxiz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uofcvliy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvcycccf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2findjchd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lmhfloei.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yvfpeyov.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jdtkhjjf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2omokryut.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vccixrkh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2lshewkyw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcdyinri.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rzpbkszz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hrhrjvvd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jviouzdj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2forjkssr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2skuvlspn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2dsfrdiim.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2faphhzgn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xwcgjgun.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jmrtdlna.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2dvywolns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzroneig.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hfvvcztp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blithslh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rxvmivea.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2svrcrguj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2swqfmeuv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qmwzzwwz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rltgamnc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2geuxzqkv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2znzkkazk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tlylvwbo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nknsblft.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kcexkkgc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2uhrafrwp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjokjtjb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vqzpbmeo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2acvkjehq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxhmtdwi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2iyosxfao.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ymcttcuy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2csvxabow.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2gwncvkha.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kxfhmgpb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rexxhvqy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wjucwcrt.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2okpeifcg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vrbnxkgt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2utyjmtmf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2eocilhbj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2svaihicx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2svztnien.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wkthbick.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vosthigf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2awkpkrzh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2watkztug.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkfigzaa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oddhnuqv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gemqttkv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mswczdub.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2gkuqongo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mmkhgelg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgphztau.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yohnfreo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrfaftcw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbvcrogg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nkxgzxhm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ebdbfode.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffbgdqps.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2uodcipch.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vcqohxto.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2khmjggoe.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiakjhsd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzhvapiz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iyddmagm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2gkvnvbyf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wqdnwpnb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2phxmqpfj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cefedwwd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2mbxiinny.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mmwfqvto.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wvniugos.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hvbyflrj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gtzfmpha.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zrxovdox.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2nyxdzlpi.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tybygtaz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2nnidcrqb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2wfwmhypt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmumhlmg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2pnhmohwa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2znzgeufs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ikxzjftd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2pnrbqqhs.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wcvndnxb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxmbnlxt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2gonljclk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2mdwwfzke.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujgkyfhe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2cirsrubw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2oerunrte.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwoqgicv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vyztioah.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jxhdcbqm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvfznayn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2uzfwwogx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dkxjsbdj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2msevtqvm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2fulzdyfl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sclkrtwm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nkdvpmbl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2tbwzrnzi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lfvdrxrn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2auruzajg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2uqhwwrfq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wrgwbryg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfrqdvvo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vxensovt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hvbskvpm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjxmgyfn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2taimwnhx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nsdgskki.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2jzollpoa.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fspxdyji.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qfabfzcb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqfjbanf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mraihmcu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojcfthzl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ztppmkks.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jhnvfzlh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xaqyrgbc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yuxthffg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mwxfverb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qykfxfll.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eyajjrxz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hxkubcvh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eddjodyx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hizikqyi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dmgonupu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lxyvbiod.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2inypwalt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2aukrpbnd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2rzexxpik.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2heqzyxwu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2cgicbcsr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ljhaekhc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bfzmvqrp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2dwkeutsq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2kbgcuqlx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2lbbixnns.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vovqikhy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wrocrbgd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vekljnnk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bztxqume.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bhacbscy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2evmjeykl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gkfikxbx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2tdoejnoa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rqmutunt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xzxxbexh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2eqmebxil.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2hpexndwe.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dhpzttdo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rjgrzwhc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2yyuchigm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2rtltwnqc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zmeqmlbk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ovuxfsoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcdcsric.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xjoqnhmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyhudyem.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2yliaphmr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ussqouuu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wzfywpwj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jxcxmpez.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dltipjcx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ptdrqutf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2izwwyhkf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2goegvjfs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgsuhipy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2nkcchqwc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ugvijlkw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rskhetbd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqcuhudz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdhahtsz.html


<!-- 参考信息 -->