代发 wailian999

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gsrfzvprs.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gxvzomctq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gxpvhbsue.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gqyihyfly.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/grqjlpgso.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gtzztbhiw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gjjxxqvgk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gcpfqtpzy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gxhgtpgax.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gnnwgtbgx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gennvpqec.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gshrutylm.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gvigtrrnu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/ghitjsjsj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/grbfkhvyr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gjikdqhip.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghyaafqon.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gxeeddhku.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gaqnpwumg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gmfzrxfrv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gooogmbyk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwbgncmbw.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gaymzepnp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghdvnfykj.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gfnpdlusx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gzaancdpc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gyzbtptef.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gzoxynimt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gompbtgio.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gsmmqofhq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gsbufzndn.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjkpbbito.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/grktrmwou.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gklxzghnu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/grurodxne.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gdprmohxg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpqillazu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/ghvrpjols.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gxptzfdev.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gnzrkkynq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gjmhghzlx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/ggbotzxgj.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gdppjqxze.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/grqpycqiu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gozldsdvm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gnftrrarm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gpntwsowp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gnqjhkhvq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gmyaqwqkt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gncfmtcgd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gvzhdnwgt.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/guwnidzbr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gyidgoaty.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/glusofbjq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gwjzsyips.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/grldehdzb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gsebjqrye.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gjwxuioyl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gfvqvwpow.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/glydkkfsl.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gzgrvnbul.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gxxmgjwwd.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gizaerojg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvtcpcndo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghuevanqy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gtczapomu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gaorpwddx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkjldzlak.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gafedyawv.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/ggbrvoyco.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggnsshsii.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzyqluazn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gimecxrdx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gudohxosq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/ggmdvttsd.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzhnmwftt.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqzzhfcwj.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpgklcesy.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gibaphuba.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gfuxjpgvb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gmqnvaxqt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/glyljwrau.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gunrgrddw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/ggeteehgw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/golyzvsba.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gbxfpwdgq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gosgevgbk.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gjkxzngxy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gitisimfa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gaqatoogy.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gszumlwjy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gfjsuvfga.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gygeqvjvt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gihxugbjf.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gdunnutfw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/grgmywdcu.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gndatxzgg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxxnrtjwf.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gnyfahues.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gidmnktjk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gzhyvytmz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gcyxshjgy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gkbjsyrgz.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gntbnzrak.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gqxyngtch.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gwrprnevw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfsyvubfx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/ggznymqbv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/guwktiema.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gaiyyvfyl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gqdyffwdw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gazxlpkap.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfatdrwcp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwngijnqn.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gbscqsytt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfoubbcbj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gvczbwhkw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gowtkmfpz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gsfddovxq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/giozqgxbd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/guzdcwrxc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gkrvixdhv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/geqyvowdc.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/ggdphxkzl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gyaescrbu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gmegljqyr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/ghfqgfjhi.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/guyyezwuv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gaaybokhe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gixewqdft.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gkrlnrrtm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gkbtmvrtw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzivwqwru.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gyawejaax.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdizxtela.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gbttmiwfu.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gyodqpcsj.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/ghkpfkeud.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gwcbmbxmf.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/giezxjjlc.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gbeekpuun.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/ghkxckhnk.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/govttydpj.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gptenzide.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwlzbxdus.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gtivrhbhe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gotxbmpml.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gibyebayb.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gkxodagel.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/grondoqch.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gmuvbtyns.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcptcgvqd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gvzqlfflv.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/goktmdwbi.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/grgttexjn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gamdyeqyp.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gpxfhfbwk.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gkzruxnpt.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gkaonfcvi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/glxtgojil.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gazijlsub.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gsrulxybr.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gkjhlbirz.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/ggarkslpk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gbiqymijr.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqlabapzq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjfdqkmgt.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gfityijpr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gclpcabzr.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/guczeldod.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/glmwjfczq.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gxhnygtgv.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/ggpfgpujo.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/goihiygbu.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gkcddojcc.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gbjuerdtg.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ghgdvpskd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/geonuwjpq.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gehandrwh.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gsaamtzfh.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gskwywzxq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gunsrtxib.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gvrmrspye.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gcmhehdcx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmuaveaic.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gaaytbnly.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gdtmqsjva.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gqavmbzfa.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gpzcnlscb.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gnmqlvzqr.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gaskwbpnp.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gnuqrpncn.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gtsdzlees.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gapadwxbw.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gwgfxygrl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gvrwvoggv.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gindnebxd.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gqiiihuts.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/ggzsxvevm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gpjyjfqhz.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gvyejyaqe.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gvfetpnih.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gznbkkcox.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gtrnbubkl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gvermhezy.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/grzgvavyh.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gdwdotwwb.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/galqqprje.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/guwwszuwy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/ghrluxbiu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gpkvlthtp.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/glsjxqklr.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gknvqohia.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/ghaiochbn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gtdtobdqo.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/ggjgijyaz.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gidflznlw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gmfdlqsys.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/ghgimrnwc.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gxkqeljfl.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gfrdxyqev.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gefrvrxup.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gfvdvvjhb.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gdvsvhpxf.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/ggwarcssu.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gamikfvno.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gxtfctdhz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gbtuvxnva.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gbmkqmdzf.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gbiaphouz.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gghsifegh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gblgbsnam.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/grvdrzaxx.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gocmljexp.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gkawhbcud.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gaekhxpim.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gusyhnobo.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guwyxxnbn.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gxsjcqlny.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gieaeszki.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gcsncdfkk.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gwwncphgd.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gaactxqid.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gwzcigsvk.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gyueiwiwn.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gzroiqydh.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gqpmyxlcr.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gpnwimuup.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gautnzyic.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gfscgrghx.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gmzjynxzq.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gpyuxtnxb.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/ggophlmhr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/ggkpqiizo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gefphfujh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/grsxykbuh.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gxikduhcw.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gjrliascy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gqjkqvkpn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gcdgnlzds.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gangmpnfg.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gldjlbwln.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gzzrwnrtt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/guyjanjcs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gqpbzxmzv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gsdwmtzqc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gozjsjxbo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/ghnrlpekt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gcyjzefjl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gvdlxismj.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gxtxveqrh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gmalcqxtc.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gsloshsyv.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghqaonphs.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ggbsqvblv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gsorwgifj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gporpqpkd.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/goqhoygxt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gajwfbkhf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbfqpcvlx.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gvggllktg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsjgsnqpw.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/ganzalrgr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/ghffuvuud.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/glrcmfycq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/guqhkyxyr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gkjiyjylk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gdokmsuub.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/goqdyynra.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gmltleouu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/ghsojlixy.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/grodwidjx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gzszpbynr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gkdvxeiob.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gxxagdhhp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gemfqtpfy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gvtnngmql.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gbrrslzvc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gugezernr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gitcinofn.sHtML


<!-- 参考信息 -->