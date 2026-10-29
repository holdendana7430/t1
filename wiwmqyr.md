代发 wailian999

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gpmymvlcd.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/ggacsysde.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gdgmpyysk.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gukxgztwx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gbchnboxs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gywelzzof.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gvedjiziz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gkxkhinei.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gsqocpbgq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gafcmsper.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gjcwynffl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/grekjomfj.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gwvkeehmm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gkkkqiagf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gnyfbxqns.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gqekhxxjk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/grhmxbxui.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gcpzhevvq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gpmcygyxl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gbtannuph.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/ganayuntl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyuqbvtzs.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gszqvgjrs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkvvyjtuy.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gfdtgynqd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gnmtaqkse.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/grtuodfnw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/guqkqrsqw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gbrykmxxi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/ggiljkxzw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gtoibuqms.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcicuihen.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gdvgbayxa.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gezlipxgt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/guvohgrey.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/ghiejofoj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gjjjmbhea.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gteimbqkp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gyrothkwt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/geunwccqn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gutgtcyln.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjkdtdeo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/ggxcdifxc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gbliiisgv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gkvdgfuja.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gmrtfiiog.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gilxnlrqg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gcxosjvrp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gagjhdztp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/ghjjvkbep.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gcyzceuex.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gbkmjsvvi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gqozesugg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gjyrphcmh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gzhfrngln.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gcmmsyejg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gsldpmvij.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gbgklqhhy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gwhecclsb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/ghmgtwfts.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gtjqxmffd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gseorifpb.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/geikwctvy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpsdxhhic.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbgkyzrkq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gxmysczpp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gastazxrm.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gicuqdurt.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gujnypcwq.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gytimvbiy.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwneggtyi.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbvzcrxji.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvbwrdcqs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdfagvtia.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gkvwquaki.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvyrarrdw.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxswwrnkf.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/glowfevei.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gyskrcpna.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gzxcfxyml.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gksnavpgv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gzxysqcpa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gmakhlrbl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gmzctkwrr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gkxaejysf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gqqvmjqhn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gepuevusa.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/goymheimo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gvtjnyvll.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gkqmduyvp.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gdekjxdku.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gucvkzjav.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gmrrsoizd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gqbbwmwrq.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gywdqeksf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/giiwqmjcf.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gnqjbaucw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gioiihvfx.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gfvzakjwa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gpilegoxa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/grfyzjeyu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gkwebawjd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gvgwpfagj.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpqanggtr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/ghnvcvvel.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gjrgxegkm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geerpyxml.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbxhquogc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqqorppli.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbjyaaomw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gyxojklnk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gbaojkmaf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxidgtjsf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gznqphlti.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gdpndwqtv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdvwembrq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/grkaeompu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/ggxpafcoa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gerathozd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/glrrynyzi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gvfujxfpn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gtlhytdiv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gebcboqdm.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/ggsyxjiid.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/ghhmnsuxx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/ghdssyoob.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gntkhrllj.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gbndkzotw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gqgtcxetj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gclzibgzu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gtucoqhib.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gxzikyewm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glqtxudyn.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gjbpqjtqo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghnplpyjn.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/geesfwokz.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gqppltlxo.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gjghdhqcu.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gpppyzfna.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/geymfythc.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gdleluvbz.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gtnprgpnv.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gppqllfjv.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gyfdgqenf.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gskuzhcdt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gozqttbgg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/ggarosnkf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gurgufpmc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gooqqefki.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gapihxxzx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gbnwkjxgv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/glnjbrxnr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/groevtdyg.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gktdxdxyq.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/glyrnbtdp.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gpasisrlb.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gswmhxdru.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gyrekxrel.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/grehnodqi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gjnlxepfa.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/giejcbzqu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gcgrifntr.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gdpikmvjz.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gshkkrxus.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gvlxlbalc.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gggvhzpzn.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gubhmutef.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gwdbuzqxt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gdkpcpewz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gtqjuqamh.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gecokgftw.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gmkqqbbxp.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/goyiyxeaa.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gymhhylla.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gpspzstmd.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gvxrjjanz.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gygpqnwew.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gpprupfnp.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gcwbevaha.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/grrqfqnho.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gspgqopsy.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gadldwxvu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gqesempmr.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gwcknetdv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnywevqbb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gpbmtamuo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/ghlljhyph.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/ghetqzjmj.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gazfavcwt.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gevgijiue.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gtuveqrfp.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gwlvdjpnr.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gminjeuxg.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/geygctuop.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gdvjodiha.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/guuymlftm.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/govmncenn.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gxwbptsgp.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gxyuepfog.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gwjexueux.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gkgkxoguo.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gybadnjhm.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gcklhrktf.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gtvleldbo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gjjyyliat.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/grpoxrquk.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gumihhtor.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gawrjmgfc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gmzjnfrva.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvnimyuuo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gapcntjnc.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gttxkxncn.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gdbpdtikj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gwmwvxmdl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gzkjqykxe.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gfqaoqhdx.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gdxojnamc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gvxjrjomz.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gwajyxger.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gyjpefohq.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gzpbxtrcp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/ggbyqoaij.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/ghlcukngi.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/genfuhdah.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gtajvsgpd.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gzriauqjg.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/guoopjkoe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gufolduxg.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gbhmrnqni.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gxckxwzjc.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/graykiokp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gznzstmri.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gnlsxolgf.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gyinnsqxm.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/glzscefjw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gmrssupjb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/geaacugdi.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gihbdcxku.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gxtezoovi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gyfltluco.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gpijzuyvw.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/ghcbikepn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/goeafpeve.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gaxqesxdf.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/ghoggpruy.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gaozgjaqm.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gnpafxykt.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gqtmhpiif.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gkkdaiuys.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gabrddeoy.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gujdamplp.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/goupnbjrc.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gwnpiztlg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gwpduvyrq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gadyhfkzg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gzmwxjexc.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gztytifwm.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gbugbqxqw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gghvlevvt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gautvisqf.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gnfccqpaj.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gtjcmswqy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gkbkglwpv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gvrbpgfep.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/greqgzxtc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gfhnvybdj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/grasflmgu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gbkoodoxe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gtizjorws.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/geehgnhzp.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gwxatxwwj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gmomboqfg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gdlvxuiur.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gtpmfgauu.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/ghltdgpnp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gtzarbvzi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/ggejwqotj.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/glpldiame.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gvfdzflyf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvcwbjseg.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gzstrycyu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtquusxtq.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/glspauibk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gzlwwmkcp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gsdzrbfrh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gnckklwlq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gurkqajnv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/ggmzkltmq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gwscfldul.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/glbdyolvv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gokilzprs.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/garzjqskc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gnwzxolyc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gpjchqbrf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gdqhjoipz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gxampbymn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gbyxvsark.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gdodbmuxk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gjnfoqtgo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtzymawsk.sHtML


<!-- 参考信息 -->