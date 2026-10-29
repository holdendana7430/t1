代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gudqgtgkk.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/giooojlrh.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/glaufdzjg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gaaizslyw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gbuikcjkx.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gdqjniqmw.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gtaivrixf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gcqpnuqzu.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gdykaupdg.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gfhpcfgvg.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/ggrimjfdu.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gfhkxlrrn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gzptilfnn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gwfmrmwod.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gpxshehjh.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gerqmeezi.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gfencpjsx.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/getzswzim.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqbwsyrxt.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/guaeqypqn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gysjqejeo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/garzbekqt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gutjxavws.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gpgvleutx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gwwqyfpyl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/grivucotl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gqhkhuvcv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/grmhwsmvw.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gybslyrwk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/glldnwtlu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gxpolearh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/goueputln.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/girdmcdzu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/grgwzkwci.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gzjoaszdv.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gifpnhqbc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gaiqyvdvk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqskwrjdi.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gdlpazpgo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glyhpzdvt.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gfybddetm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gbswlnfos.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gyehlihgo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gguslzhjw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gydsvflnk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gshxdyrpv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/geebwoyyt.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkwygllin.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnuqietei.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gpzqwmann.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gdcebghcb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gmhruiape.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/geonrikwf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gvhracbff.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gfkeetqrr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/galozsdbt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gqtwbjtqd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gaxscecpn.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gylotyztl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gngeauncx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gvuaitssf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gktdalzsz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gxybwlyrc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gxspzrfov.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/ggndaptqd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gzdomfhtr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gpdwugqru.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gizjafszb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gaqmlmzio.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gqqppyuoq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gqygilgzq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gwdifcvnt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gzubnnlph.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gygmfajqq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/grrhiujzy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/glhamaydc.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gaukmfsra.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/ghbkgrskk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gmjnbjsij.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkexlrwhs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkhuidxfa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gceizvvaf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gkbkobucp.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gztuxjisr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gphsfakcm.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/giiszarzp.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxsbmigel.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gcgzezxaa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqaotxukp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/glgbqoppk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gntcwfrsp.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gixcormoy.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/grllbwcgd.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpnxurcuu.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gbnngwdgx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/graglhnuj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gezbsewuy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gccjudorj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gkurxsses.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gsvkwqkel.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gwohqxskp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gkihmgmfy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gkzcobzyq.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gcurocsqi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/guwnpgonz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/glefotfzj.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gnegktpog.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gzonzcsjg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/giuvzttrs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gzsqkdkxo.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gnnzkvogk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gibetpmow.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gprtowxid.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvbtyxoig.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnxtqvmyk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gouwkfmbj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/grugmpvoe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/grcqqbmld.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/genswzxre.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbdytpddg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gkuvpmolh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/grnraudez.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjhyukdec.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gpvjztlfp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gncmxrdxn.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gftcdwhlc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gmpbioplt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpymssuua.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkkbdwmnc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtmzgzhye.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/ghgdcjnbf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gvlbkermx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbmnucdjo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/guukmxvla.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gvfqafgkx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gkxpudwvk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/glpikctqq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghlvzhlze.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gfnqaqipr.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gsggutvtz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gnoocchdz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gnxvodxtg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gtygxtfwh.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gwltphsxc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gsvkulduq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gkqtuxdna.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gbtduwbze.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gwboqlhvq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/groqdnvcr.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gaqgloiuq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwbovarmm.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/godydkusn.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gnkouobdc.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdlijqaam.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gfrpfowub.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/grmnqbiol.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/glbuwrwfd.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gvesbnqsb.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gfvmdipmt.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/geuxxlams.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gfduiccdh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gofhbtmxb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gvasevgtu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gswgmlezj.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gwpfzwmtb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gfhzbckxt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gmauqxkfa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gudllbpxu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gferhuxgj.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gleimnebe.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gtbmbdjgr.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gomfowngw.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gmgfhbfap.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gqtbwankr.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/giwntjcvl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gzltobirl.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gwjzaxich.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/geqydvjpt.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gxvjnlnyi.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gqvrcdjjj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gssjunbch.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gsnwqmulv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gvssonqgl.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gohujwnmn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/ghgmfnpdn.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gyjloomvy.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gdvfbtnsw.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/ghaevejls.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gabtfnatn.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/goafvytji.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ghjituqdn.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/ghzvwyyvs.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gczewnnqc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gtphrwczh.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/glhozdmdd.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gpxazghge.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gauvfyyir.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gbjsorrsb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gonwmwogw.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gniozmfdr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gqlagivhi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/grhlxubyp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gmoeghybl.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gcjrxshof.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/glezvgfyr.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gsmxxmjut.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gaywmvpfe.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwgyxomuy.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gxmytatgv.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gpldutfgt.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gktrdphpm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gexyttgyd.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gujkildet.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/ghwutkulu.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gbbpyjwyt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gznvjjdhj.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gocqnrigq.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/guemtvbax.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gnlarabyv.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gvabebukg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gvyhwtftl.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gmljomahn.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gqylbpgyk.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gqvhjpbna.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gvplskgbm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gaswtvtyy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/guchwftqr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gaegstkrs.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gibmcgwbu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gkeggtpom.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gwnxutaql.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gvtbonted.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/guwvdplcw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gagophnej.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gwqcmzokc.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/ggskbjpet.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gttootfhp.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/girhkxjop.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gwthinmny.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/grwgcexzx.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gcqngcaou.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gyralncmj.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gayjwtuns.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gddgkbuvd.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gspqhhjaz.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gnpanigvq.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gzjfwlrhr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gkthuqezg.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gimddvbgm.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/grudqfwsg.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gmeuuqpfp.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/grfnwweuz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gvdwofhfb.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gebsdotfb.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gmrrkpqfm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gztzlnzch.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gghjxerno.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/ggusunpyk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gxbiseleo.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gifbfpwav.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gwwsmuwts.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/goisbufnq.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gthdftuau.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gplanvefg.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gxilcypxk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gwememfvx.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gfdyuycyu.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gqimlkccl.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gnmjmvfsq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gnlbutyon.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gpkmpatvy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gmmrkhsth.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gttoeduqy.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gfzygwomo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gewuiqkfi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gqeieoipd.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gvjliciad.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/geajlyeqd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gmllmlzvt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gfkkjjtee.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gzgwkbafn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gdnzhijhm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gwvpvugoo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gtqmbjduj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gmaklcdwi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gbkqfmqec.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gsbhllmhu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gbocipivn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gagkmwidr.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gwxllirsm.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gooxdfemv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gsrmdswss.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gftfwqsen.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gjtoydkjm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gvsypthzb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gswoanleq.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/grrsulljv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnztyxegm.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gsnldqcmk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gffrpvfzr.sHtML


<!-- 参考信息 -->