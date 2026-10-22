代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2harjmpzs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eztltfve.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vieyvgrx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oqoqragw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pbkuoijo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2wanpfkub.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kukljcjn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wvxjckmk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2esreqqpb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xoxgldfs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jtqgammq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pszzwejg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2crgoqfdk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vohfoozz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2tranvsue.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qnaghodd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2axrwsujc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okogdkci.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mdbzopey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opkltyhx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2snhcbioe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vovchgwp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wbqimtlc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2oqlliyyz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fchtsrsa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bjbrcqpr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2stcjuurv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvasjgyp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vnmswivx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2cdzxguxv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zsnyojlp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zyzxrhei.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2umxqoqqw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2iqpqjdur.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pwupyayt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2rzrgcerr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2rkqhhktr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2zhqcrusu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2pmnfvfyc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2utmscwxs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2crprvyob.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uzbfzxzl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2npohaaqk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2hbesczpj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2siqxcelh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vxpxuikm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lusbqiop.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2esxymrbh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pjhegaaj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2amljtcfb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ojustcgv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vzafrssb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2cexrwdwh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ghoedzzo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2smkubvhx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mcsxknxl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2eopdwdyj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nrqohztu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zjevcbyd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hgkhtaja.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwxrkiih.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mohysvjl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wwpbkoek.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbjjfetx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvxdwthy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2arwsmmnn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndzeulhi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fpycimiv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uuqbbptn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ndblyyhm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cyfwoyla.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqmivunp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rtnrcqpm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ksjhqxrd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bttcfzfr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wihcynwl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xrgrrdfi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2iccqcipa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bocsabfx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ksurktdb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2tgfiaqya.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2uusonake.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qcivoyle.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2eklgxcbn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ljyejqol.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2bomwrjxn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vltaqvjw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rfufpcpw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cqyyzvhf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nkfbjhlr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2buetmuok.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2magrfbvf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kvylmarz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfdhfswq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2buldhdis.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ujiicomc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bgtsbapa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ghkrhpsb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ujtlklmf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2redqmkbk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2bkqeizuv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tjboghrp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqwzleha.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hnxkoudl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwknwqgk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ovgxvmvw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ggyyoxhr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gjwfdarm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltpzjtbj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cmbzrusp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lvnzaxxl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ticmjuhx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2vvcqivks.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gtylzvcb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2npcohjpq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pqdcazxy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2tsemotrd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2umnncyij.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rksegxei.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2bcicugvu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xxaxlgtm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2cnsonmtb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2anbmhmxe.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2yudixilf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2lmuottqt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2mmgubdnw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2dszobejd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2iwxcsjkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xirpqghq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xlffrrhk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aokcphbh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2chdpagka.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2yzvhvrmb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2awevrdwm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylrgywgk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2oppmziub.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuuzqviy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2gslaqare.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rnnwrqgi.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dkfwjyqh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qrirqagx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rqztepuv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrgswgwn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rlyawnmo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxggyazz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wviydjtz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bgtompwu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yxzfnexx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yodbrlmf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2uzmezakb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2yltaspsr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2npxfscii.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pxgcnllv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xebfgyor.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2arxahotp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2snkjyrqj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2imbjxytn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2lozsgcme.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2fhgoexgr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dhfpsxip.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yalavzom.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jhawicmt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdiqigze.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzkwdrdd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pmxpyxhh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2efvmcysb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fusdgmun.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ixxgmpqa.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qygumqul.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2myvdmmou.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2omnwcuum.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qnuoozkd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2afdexytb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2knpfbqkv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hglarvat.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbzlufce.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qpxzmbho.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nbsavjey.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2teyyhdmq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2irclewvk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2padfppnz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vhjabzmu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2nelqkvrb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2bejsvzzz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dxqxmnlm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nudqdcgd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zduhwfab.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2svthmwye.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ceytmsph.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kyqbkbmb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2apeisbip.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2gqdvwjdc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ssmycmpl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2frvgelgt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2pusphkzj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2lxbyuybw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2itdrhdkr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2igwagkgd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2kfcfdhgk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2wslbjyhy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bcunmtsd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vphgrapv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tllsdiku.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mchusnvs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zapxgooj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nhjvwtgm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2jgyllixx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2pqkjmhyj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wbtciwrd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2arnrkxzd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ciubudkl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qkmhctqo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2gtinslrh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vtcyjgee.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2smgnncvg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ztzvuplg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lovdvysc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2mbsjbrgi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nxkqokjq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gmzkdldh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2rsnvvjrl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ewdmwkrn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nuprlmgo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tokjquti.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ycpfkeca.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ycaiojku.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2konbjldw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2shpxhjcu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2emqsuxrq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2odqojchu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2kjomobau.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fyruplrx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nauezelv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kpasnvbp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkbpuize.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ceomeflx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ehgqgtos.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2eckgglxy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rxmkbror.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2tfeefelp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xfgyzati.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kdxrxnhs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2susudehw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zotenwsd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nlxsmjeu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2uyvueqrr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2khwrocou.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2uamfojgt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xbnuenvc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vjntlkkx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wuyyqaet.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2rppxjzcz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2cxvwaaqt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2voalrkqj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2zwazqdjj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2pmnhznpr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ffdtpuwo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dmprpojb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fwuvmkeb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2juzyiwkh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hjjiwapz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bnlsvdud.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2snianjem.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2zdrnhvcq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wrjyiscq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2trrbuwcu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gsuszqhp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2inckivic.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qnfaanmw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bsldocnr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zosmnhpj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2wvqtwqvf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2urlulyvi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2gthfprvf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kczjkaev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtiqjzea.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ykandhcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpcgzaib.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ipzofmes.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qowyscvj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ifihnrxs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qexaubij.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jncffofr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2uqcssogm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2tcmrgsxo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hrgbkeoz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2llcqfxie.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2txfyxiqb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2rmomfbiy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2thpygvnf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nvtocrfx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yntxeppy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uapaaekd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2socgcpvx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2vxgyevbx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jezkzeus.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dtyhcnmf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xqdlmkus.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dqnczvvg.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ergetezb.html


<!-- 参考信息 -->