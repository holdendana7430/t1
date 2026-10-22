代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubuiljji.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2yswlttsn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yisomunh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2accubinw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ijicwuxf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oeysxqqv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lydabpcm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ibojtfvv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gsmkwqza.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rdyyiymd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kpxnykop.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ydxkcpaw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2vajjqmgs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qudmhrjh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zjnrfgll.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cjginqrh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2odcggvbh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2arjhsxcp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zvftmjfi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mbolfzuw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qflnhjzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imgvbzym.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zivvstiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xknhetpf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2adazqciu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2eioefwiz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wbybkrql.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nssrmers.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tkewwmue.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nhliawvu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2nzwagpnq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2secdqkws.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zjjcdzzv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wwcpfqyx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2amncssaw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jodljkwa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2axkkpeur.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wlkpnbyo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dnndgupb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qicyceko.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ksahctqm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2stcdofjf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2bvvoqqfp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mlrfdyvt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zjqeioaz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zhmkwdmx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zreysymd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2owlrtdjz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2yiymudgj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2pfpuqkun.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2adkkjlgt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxqxyiue.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qdptlkxz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2eijzlccg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sjzcfcyt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tdfphdnd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dxcwajrc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vdgkwldp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2vfbwxiyk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2juethgct.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kshpmemb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2dwctcptx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xrembggy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gkxxcsaw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pknnhzxm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uchbodkv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vpzekkkz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qkclkmaw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvrcytdy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2soaodvkq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmftkihz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2umsuzfly.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uuxqmvvz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sivtbcyy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cdxjlzsd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jrgtdlgz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2obrxsybz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jdivjhew.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bryxcvma.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xzdwmgiw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2gskdxddu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rmwmjwjp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tzhsbpzw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2uuzwwplp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wiemvbce.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2fdpqjadw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2sfdxblif.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2brpngtmz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gckvzdws.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2essdgnfe.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2imcpauha.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aokqlshd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fejswvmw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cobyuuys.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2qyxvglgi.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2afllscpz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gbcnziak.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtdaqsjz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cuasttbp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dsssdxmj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pptyjhmo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2scbjjfxg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uqtrdobs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iatghwxr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2izrocqgw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2awpjagmj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzrbtxsf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fcovcewq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rllzmqdr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ymbtykqw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ilukyaqw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hvcbophj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbhvdpwk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xafgavbo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hkpkhyse.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sfdggifi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2rbsyeyzv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2febjpqmk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yimsathe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rdxknysl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2rajpnzzq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tiexvsij.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gaydzywb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2hzbjjvda.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2bmqopmwe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2opvmtnwf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2lkhphskd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2imgkbimm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dlwdwjgi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bwibcefs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2iwffesoo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ivhrcdrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2litrsmfl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2yhfamwsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtvzurjv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ngrlhdmp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2wtfluzhn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdykafdb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pyqfykqh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qqpaixbr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2yerexuaa.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2iofybnie.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwjxwhar.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ndffqnqw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2fqjhcsxu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2vjoxwglx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2isqqwcns.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgeacblq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkrsyvbu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nsjqcuwc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cjmfqysc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nwtwgvsj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbwtipww.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ijbljgdi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fykagxrx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2svexjaek.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dvuojcnu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vcozpldp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2pjicevcs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2bewpqlgx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ahnsjltz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2psparqfq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yuaxjfzf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mxilzece.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2imjuhskp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaoennts.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjioxinh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oswxxpet.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nulawfxq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ywrouxdj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sooyfcjr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2usopxdtr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tlyxtuql.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwesjqla.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yituhtps.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppvzxeyc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrsnwoxm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qrsdgjbv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jzfkyrav.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2pclnkidi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ilmywldb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2iuulnqiv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lveadmgs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2urbvgsoy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fuxpikfx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nqdyoiqj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2etyjffyv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2evfwvgpj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2bacasnkr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mhawlptd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2iezniize.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ovbylits.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2euyjalza.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mhjcntkv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2twiecfto.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2dziunmtj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xqulshcf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hsavqitd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ntfkhnki.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2piygvfos.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2lqrcdtaf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxelunac.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2yhsozqyb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbkaegsf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ncquvhgg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2oxljrrxw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2coyvyycl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ucxyhuge.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2sfdgzcxp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2uhsrtljj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2scaulbec.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2twveeeoh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlatjfyg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2gxgnftzz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2reccbrbh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2sbnokiev.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2gttytfht.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2wrzozzsm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hjtvggtv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2lzsyawkd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ovxkvvle.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2gqkzajnw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2acbltdnv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oczbespp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ygafhnlu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zsdbnehu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dvyonlsj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dbnjazyg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqhrflyf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gnklbchq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kslvmcpk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xeyikpea.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zxhhivyk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2glolyirp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ztefusqy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2numsvtah.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lktuhlzy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dphbvroy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2moizbxrs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xecccjza.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mxmdhuwl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zqmhypdj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pxfxynpx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jprwcqcu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2btbwuqaf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uatckzyu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2thyrglrl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kqjfeouy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fubsccux.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2enmtqhws.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2oncooksz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ooblcsmt.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2bcftfymh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2avgixjfc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2hfcraesb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ifpbheiz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tfrylaka.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2mxwlimaf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jpesghfp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2qxltmqfa.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2siojgrzk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2zypirodo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fglyqfbs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ntjnhvjx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dpiylotv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ovpslphb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rnqteozj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2abnvoenv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2kkfbbnrv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ysaspnks.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2cqxwxjyk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qzqdrcza.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2kjztvwif.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gzfctuka.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mtdslzeh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hdpngonm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2dleoxeti.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zdaarqeo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kresvetx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlyrqxvt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2evoqbagj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ueocywtw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2mqmybazv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2mpbdasgh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2fyosrcgf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qhmycdhu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvoltvcf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkbggulk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ocvvmyov.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2kuwdksmb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2gjopumri.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ymchehdl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2sjkhxxds.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhfiokon.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wvrauiew.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2upzvnagi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nfbbktjy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2laqnpexo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2vgizritf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vihgrrfm.html


<!-- 参考信息 -->