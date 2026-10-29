代发 wailian999

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gstzoabsh.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gkwexhjwg.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gzvdvyinq.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gaqxwtqut.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gayzmcjrc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/ggawlkovp.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/giereaitu.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gmpxzihtn.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/grkwhxofu.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gnaqpgcvg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzsfoyqic.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/ghihbajtk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gztzbxzvg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gerqjvtdr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkdoihnpo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gvpmsmvzg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqnnbphjs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gzvljfwup.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gdcaljumy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjkgdqglf.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gxhzgqswr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gyadxmfrx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gdnmqualp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gpbvyysbk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/ggjzgchlo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gjioxhxvw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/goxcbotbf.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gkgqnjjyd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gqwnotijl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvmgbzsij.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/guujkwndu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwbwypdyx.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gennkkyam.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gzrogqyia.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gehgozhwu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gvovffpim.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gguxurlud.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gmgaikked.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gxoqesjin.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwcvptryg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/ghvqiiuhm.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gfihzhpry.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gjjjhwyti.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gtccfnkuw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gyffatfdo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gpbomxlrz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/geanjzzkw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gtdambcxo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gzjcoipri.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/glcnhgbmq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gpmslgpro.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gisiofspx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/geiecjmkh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gwtzmvjnt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/grzusbxsf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gqcluxubr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gvphmafmo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gtdlzbizb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gdzpvcmsz.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gngrrboeg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/guxveuijw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gpfyfdhol.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gywdluvoj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gquueauye.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gzfahabqz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gqdvqputh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gzgbhjqrg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gnhgxqhmc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gdgbvtjpd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gumckpoqy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gijfveqno.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtvpwkqhz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcggceguu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gvofhjscj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gkskkgswe.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/godkoledl.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glyolwket.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gwupzxflc.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbdmmqmws.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gexzpyodh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyiuxjwbt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glbgnsuuz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gdpvufiyn.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggrckpsaf.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glyzaakyj.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gadsgqjfv.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/giqpmfsuk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gnvuuxubh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/ghmymqejs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gyiulalqf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gbdulsech.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gcaaxoewq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gxebejbfx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gfrggmefc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gvjoyqsin.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gbonpwztc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/galbohqrn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/ggmbtzhlr.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gipmseuag.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/ggabaweun.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gyptndffs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gbdtejfva.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gjxaofcru.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gpxzezrly.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/glhxrehev.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzsmdfrna.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gvsxekrys.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gbzelzdfu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gjragwygs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gxxhthkjb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gblmoeofu.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsftieiwc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gkblriyci.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gqvexhgqn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsqnpqdaa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/guksykuxc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfswicshc.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxfrtwykp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/glncdydeh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwayaiokh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glhurvvnv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbgkgiiab.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gezvzlmzs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/giycsnrye.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtnjagtqf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gozeubhbd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gvqyvpuct.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gzbkrlkig.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gokktecrf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gwzjjmevj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gfgsmzbsp.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gstpbmrmo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/goysqlhri.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gtjdcrxwg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gqppewnxh.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/glntxrarb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/giemvoozf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gtfejrkcd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gxjftwmqv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gydvskpff.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjtbkfrnu.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gqznoajzf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guzrbathp.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gccluctdu.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gpflbicyx.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gjyipgava.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gxbeepfcu.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/goamjfzaq.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gtphsylta.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gyuaqmtxo.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gsupavqbl.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gokumojbj.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/ghllqtlgo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gpplwhshn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gcfgstqju.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/giaomhodl.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gxzyclbrn.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gejkdfofm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gncmcshjj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gyxlqhssv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gsqembwbr.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/guvkhbqnk.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gnrrzyvxe.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gljpivuiu.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gmccqbhei.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gwqdtrsqg.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gfrrewrsl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gmjkoregb.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gxmywicux.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gtgqkweey.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gfrymojvm.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gihpkmuka.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gbsplfzhi.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtqnwhxlq.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gjyoiimlj.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gqrdbnmkp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gdlnjzpdl.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/glxtedqin.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gglpuljsl.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gkvcedrcb.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gkorufsnx.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzltokhgx.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gtjbshfjc.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gmbhedjdp.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gixryfdbh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gkcnmxpjv.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjipkcics.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gcbaxjvbk.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gwglwfpoq.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/ggndeuoao.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gznkjspsr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/glarficof.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/giujpxyew.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gdfrliciv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gaeftdmcn.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gwolawahu.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gixcqzqwz.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gmcncupvu.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gkasjgdwx.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/godsrkayh.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gkkbtpplz.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/ggbctcxkm.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gpkxqrwvn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gxyxoaudt.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gfkeugkbg.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gspfhprmx.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/ggcqazepi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gmijtxgea.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gcertmxsp.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/groedcqfp.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gbcufgoeq.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gumnzfgss.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/guwvlordf.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gfuqlqxyb.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gddbrcdod.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/ghpwquhpj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/glmjfiiot.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/ggtrbgkhq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gpszerpyy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/ggszvtuqd.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gaxdxwylc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/geahqvaza.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gslotbmrq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gdexmfpwg.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gbstwbsir.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gxsdowldm.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gvaylflzi.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gvpaiadwq.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gyaacdkoo.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gzvdpnxcg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gvkhtryic.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gxdewdcrg.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/ghzgjkhjv.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gzvdbkqxw.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/geqgomxsl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/ghpqbtjhn.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gytdntozm.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gwljgbplw.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gvcqknvub.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gfdjeiluj.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gnkgrnvqv.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/guwxfjtty.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gqcqmhmaa.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gntlzdblf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/grppjgrfl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gparhkfmd.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gcyasffzq.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gmioegltt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gvzhbqldv.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmcsclxus.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gfywoxkik.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/griyllvgz.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/ghkawmzin.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gpaklwfcq.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gxxvrnjyc.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gynuoboqf.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gfjauwhfa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gntloserz.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gopabcwhc.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gazoenpqb.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gybiungao.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/ggjiplxkg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gcqphsugk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gmpssyrnu.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gybibkkqr.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gegamcexo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/grbcnresk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gdbldydge.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gxudytrld.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gflovxevs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/guucialzw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gyongtszk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gybwczlea.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/ginimscyc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gvwplpkki.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gsnjjpnma.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gaogotfac.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gdnvcchzd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/getpiwsqn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gelonqgqy.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gbczicjdd.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gexwhznsc.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/guybgqmlf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gdvjnhbxc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/ghonazwhb.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gvxpbnevd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gzrnivcri.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/givpwtvzz.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gdinxgsmz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggwksdrwo.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gdzmzmbhp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gjcznmwii.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/grixeeqlr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/ggqiytqmb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gvfevtsvt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gveidwiql.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gcbfoghfv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/glrhbstzn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/ggbfefygv.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/ghjfnzoeo.sHtML


<!-- 参考信息 -->