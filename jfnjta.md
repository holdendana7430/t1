代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3napenhww.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cjqcpsmd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fwahgrkb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zzztwehg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bgaswnot.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3phzhaogj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nhpwppjq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3krlsmwbk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dqouhghg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tegpauty.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3amxybbql.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qdgshjwu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uxsrberc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3trdlbyvy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3swiiyflj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gxaqdiqy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bzuohvvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdtqvozy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3tzjqdfgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlmfanjd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ubayhqtu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fwtomyyv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rzvyzbul.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nkbzgsif.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tkiidkxi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yphwmzoc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3kpszovoq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wurfhcmf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3utjvqbcl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljmwyymr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jsrlgkez.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gfrqcpzg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qzmfbtff.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3crqmifpv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jsvozysk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3fhyikukf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3jqykpwfb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgmzyqlv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hvqdlygz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3gbrwbqtf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mwnuguzf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cgcyptru.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iltczjid.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3spxiheka.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3yyjwklqr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3oyvkoijt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uongndxf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3gunxdtst.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nodypucw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3oupyvlxa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jzgpplkj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hkocahic.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3uwztsuyi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dkvejvsm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zlqdlauj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3rvilqgba.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3hkatgtis.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3sezpnajj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lvxcbyfl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjwivcqn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htgjepgh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bqsndpjc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ftznqtmh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ozccdbns.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vmpyivll.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dxtsydiz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3majasjae.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3znowarlh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdewtfir.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdybuxws.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ylxihgkf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3evywgebx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtnnaihd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3foegpbug.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3lfbzovvr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kbeqjbcr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3qsvaljhj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mwtldgme.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nxnvochp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3afamsonf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vwmfwmva.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3lulkwbzl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3uhldifpq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zxsqxgsg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vrkzxgup.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3respjlle.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qiyzydxg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lnnobyef.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ojprmgyp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3urvkdpud.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kriocjge.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3yhirbnxm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3pmxzmlmk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3icepjask.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3drzycgqx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3aaifytoh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xdonskze.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ueudhiks.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pyfjduao.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qnswlcnq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zwyymsjt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xcsetuws.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zmrbzljo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mpioaawq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ifeicolg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3huheshss.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3palcicaa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ttvawqmi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnhabgzp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rnaymgwq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3osaaaovq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sqkqblug.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bnvebarf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bebegjcu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwijiuzw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3thanyrlx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3eksphklf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lwdsxopg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gptrwhnc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3girtssau.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ecivnfji.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3kkdolryt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wjbkbzvq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pehvtyrf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hvefejjp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qhsnmccm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gjiafkwi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3cammszhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3muqgsrdp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ligdzhvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbnabrku.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3kunqadwy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3legjfrio.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3igyaoryt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvjcfswk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3qtvgezsi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3czvxwkps.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gilltrdd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3czfjivjv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfglcwwb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ayyltjzs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3tnkwsjoh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gcsgaiby.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cavppqty.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aopvfxnr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wlchavmc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3cqkxslvb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ueixhfzn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvcazuja.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3pfwgncgd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wojqlviw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cofhoixq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3obxccnlc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3asfyxlqs.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gvoxuzqd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3esvnfncu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rzwtovyp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3luhhqbje.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jlvkvbkk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ttqfwoca.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zpdauhci.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3unktpsos.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xyukjuit.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qqhpdiss.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ezpybhxf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hgzljzid.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mwvvbxtx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3skiogyqk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hosohncq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cfjrqubs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgttjums.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gzktihst.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ctshldzz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3sdwcbxyw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dlsqasnu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ekqmpxdp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rrnjcntf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3oyxxqlxv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlxnompc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilrzpefy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqihhjus.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3owmsxena.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ozwssgis.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3vodenjbn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3jvstvcob.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3njwfsjgt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xtjyovom.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3sgtjvyxs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zeomlizo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cefmycih.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qbtqzfvl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zerjhexj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hvsdeuom.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xzuygfwv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3iuqujlrv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3aipkmghq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3joupxmly.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzzltswe.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3udytrpfi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3tlwqaejz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3pzktsvrc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qbggvjpu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3inyumjzh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3hmcvrwgp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3dqyxeazq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3pxcatakv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jzaitsxt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3peowhfyp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwhpijlj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3nttygoks.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zjvsbyvl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tfrdugyp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3xomhazta.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hkzuqupo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dqtjywxl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zvcwcooa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jjtefjkc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hnwmgypr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3qfnptzgr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rhuqnkqs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3emdgqvpu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3nuwnljew.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qljeivpf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oimjlltu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wyflaeey.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vztccgpt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uwkcplbk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3avjuqbph.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3dbsfnzvm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3zdbcqmjs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yvgztour.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qcgzbyho.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsbgiyzk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3occsvzyr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyoiiqli.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lycuhdwz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qcnmstvx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ukfpmist.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mirsrouv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rwvvrwgt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wbwfsjem.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wvzsghuf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ojunwuqg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fdtnjzpl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pueirglq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3cidranpw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xlmqebql.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3hoxgrxwi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3olabumpj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3gimtupvx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ggjseilz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3otxnulkc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3caqtlnsn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3xklqsnqr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ipfjehhf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3dljxvheq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vognpwgv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eznmpwaw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3duofwmrh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yreygmqo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3uvloufho.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rnzjhbjx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3pbumtbgp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ggdwpkfp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3sawdwbvc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vmawozsg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3hivsxfzb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zfkikbgh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3liktztmj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jdzomtll.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wafdnugc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ldaizugt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tlkgszzt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3tkjsflwt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3unatwtxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iiztyxat.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ljsgkubm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3deidfnyd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3nevtfrgy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dnsjyytp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajdnctdm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pnrwlozb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rdtphtqm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilgtrozm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xptqwtcl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3geztssjd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gqzbqehh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3czxkuoib.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3cwcpnznb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3szronaui.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvfncyys.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3utjmtdru.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbdmgsgi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3rnlafqti.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3cdfbjliv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3whaqllwz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ezpvlpsy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3zzwfttkb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3moifemwm.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xlwogybk.html


<!-- 参考信息 -->