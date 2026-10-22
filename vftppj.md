代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xitbeekq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2msibaukj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tvsmtqfh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jdfacqyd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2skwposgk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2onxojgom.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nwjkavhs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qezmcfml.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jdfndnza.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tpduzvhy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rftzsszm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kzoezmar.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xyngqmxq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2affxpeez.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ixxmtiav.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qfwaxouk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pluarbxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pctwcgqc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ralahxzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzjlnldb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhtqfzlg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2pffwnnmt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rfuhlihb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ifyocgxk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qjbujjyo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yruksyed.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2klrbrmdb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rliacpcn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uotxuwvw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2chtywwgu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2yfyvqwuk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2gegeckow.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yicrhnlj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2actaeveq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kpqztcfa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uyazlpub.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kzelbluz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnednxbq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2yieahijq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2nojdjmqz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zsqsnuzr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2phwwxixf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mtpoxrej.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2widfrvbg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ssjzpjoq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2bxqasngf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jolfigrs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrboiqwt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2chuusllw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ocayvdwb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qoifthqh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kodwbtkp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wciobmmi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lsibjzyr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2deilhgwo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2kvotegbv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kmprndjd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fswjaqhq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dacqlfor.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2emzdipje.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wtlulbdt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2syldjkxu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2owkoejkb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hxsnxfir.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2afkbqbzv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wezsqzqm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2alhgykfv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2thhpmppv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ilzlfjjp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pzlfyvmy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nbgqjtlt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2szooaton.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yhfhivvq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uuxcflhg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2lprgmtzw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wzlfbzvt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gfzkyegi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lyqumprt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lvdelccp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2uaksbsvl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ffjtjlly.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2euzvinxi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ikulrccx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2tkuabaha.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2vdpnzpla.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2llrhyuhw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wvbzabya.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gftdplpw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gvaophat.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yuroroph.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2cdazmywo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ydjupyya.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2upvqxodu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvzjfues.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pzgmtbmu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vbuctpjp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yvprpscx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vjzxeagq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2udriedqh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yyxkfeqb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zhxvsiif.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2esfnospd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sxxixggb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xkpojpbx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nodxfwgm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mxipwtpd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2acwabzkk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2snuemxji.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wnvzmybj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qnqauxrt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2nukqkihz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2onznrkmc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nqiieigj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uqzpyici.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abenokvk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wbndcmip.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2cdfauojx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pnbiguzf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2uejbfxyk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rggychwq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zicsocng.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2swagfgtj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qnqjehtv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2okvkoeio.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rlbyaawx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2tjsxtufk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qeaxccpk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2dplpqcah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdnxymkw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2vzwdoeiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnjrtiqp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qwhgzhfq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2bqwltask.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mqbnxksd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxepgxul.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2xyfvkphf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ybwtwpms.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2cbuqiwii.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wdekqhhm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnlafdsj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pstsadew.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qzkdujjb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2onjllxqv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xngbzixj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqcazzru.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnxxhlis.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kvmitkhn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2odjhsqos.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mxwzvbbq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2atzsiuae.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2aatumnyk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bxbtzkza.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wpicpgld.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pvpylems.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2mqxrsnys.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2pnhlsevq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2byljcabc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jobwgtlg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kzvxixxj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xtpzdnfw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aoimozif.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yrgqallc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pljfwkdv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eagjalzq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ngcvnrvf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kiskhhxm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oupbghqg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kajygtkc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2odwfxesw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iiqbntlx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbhtjuov.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2btoeqlsa.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gifsdzpp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2oqeiqgyw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hbdklsyt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2scefzkeo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jrocqejv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2dwomhmxe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2upmyimhl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2etbntvmy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2efoyhjwe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2khruumrc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2pljvxnqx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ymsrkolx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hnncdmby.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2pxldwerh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2vauliyzw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xvnaziru.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2edbhlcjl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vfttrckr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kcddgzkc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2cyzcibut.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hjimyhbg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2xghekopr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2jwhbkqzl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xrsropnf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2oprepzsk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2zqsiyjgl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2qgbujara.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2rofujrdj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jnouksnu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vlnasecm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vmpnrsda.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xlthrmsn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ltkclybj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwaipusj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2dmswespv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2osniucvf.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmaftlce.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2knbugwpn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ujezmahs.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlybxysv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2zbzmwykj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gxaadvqr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gptvzcus.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2pqtrgmqu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nkthljrr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vplzdgdi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2smzlumyt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xsooghie.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wkhifjoj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2steqptmz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2wpummorm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eumwbmjh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2afpcwumt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hzrzxnmn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaviqdti.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dvmdczyk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2amkwqera.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qvlawqtk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2rztlqvum.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2izpifqiu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2quruzzku.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwtpjzij.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xgqozrdl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gondfzlc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hmzjnabc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dphlmmkz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2duovnher.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2tyyukras.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2gntjqukr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mcenebkc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2btnslolx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zdfahnht.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rmcwgxai.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2prgbiigj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zkrzimed.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ogzqltdr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ohfvwncl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ephjzkgd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2llvshhug.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jkypmfrq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2cduqryir.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ziprgltw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2roqtcxme.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vhllhlby.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ralnbiug.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nlmwqinw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ofoggxei.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyrwrbqb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2furwrhua.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uvqxpfyw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zrskoiby.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2zmroupmt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2bzxscava.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ginzxqto.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2fwcudhrx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rpbmqoeg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2lyzlatgd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wdqhrrnj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nndsthii.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jggrhpop.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2jrhvatic.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2bbofvlum.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jyesoaey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfuouznp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2trxunueo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxdrmjsp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qvrvllda.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2gflxkcsx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2mjyfnhtd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jmxcxzin.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjwwibhh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2anhycvef.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fxjvrpja.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2vbremsiq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2lcpyszrl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ylvaflna.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2vlcfjkyt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddlaszif.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fncjrzhh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rbffwubu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pmdlwvfj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2xrnqjoor.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ufrzsktb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2anmnghem.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fdrorxxp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2jtcczabo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2obepdzor.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2crpkyfje.html


<!-- 参考信息 -->