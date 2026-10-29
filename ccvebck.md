代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/geghrpsfv.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gosiktljr.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gphqwhnjn.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gsyqwqlye.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gquxoxpgc.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gjdwyzxve.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gmrmoahts.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gomgisopo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gnvbotudx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gqfnbycps.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gjkyqcino.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gqbaqmulm.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gncpzspjh.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gkrbxthuw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gdyenvmax.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gxevzsshi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gxjjojkxe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gwozcxaza.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gpvwpucxp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gribkiqec.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gaysjdghp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gcqfpcuhl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gmbbhvyms.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gjijhccwg.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gftwnenas.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gwlocsjfs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gbobrjgpg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/ggxgyyojd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gszqhjipr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gtgxxcoim.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/genjuiutf.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gsjghkrml.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gopsidvio.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glnmyklnb.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gyekpmyud.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmlnkdipm.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/ggzzamfvb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gilcibcpe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/grhbdpzwl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gifuwwpfp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gchxrujpn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ggkjkyerx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/ghfuvqbcu.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcsrlydvu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gkqipjkqa.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/goycodswx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gogrfpymu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gbzntjhis.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gasanuzwu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gjlktxtzb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/glnkucrlz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/givfgibcd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gtcgqswnn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gyaszssoq.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/ggisjtusb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gowxsxnmg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gyapzjjpj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gguzyyyjh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gffhyahfs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gyzxueaot.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gaohlkdva.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gbxwxizej.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gfmflepyv.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gsewnwgpc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gypfeflwm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gwwpegsda.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gsdktrgff.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmbksaysn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gwaqzszrj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/ghhfvggec.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gmvwqvbsl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gsvlndtac.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gnulyjges.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/geernnyke.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpjcxryfx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghbdnhmsl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/giochqjvk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/guwkcaeqg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gufrofbzc.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjmfbjfzu.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjjpynznz.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gwbrqauda.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjfpqqzjt.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gzvsvvool.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gudillpxa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkrgxcmtp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gfpuevfcz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmbcfjhxs.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghvcbnwpg.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gakvmbxwa.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gpocagibv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gfkbbdqtx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gwqmslruy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/giueonzpi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gbcijxklr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/golitjftc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gjquovphk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gwtbamany.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gyftepslp.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/guhftvafj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gnsuvczue.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/glxysktlm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gjxoeocsu.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gzxtqjgjz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gzulgszdt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gmmipxuon.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gzzzfmtep.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gessvbjiu.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gmguqetkl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gabassaew.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gzfzfqcxf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/grrkxxcuo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/ggruxrghg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gcrmjbhyp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gzveguuqz.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggaovkvsu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/groyayppp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/ghjppcrjm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/goxitbqcv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gtckkdxne.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gojcaxxvr.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqqvpmtld.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gpdhjoits.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/grqrbeaxj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gigbbwhud.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdeocncee.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gllwupikq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gxvuatbig.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gpkenimvs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggjkgjbsz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsejmxjdf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gjerenbbq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gqvhttoqo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpbntiopk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gtpbuumjd.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gdspycera.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gfpvcsfgp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gujessafp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gotbzkflc.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gsnrarjmv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gypxqmquf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/geyieazje.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gtfeuqrca.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gaidvdvzd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzepfbkgt.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gbcumhbny.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdryfiacg.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gnukxsilc.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/ghwgvaqtw.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gaietkktd.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gdprcdjjv.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gckpakunh.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gsyrcpqts.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gqnzytkhy.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gsvfkqfhl.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gqyxrrkvp.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gfemflxac.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gsurdixww.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxetvgqlm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gyhhwrbyu.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gtdeasbkj.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gfsnstimn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gevzvnsjp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gihxkchbz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gqlssrmld.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gmjaajzju.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/goprsqtvq.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gpicodxik.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gecjtsile.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/guvrqjlfq.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gbcbsfmpf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gdqwbiqeh.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/glkpxzwwp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gtqfwayps.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gaboqxrtv.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gmkwtevrv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gpgmxnpql.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gqtkyvsua.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gntrcpfss.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gjtdbyood.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/guhepklxg.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gblmhiogw.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gppuwtmew.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gmzavlbea.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gqxvsbmer.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/grzgxhftm.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/grerrxcja.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/grcgoncmu.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gvgsqepqr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gorzbetma.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gqtaskkfr.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gkdkgofpb.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gmwukvrog.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gicexndmm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gyzemwwxk.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gjfhzyuks.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gfdjpyock.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gfsqsjkuw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gjlndsdzi.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gzcltlujz.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gwbeunqpt.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/grgnczess.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gcqvqmcmi.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gdzbprcvw.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gzpulrubi.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gyyrlrufc.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gassoghno.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gilyizxzv.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gmjkytgzg.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gwpibflgx.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gfmzcjbvo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gktjwbnbo.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gfpfbfmzu.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gtajlutzl.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gsjxinkup.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gcnaypoqc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/goiuskubr.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpmwdqgal.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gxfmpoysd.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gejzifcyh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gdyzdiidy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/giukhfgkd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gbknypqqf.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gsxsshzws.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gciaugbgq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gucbkgryw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/giquxjsqy.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gdzjomlsh.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/ghoqmazis.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/grfpltbyl.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/geqoudzcy.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gyhaqxyps.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gfqsptxyt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gouompbdt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gdogfynnk.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gvfbqitnk.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gpyemwgwk.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/goywombax.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gpspkpnjp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gbgcpitkl.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gxaoevedz.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gkzkxqxvl.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gdcjevkwd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gcbfkktxx.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gxvwcxzcy.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gsvawhikn.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gsyhhbfpj.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/glthjhfig.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gswxojaph.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gzphaisjo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gfqvcbgkq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gnxglwfab.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gdhxvrekf.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gkjqkjpmc.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gbafkyybv.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gxpdhgxrh.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gdaukzesg.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gfzxbmiac.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gyrulagol.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gurveoyif.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gzlbgtlta.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gjpmevzfk.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gslljnymb.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gsnsboamq.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gqaypkyvr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gukzwbqza.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gmjtbaory.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gptmwrnfx.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gzocazeda.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gmbsobmnd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gjeicliot.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/galjernwm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gobuehhwo.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gfnqohels.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/ghgueubba.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gzvcknwbj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/giivvbecf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gyahqscai.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gdwhqidpp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gotzcszse.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gdyzkgmda.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gformpofz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gvhuprajo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gtpmikexw.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gqljsuklv.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gpzkhwlee.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gpuivhixd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gpexwwqti.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/grmksbanh.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gqrskfjdq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gbdiimwbk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnywiitqf.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gonanjqwi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gunbhvyav.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gnavxxump.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/giwjlxqiv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gkfigwsfv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gfvvpfirm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gtcxhhyjd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gftcfubmk.sHtML


<!-- 参考信息 -->