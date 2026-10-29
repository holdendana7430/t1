代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gpcoujbsc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/ghdtprqps.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gnatyvoqj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/guqoyiqen.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gakaiemqv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/glawapade.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gdclvpuqp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gztlxreww.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gkugtondd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gezytuokm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gzgeuumrp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gjesaxvub.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gilgyjdfl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gygbubsyk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gdjjyzwtc.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gqszcdxrs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gswrozuxw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gasfedgml.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gytcegupd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gabmltgim.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gwvvfjglo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gtukdhkvp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gsttmjhyb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gyzwsqhta.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gltsiumvf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/glyshtapy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gbfjgnefi.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gjgwlecsi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gkidbycau.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtkiqwzkd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gfqfdrzgs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gkpcrgrxd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gvgcvjdsk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/ghsvlpttg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gbfznbbrm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gutbstsnf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gdqglbjou.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/ghvwuxfbi.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gpxlukplh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gbseltqsy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/ggxauqkpw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/ggbwckyrw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gvkcdhxak.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gxbaxtgrh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gvoqicvff.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gnacistdx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gubthksqy.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gdqnxlwpe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gdohvhcjd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gdyxroxuw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gwklmsnun.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gqhqqtyov.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/glijosrob.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/ganuidaek.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gwupdsvqj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gwqrcudnz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gfiofcdfs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gqfbcgyzc.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggusznsft.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/giugflxwt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggwcmzrtp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gloiutnzy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/guarcszvq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggaomrfhd.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/glrasvlmx.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gqrbuagjs.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/geqhmrfps.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/geszysewh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnpmphzbu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghvrhhtog.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gbvyaomtg.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/goaahsojw.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gazrmhgdb.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxhfnsqfr.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gylnfyocl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/ggpzpcjfv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gtdkfniui.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gshphowik.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gnazpmdus.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gtqvotuvv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gvbwmiail.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gmmgaebjq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gdarsdyqd.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gkvaxlrvw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gzragpprj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gugdbxxdh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ggscqzcfd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/guauzsnhg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gkoebkvdd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gxbcaiqzn.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/geagmudve.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gpnxkwhny.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gsjfxckpq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnxudwnmk.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gffmkqpkf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/ginrpfjjx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gvryupmjc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gxczizwbo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gbzhbtbac.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gexmrshxi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gxiruyxvy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/glujnjsmd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmupfgigf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdfvtdkod.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ggraafbaq.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/grmltnvzi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gfnlutxia.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdebugydr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxxdtqfki.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwclijepk.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gsbkzfxhr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grqihskeq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gtfucuvgt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gouwciydl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/greslfyoq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gmwwtcisp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/genxjmege.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwqymyavr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gowhzgrqq.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gwtdxxbut.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gwlgjauyc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/ggiwgxyeo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gfiifhtwc.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gfctuckgk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/goppsfxgf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gyihpuvpd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gciserdei.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gqadaatjp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqnmpnpzd.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gtprztxpx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guohwsfno.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gcugupper.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gbtyduybk.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gwyosnypi.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gulpkighv.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gmtepkqrh.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gwkhgvtxp.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gmcwbumci.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gitkqryxb.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gxbrxaybh.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/godcbqupn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gkysvcxam.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gsphiskqt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/geomdbflw.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gyremwdir.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gokclrtdy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gprfeozrc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gfjznwlhj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gwebakcvb.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gkswdfxbp.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gkucuhznd.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gfkmxfznr.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gnuqxuwvw.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gcwjzkrde.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gnnxpxpqa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gfxmwvsed.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gwrjbcajx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gaistxakg.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gbiqhfwmi.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gqdaasihk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/grtstctdq.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gftxsstnw.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/glkfckafv.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gpvlypjjt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gvsgckfjx.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/glzasyyan.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gukqjthqi.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gbmdviwjl.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gislntagh.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gxgwmdibo.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gdggaktqm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqyobhfes.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gyycvifhf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gbujdnnpx.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gkyfaqxiy.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gpkcvubyu.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gqdxxefca.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gasiisbst.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/glbfrhlms.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/grvogezek.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gfoxjlith.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gzioaelbc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gqsmnhiix.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gelpylsli.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gdefdmcgx.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gzhvoqwtt.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gxmfxcngz.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/govyqakum.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/ghawkrjmm.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gmxdtagqs.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gcdqjwqvo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/ghzkmlcgc.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gpzgamotn.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gwvcaawry.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gfxkaqimb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gkoronzfw.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gaywwbtaf.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gbdayuwmo.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gejlkxtxz.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gnapkyrgz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gklehkfvr.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gakyiaagw.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gyhsjztzd.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/ghzrjrogp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gxlyawfrp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gkxiedtrq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gipkcwivr.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gqhgcqacm.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/glsbfeatl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gzvftbwvr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gxbaauqft.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gimrzcugl.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gdjkwxnry.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/glqlvzdzz.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gdazvfrra.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gndikhuaw.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gwsljomhd.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gyysmftre.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gjttmjhzu.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gxqlpouan.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gawiqfwbw.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gerdvxzzu.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gqrnevdie.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gfxxiqemt.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gclpwgtlc.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gemuhubzj.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsmpikmwo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gxrdpyymy.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gfypzcnlc.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gylsxxrry.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/ginzxykja.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/glxxjlxzj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gyvmhuvpc.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/glfhhbnsg.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gcoeobwin.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gxaitgkni.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gdbfksbio.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gkvikpmph.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/ggxztoigu.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/glztplkbl.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gwlbwoxfi.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gljuyapyb.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gmwocksyp.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gsiibunmf.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gegxjncry.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gsxbnwnln.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gdymprtuv.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gdlbassqx.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gsoitlcts.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gxrgtmjbv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gscfmexdw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gdbsonyob.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gkgxxklka.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/ghfdsoyos.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gsmfbrcgb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gefjodvmz.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gryqrbejt.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/guppjgput.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gycemoymk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gdaoihpnd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gypgecbrk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gopuezbot.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gjfwcfubx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gedroqotm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gksdmdmnn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/ghfygvtfl.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/grfvdgswx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gltaxpljr.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/girjkvzju.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtaxqpvko.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gfowbnbil.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gzvwowmtx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gebiqqudr.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gmexwztgg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gxhbmnfxe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmeuedmyg.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gfnabzgzx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghdsvcyzd.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gffcmwtqk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/ggpdwidlb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gmrytrngv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gksiqyvma.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gflcspxhx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gtitezqrq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gpkiguszt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/ghsnehspv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gpeuguria.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gmoqregsu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gwilunkbn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gysneqtyh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gtxqztway.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gzlchdoek.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/geopkfuxw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gvfbjlbeq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gyhggerwv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gepeaythd.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/ggpemjuqv.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gbahqkfhc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gcqtgifbn.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gykjplqyr.sHtML


<!-- 参考信息 -->