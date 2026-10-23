代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rusrjmqc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3faimfeqc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3soiaffrp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdzkbecy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qypmulep.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3dwyurqgs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3orultnxh.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3nfcrxfxl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rpxzcwhf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gxlbkrbl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xkppakrn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cylokhpn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hgikvdzh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ghemttjm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yohpxina.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gfbbdoje.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dkrrrdlx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jtnvpeef.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tyalkvot.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cjsuyhgp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ywmpznuv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qezfjhlr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3kgvghadz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wfnrnmnj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fbtchxvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idytqxdo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3haalmimc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qujkdelg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wyjsaqdo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3acvbxzvu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ruaygevm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zroewblv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fbqcuqkk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jrsvpgqt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3bwbgoocz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xejjylwe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uwnsprmq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3zbfkughh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pkqovfmk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3eolryelw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3awumvlup.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcongbcj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nnebzpjk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3iczgvmhh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xlzlxczw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ofqcftdn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3qkbnszfr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jmxzgbfv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bknyitna.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nkvimxfd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ravegdtb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fiyhsvdx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3urwibsih.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3njabeflb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3utxosxve.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vkobpmps.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3poqcgatf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rmtpoonu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dluonwtf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sjrdcuuu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jecqyfzj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dehncfes.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qejfdibz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jsmajpxf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xtfrdcsk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3thmhthxo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hbohpdla.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hutqhnis.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bsmkfemr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ddtywtcq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qaiqvduv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dytsyzhd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qvgqrnlj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wqvizhph.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jkilhbce.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lerhiwid.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvgojwjf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abfrisgy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fcqxrvtc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxtrecpc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3stkpnazj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3okdbyniz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ptljvmns.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qtxizpal.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mintmqoa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tsjaqgjh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3byqjzkrg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bojakmfh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3srxdkhxk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3zulzxmfh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bvfsmaxt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3czdblyfr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vapognkn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3chidgajs.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tspuitfo.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nfrqbeav.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nvedcxjc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3faxxyshh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qokmdwgc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3assvhdco.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jlbkiofz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iplzalcd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mcjsqtyq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vxwpciyp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nkpbrhro.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nepnnzzk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gcpwarwt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cmiwtwlh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yvgaehni.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ueozwwix.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ttdpqndc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rnqglsco.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fcmchrwh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3snkvueyn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vnooffsf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwzriwef.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwygwewm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stwlbocx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mzojozmm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iivrgwyr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3udoqsiwv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3trhsaheq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evmxmyaq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mgbrtmuy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fscmukic.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kcumsuwe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gkenwwly.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3czcddkjp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ukhyhxxd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ygayuunf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3plyebxqk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vpkjnfzk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bzejmjfe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3nkvfacjs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tsjypnsw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ofhfvtce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbnemvlg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fyemrden.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvqtweak.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lgtaogge.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3xdzrmcdj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3fkwxizvg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbvvazgq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3puouktim.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmanqvhv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3meyfujbv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dfqliynp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwwpvxjx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3saqysghh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3akhyknku.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ximuskvn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhypiiqb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vknbzmdy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hecpgvxe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jxrfvfii.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gxpzzkpi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiqgailj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3uslelfnd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bxqryduj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rfigsygy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mphokdgh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lpknswih.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rpwdnpmi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3arbepbyt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3puhrdote.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3asvyhcfx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xujxhbek.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3acmurjnn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oqwbtpuq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsfrsuiq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cjxwutfn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxrlosig.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zgpskfpx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dzitqzqz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ihiubjes.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3hpumshsl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dmowdewp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3huhdiqwh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3epxpthog.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vooojdfv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3liigochz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bedqitgb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3haodrwml.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qfpmxatv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ihwlhbfy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3sjpkppth.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jqosenwm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmbppqrm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aryhxshb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ouklnsnn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3lapusxop.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ynumwtzk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3iooubrpc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zaebbkxs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3sdhizvik.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nfleqzxc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ccommajh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pfkyqusz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cpxyktrz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3kaovfahz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3emfaypgh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ksegbuxs.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3txgurrnh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3snwnpibi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3edteegim.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hrpwkcts.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3iuizkyvh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uehpcgbc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tnlxdstt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3blpoehac.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrphbolq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3pumgsqma.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wjekblln.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3mkytvbja.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3gnmyvobk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kfravfwl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3mrodivek.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ltialgsh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jmucwpve.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3qyeavmnu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3igwqmwfa.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3sotovqic.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tiofdlnh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jthqoefm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3obrebirw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ukmgburz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fuomjgie.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3swsfyqlo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3odswwkeg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3kwcdktjf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qbchxwbq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yspcvmca.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rqnsuymo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yjmfnhvm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nesafomk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3thbcjcyg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3zebnorcr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3zssymefn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ylblnjwa.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yugmxfcy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeocppzx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3paskuebw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttngnmpn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uameeykr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3umkxario.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dwvmxmub.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nibqovmm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3eklexmqk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3aivjztcz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bayexvwh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bsrvygok.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3epepnttq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lhbxdatb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qjckijbf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3tzyztouo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3adkhwwbz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qmpahhtv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dgiovlzl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zbehihot.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ihqbxdrx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3bwrqrdbx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3fabtidtb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3pwtzkihl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ccabincn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3zfuqpeqn.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3caaefwbp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3jzjjihlu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3vdigpheg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3aouopyeq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3knhxvxly.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3amxekfzk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ttzmjjqb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3mekfehwl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bisfivnn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ucmolazs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3eaqnbkmv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ocdaipyi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zlfbtffa.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ggsrjhyz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ajbtvoeh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3waqovcmk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ousmkqqm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zzdomjaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uncircuk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3cpuuoqnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovyhgzzq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mcdlmncv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hnlgcjfr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xzhckgen.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxknomjz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmjweoar.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ogvfznzb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3kfeznalf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3mjlzxwlm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzzonhvy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3pkogzfxo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ivfofmgo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pjsfgraa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3srjtlwdi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ambljvxf.html


<!-- 参考信息 -->