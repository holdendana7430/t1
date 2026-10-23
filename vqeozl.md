代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xvvlotmk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cgfngjmj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ogiwubih.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pqqvkwib.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ngvjjpnn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ozunflip.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3egimbkfx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3geoewcxj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3agihizhi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3jixzqahu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdzvncbx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmepajow.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3awfpewhz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3tbsqjgxd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3bzutiyfq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3sxuvqknv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3iiwcthsp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ustitbrx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eidkdtgx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yxzmoinf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hosgmkac.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kpouflkj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jsofnjlg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aaefehqf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3itnpmftt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rydfybmd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3eayljfej.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ubztxokq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xomrqvns.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yrqjpfve.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ohixjzka.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nhtpdgxo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ybhxmdac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vozsoajt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3atkrmqoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzgzyprw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jopgevjq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mwsvsvny.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mhnatqyk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vpfsowdo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zystqjya.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ogyojspg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3gcqrkhle.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fcwtgxlo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bacyrhvy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3kvaugouw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3znsrgbgn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3suawzlxu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lqpxirfr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qppudjng.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3icrjrfjk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hpobntgw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ocafnujz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3zvfwvtyn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3gzukjcfg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3depyzxfb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3trkcretz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3msujblvb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pevmtrhn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xnpvgcgl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ayzrkkhy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rxnvbizb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3aymuqqeu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3oiuxypwz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cxioapsm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gpqzdqld.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3euwpunjv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kmypdnok.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbzbfdu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cgtlcfxt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3fsvcgyuj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sujhxsqc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rltcvbxw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3tzztdtzp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gszhizia.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bqhdrujy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emybhwen.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hquxqsgd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yrrppgph.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rudesdhx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kogvhuoq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3szghdnkc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebgourul.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gylitbhq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nabvsjia.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3limohjwz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3enhiipsv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhduoafa.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mabxgyfl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pfigeblh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3iaafvwvx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3crpimyzh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ornyyuzk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sfrgaleq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zllpzdmo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3yffychyk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jhsomimd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3inodzzux.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qfecxyqo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3oyyfjhgw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3uwmmkwcp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rqlkdmmp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wgybphqx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ptdnfdye.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ppidrbnq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fzkzeitw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fvgtghuy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yrpiboin.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3rdgiznaz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3japvvvdn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uhzdploo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3izfykyfr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lwhukyee.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hlfrdejb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tusgqzxh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fkelyyvo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qtidtkls.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xhtikenn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tvtcprow.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ivgsewhe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yaslxqhz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fiwmxhok.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3cftqneec.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxzuzvyn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vkagluhb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvdpijqh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbtmhnon.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vcajtjun.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jyasyfpb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rdupkleb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zynerozd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vqpqtuny.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dpbrolcm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3piwodqzp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xhalaaln.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3lsyhklso.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lamkulme.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3kkrupdwh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vfjwljka.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3fxywboqh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3csogxpnn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3lwbfxpmt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3avtkaqhy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ykfwyfor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqxmpcuu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3rhaceuwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxcowida.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3irhrrlmq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3guvxmeob.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hndzajrv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wdiatkft.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwyeklgk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3rbgsvogt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hzqbppej.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3iacumscy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcmtmfnr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hpyvgbwk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3fvhhcjvc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3weajpntg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rbvuqqbr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3yxskxlbp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3alyesklk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3erkewzcr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ajavfkca.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlbmvshg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3mvaxcscb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sykjongl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ngxubnki.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iuyvwwal.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zcisvtzt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3fiynnyqh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ovlsdnys.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ldlqaqna.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tmdgnhpa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rhmzewur.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ofhrvocl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvxuzmxd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zrbyuyfa.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsyfnuiw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqhjgsbq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aikbhyom.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3suwmskbn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tlfztyct.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3iemushub.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3bvivvhrj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipsvhokg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fjrbehcc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uvrrdcqh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmrlybpn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ckeefelc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zhwjjroa.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3adwviqnb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ipjppnrn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3trejchay.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ilsfvrho.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3itvlhgzl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nfraffta.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovbjyxsd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3sqidonzf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3wgvpzdyx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dvbyniww.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rwidjzpz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wxdzsbmy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gcmzucox.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hbnktrso.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xwkxtbxb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3glyxhuol.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3wrgjjjbr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3njsdidqm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gsmgtrjx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jzxdztos.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3nrcesvyx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eolxoydd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3emuzotqu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdboykmv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhyequih.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3assnlmqr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ugxrmxcw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwlvhiul.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kylxddjf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mesgvrzh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rohhqozo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mfjddmdr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3sihaigea.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgunupwe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3iynbcrfk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zthgwtcb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3kfosztci.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wqmsazfi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hpqcsbra.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gxfpgwad.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ckzbinbz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aohbcmny.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3tnanncet.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rfrvgxdg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gwgklzht.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3wlpkobnx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3tuttrmyu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3zdzlezcf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjwewbfe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zkzcvzgj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ppnuijse.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ejcaybkw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vgporgaj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3mxnjqnnm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3txfvqgtn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xhqxgjcu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3erbfrhme.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vafllymd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uuqujjoh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zkinjhon.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3scmwksfj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iulzyyhr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bsxftrzs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3agiymlnk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ehhdgacr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3kijzwokb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3okmxqfri.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fodheodl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gkggxycr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gpsnsjbo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ckzkpvtf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3izjqcsvw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3bosroiag.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3whkkwsfj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3adklfbgt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3noelhcwl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ygowvwbi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3pfpfzpxv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qltjjavc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rmmlqjqp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3pzjnpbca.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3iavntrzc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ozkizofz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ewflmpmq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcpopnrq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3fedsawxz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3syzogqqi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3eionvvou.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3frwjpoww.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3henaxwhw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yqkwsmtm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3deusfmvt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lsgpyqfi.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3wiufyrlz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xrjqeoou.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3krrxvbha.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3zvxpilxp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ceenards.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3npsjkbwz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tiehwgez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odozshkl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ubgchwno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cumkrxyg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3csohvisx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ecknuveb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayiuyhte.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lkyyvlzj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dczdqano.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ektumifx.html


<!-- 参考信息 -->