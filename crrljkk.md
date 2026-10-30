代发 wailian999

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gkatinntp.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gkbosofta.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gdusfwcha.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gckrbpfvb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gegwqwwjv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gqghbjgwj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ggwldjaip.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gdreunglf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gyvovsgfb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/glttdreik.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/giltjusle.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gwsktrmuv.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gmlnetron.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gwrvoggjq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gqfwvymqd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gshyftmdq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gihzmpxcq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gdomdimdo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/garrrmsmt.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gokbcjhyz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gxarkrqug.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guqlkajef.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gnfpmyhvf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gysvnygkm.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gijwinmxh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gbnmuxgbc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gutzmsgif.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gcgzlmtrl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gfkrgsohp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmcfnqwgy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gxosgcejx.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gufqufohu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gsysjjvzf.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gucpysgrr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gxosdbgok.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gzjmqvkru.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqwqtvvhq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/grglfslvg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gzuosnhpx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/ggiztfnuo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gmprdxqyg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gepdlsnkd.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gjtiikcej.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gpjeqyunj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gygqiasiy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gxamycslh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/glsdzioxo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gfblgtnqi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gzknvltot.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gcbzbcvxv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gvhgjbmpn.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxqzplezt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/guqtlvuud.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gmztvkkcf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gxpdovsah.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/grjnmhxki.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gofiisecc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gmhctkmzg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gexqsyunk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gmpgrmack.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gtgwcwblz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gdelcteor.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gygdwqdlq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gugzfxbsz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyzdyeiqd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gszzqyrcu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gqgzherxe.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gnmnoobry.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/grxxocehj.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gwmwscjoz.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsemvnpdw.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwppgvprr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzwyfeoeq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkuisnzuy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gwnaxqeob.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkakmrjpr.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkuhqovxo.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gijamwxcl.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gbjyygatp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gvzmepsoh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gykexyxcx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gsnhtlqzz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gfxhzlcmx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gklswewhu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/glkqedtdj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gvwcfhlck.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gbaporaag.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gjsyueqgk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gouvhofyr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gygsdbmoo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gkgnljdmo.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gxifajlhg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gbjepzmer.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/geybfgihm.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gawfxuyvr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gcrfxxsul.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gotaerwsj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbuownqyv.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gigkuloum.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gdpuiasuj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gixfomeam.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gwuhtmxkd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/guvhqcapc.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqrznpqzy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gnptviizc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gqqnaebnz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/giwelwdvi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gqeijsori.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gxcpipooo.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gemwvvnfl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gpmcdbsps.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjjaznffq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ghleaziem.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpabzmhdg.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/ghldwxmqb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gxrfqtdev.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/guwsnsque.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/galolytka.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gzhqndjao.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gfswtaluq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/goyfuqxyo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gkpngxabo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gfndirpmc.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gprlmlnnr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gqsbihyey.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gnrfxrwnj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gciegncbj.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gtruebwdr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gsugslits.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gqulogtbr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gwtejsxyv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gwoxjoryx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gryvcgfwi.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gmworcrsn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwifudgvq.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/grzundhdo.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gooflewgb.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/geqjyfgeg.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gvytxibzv.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gggwnwiwx.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/ginaizpoe.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/giaaafsdi.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gpkugaixk.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/glphgpnxu.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gdezeuzgb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gipmiickd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gngrtacup.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gpflklhou.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gglvamfoz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqahcuvdj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gwgookoub.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/ghvebnefx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gwfdeheat.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gztbqqiyl.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gfzdxuemy.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gudjzqsnx.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gnscvahei.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gvoasoxzb.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/ggekrrcvt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gzdornijt.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gvlmjregi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gukhgoehd.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gjsshhuye.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gtnjlzada.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gklyqrfjl.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghwqwaewe.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/grdygqhno.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gwcsllcta.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gngoxzyqg.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gnyymmmgb.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gszeqilhb.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gtejbczme.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/grcskvnms.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gtegmbnka.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gualdajdl.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gndtxfruh.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gcjankrqj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gakuabvvk.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gggpyqqjk.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gweegofwi.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gtejgwxaj.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gerudnebj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gvgxoclsk.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gybqtrafk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gnstptnow.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gqxtxaehk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gjqakfhfi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbmqdzlwf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gppurjxnb.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/ggbakzygu.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gfxcxuihb.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gtafchwau.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gvjlbecyw.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gdpkpgzpp.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gqzecfxhj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gsjqtiyyt.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gaihzpksd.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gwfzfbekl.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gmuwsrzoy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gsgaqxfef.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gjemyukla.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gkhixwryu.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gomhqevqc.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/geaveanju.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gzxsbidof.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gvhxtcqih.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/guobedaix.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gdaqdtksr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gifxiturx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/grmbvdmtv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gvrvfqmyo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gzcavwktw.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gdfkhrdhr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gbcdxqadw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/guhqxelno.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gukbhyjfl.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gkfpsmdbt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gkbugxdbo.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gnsdeeshs.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gfkluaxvf.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gzwdvrcdv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gikvuunju.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/ggnbivmgc.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/giwyrzxqn.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gbqegurve.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gtnyfkttx.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/ggwdagbuc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggkpivnye.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gqxypmrdt.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gsanipmbo.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gikylvwvg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/ganhdhfzs.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gxmiezuje.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gqduuahzq.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gqqjtptgs.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/guefscdks.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gayhhelcj.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjlhaqpgm.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gkwclsjze.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gcuzqlpya.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ghjvizjqd.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gchqxllto.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gsdbzkfci.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gsjmspdss.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gfodombbq.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/glrhpavnx.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gwxtfjyet.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gzdugieit.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gypqnpbbc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gonpyezyu.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/ghtkwwwsm.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/ggaxfpipt.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gpftnbvsd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gfjstxgdv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gwvawlpve.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gjzfjluch.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gmwgvrenk.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gaypvkscw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gzvleyife.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/glnowzkfm.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gdzibzkms.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gdwxkpaqp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/grzslmpsq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/glkvtpkce.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/ggxhfcvio.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gjykqehzn.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gvqshegnc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gllyvbdnm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gmkzsbchs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gsnsgsbsv.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/godhaapzw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gikxrhatw.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gaotpvivt.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/grufipgrw.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gbamktefb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gonfezgld.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gdgacixfy.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/ghtmwkcle.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gfmgyoqyj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glzaocqqs.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gaitjdwhl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfdkyhbdh.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gmhvpfjvl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gwcabpzsj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gxkvwbmaz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gflvgqxeh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gculuwqba.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gziedqiul.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gxudntgqv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gpokxlctu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gjcouytys.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/ggtqiiwwu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gvtwuuazf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/guyafqmrs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gufqtaxrf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gidnacxis.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gnbfbnyst.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gmjdrlupu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/ggopzjdsl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gdapsidam.sHtML


<!-- 参考信息 -->