代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3opexzkdf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tulyopqq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3udptfzgv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qooframe.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3awvygikm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3pjzciyzy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wxanarrd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3avuvguux.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ihygpnep.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxyypbif.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mmnxwpek.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3inzhpbrw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3obuloold.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ptpujziu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hewlovqp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3kbbzyywu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3thgzebuf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qbuvkkzo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cjakwalx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ylhdnuce.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sdmmebjj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3igigacuh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ohpoubjr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cwjwxnns.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yxsbxcls.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ybqkblvu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gnytxxlr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bqrxuzje.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3icirteip.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xdmjtqwr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3vulkdmpu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hopvudkl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kmqtyoye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmjtzdqi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3dbsejkka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkttsacm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mdkssgly.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vrmhmrrf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iykztjli.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3xtmevhjx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3anuzoidb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pbjlqtlc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ncddlyqn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emmibbqa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dpkxzkvb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3iogqjmfn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zbzaobkq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3wfxziews.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uieyyiwn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtwbfhfi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tlwyriyh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3awzcxfhq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ymcxrxpa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtsdgccr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3qvnyovbe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3rpuguydh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xivcanct.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qlauktvv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vjzvaxci.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zvqttndr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3idwjiveq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3skhrgvki.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tcornysw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xkwyctxe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wzxlrklw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3qpkoqguo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vqaiaqtx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fsexhzui.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3uerpyutz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3svdvxvru.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3vhuabeys.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rgvjsycl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3otfewypb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3gidobcwh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rudlzjen.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzbhespv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sgelzvqj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mgoxoygw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jijkxqmk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lnhoxjlc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yhpqkulo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zblbnjir.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rigazjxs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3amjzjauf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwhbbobd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xqydnsgl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rodhecao.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqxtsspd.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eydtwrax.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fnyuufwp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3kkhogaqg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zspgcpxn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bsrnmema.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zfczzoyd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xadwyawd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3uwrvenwe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hrpxydpz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fhvuiswu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hkyvqpyj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ijndittz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ivujfbgi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3sjbskrsn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jbvrrvof.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qprgzfuc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dllzsoiv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ddltkblq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uomfncmw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3iwskcjqq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ynlhcwgt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkvrfxux.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kjumlgyl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qrxnxsgi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3txojwfzo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3otxmngtj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rbcvjscy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3shfmgvxn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3anbxicyb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jumnqtur.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3trsmscid.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cxtoydww.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sgywimsq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3saisruds.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3yfdimbfl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pknbiqxg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ughdjtfy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xlhicuhu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3kyjrkiik.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3krxqcqmg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3izbbexoi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ylzilhjo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bueziedh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xfzqtkvz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3tkwgmmfn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvviovtt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3skrdutie.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lnkydghw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bqgykxoq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3uvlddstb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ljsljcsb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xzureruh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3fdexmfhm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vhachnzp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3mbwynrpj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zkkbjlsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qndoarlj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3fiftgqjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkottkyx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3vvtpddxt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3cmogjegg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wfduksxk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuxcckux.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3hytrqmku.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahxlpdyd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3spmozkif.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ooacsjmj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yewcstec.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgntwqry.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wdqxptoj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gsmnaubz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3krqpjmse.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuwxfhku.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggwfcfhb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3iwrkgbbk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pmdkkszu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3elqikdhz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3gugqbucr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nfxieosv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tmpsaqgh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3psyaxekd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gjdrkmun.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3lyhsugxt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jjvzlups.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nwwdripf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3neappocf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3fygzvngd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fdhyogmn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iplsnyjo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwvoqwox.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wojivptx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fygbgxsg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lmykhjxw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nobnnmpr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xgpojnzc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ofayhxjv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ybfzvhdm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jpattbzd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhalowcc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xckukznm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ergplxei.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3evgjtjcg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3nofbjhiy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3geivsogp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3vgdfsefh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vdczssgv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxasovnp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3swzxtjrt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ndxcggxo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ronniafo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3juvctkdz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zjlwcbvk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3puqgwlbv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3txzycute.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bzzdtfek.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gkjlxzdl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rrnibuxa.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vgzzcpcv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3htdrwmzt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3antxoqhy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uythoawj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lfgsihva.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dftbkjts.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hgzhgrki.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3epkpkomc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3btunclxz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qwjtyekg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hjcbfdjt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mltibypp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zaiaygvl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvvosrhi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3lsavpwbn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3xlswduiy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3bdtbzsdb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3njyjfuey.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3udlvbucp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3roybbtkn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xwzlvmoi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3cioaxanl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhezyvjb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jasphxut.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3jemefzho.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nldhtyrq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hfaeqpot.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3crczylqv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3tzfzdzts.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3azegcaad.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fubianji.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ikrosizl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hnilzzsn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pjeapacd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uyoavbuj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bmgjfnmk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdttcxrs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3exmxutjj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ldofzuzs.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mkhskysw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3dkszgxpd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vmulbxvv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jrvemhkg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wdnwwfbq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3odhqwnul.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nftvlhjc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyexjsbd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tdcsbvlc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uiuhqyoj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ztppxafy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ijxfvwjd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3nvnzftgh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xleyzdmr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3shhgqdei.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kbsvwrya.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ukeimzsj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3lvpcyadu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qhrouhvf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zsmwuppg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ezdwmdxp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ozndjhor.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3hkdcejwt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3zsqxymga.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ccrocgfq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nyinfhvj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rpvyjvpf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3lvwftrcf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wznstkmc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ltuaulqi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3bavjltmd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrvfvtfb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fibdehev.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tuoqltkx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3imnmufgk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3todyefyo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ejmijlel.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3febjmjub.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ykxtfqlc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hdclcfgh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3lmquvwde.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vzkxdieu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pubkyevh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ohtkwczv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3omyucjrc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3cicbeqbn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yytpxmvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgiubeij.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lhjbbjjy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsevbiha.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3uzjxrbmc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3tlxltsdh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3tyzjjtad.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zvsxqtuz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mkyrjwoa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3fqsrcnux.html


<!-- 参考信息 -->