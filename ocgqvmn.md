代发 wailian999

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gsxmfufhg.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gcxjvngdb.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gjvlpwtil.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gwzuxirye.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gdcpcrljc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/grcobssgu.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gkqariuvi.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gjxqxvkvz.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/guafcimwq.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gvbvadqmk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/grnkqxvth.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gfryasijx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gocbntlkj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gcgcuwvav.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gocwkdjsv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gwqrjwlwb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gyqrhujzc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/golubuznw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/goiaryccf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gxdkqyrwt.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gpanegoay.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gdwoxbbzq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gyeittvlx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gdjfjazyu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gdvncglum.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/goidiklkn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/glsdzkhzs.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjrwwjyhm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gwnebohvd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goktdbtvb.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gyqzumgkw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcxoqbqrf.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/galsvuprd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/ghwrotrcm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gwebuertv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gommnreaa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gnidctynr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gmleighcz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gmrbwswil.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnlpamtgp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gaegbdvbg.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gzhfkivvs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gydhaecjf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gjxkulgxr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwevkxwhg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnduxyysb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gqispbpem.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gyvvooish.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gkaunzlgg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gzhgwpsed.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/ggqouiiea.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gmbtjvkii.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gfauekdfs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gsejstiua.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gwcnkyfgl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/ghzdocbcp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gaylkfjfd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gylmxxjti.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/ggvfeapmr.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gzwswmrmd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gknysjoke.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gyjtooigv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gbbeufbex.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gejhpugwj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gopbgjhab.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/ggtklvylo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gtppyoshs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gdqfzakyi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/ggipciqzv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/grezqqwfa.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjnglosle.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbltkpjae.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gubzogync.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gkvpcffmd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gbbbnwhiq.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gifqusyrw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gedwdqnkn.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gpcqdragt.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gehvkmeqh.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gcjgtzbab.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gywgfsrvn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtvelkdyq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/guemhllqq.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjjduqemg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqmihuvgk.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gaxggbbyo.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gtmbszheg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gfqejoezx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gmdvyexde.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gapkciovg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gfryybobm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gdgvocmnr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gvdvknwyc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gsdbfqnul.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gxrqsyyne.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/genjgalvd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gvkywkawn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gffsffkqw.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/glgomtnlf.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gdbjpbpje.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gqqxkpdul.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gdaoujlku.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gqvcvfxvw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gkuptifqf.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gchpfjyag.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/golalrdmf.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbjbmmpaf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/ggirkkpnh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gebitdayr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ggbsjzqqq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gkcxztpyc.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggauznynw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/govlfnfce.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gqmpktypl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqjjfmxmr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtnvolira.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbnqqvdla.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtzqituvg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gioznnbej.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyslietoq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwndqigia.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxdbqgxfv.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gebquctrc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gkllzyscr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gfspzlpzm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/guzrzgojr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmmrklyeu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gcccoerhn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gznzgsnoh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gpmoobspb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gddqlqmmt.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gejsdcbnk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gfvbkhvul.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gaumekpoa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gicffanvx.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gyycuaqzv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gzvyqneck.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gxrqnidoy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gnjzweadl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gphpabsqa.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdqtumgts.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gmvwqlhpc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggtzwqdcy.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gpaivdzef.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gotiqxnos.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gjcgmpinz.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/glpmkacrp.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/ghjktdjyh.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdpdbjlju.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gvhmktcfm.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gousccjxu.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/giarupjlw.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/goxtghzfw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gcdswsstz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gpwlwhdih.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gwgofalbd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxtcyiluv.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gzqyfvhps.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gsvwvwgfl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gbdaxzpxh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpamfcobq.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gangzsqbr.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gexyeaqgq.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gwthrespp.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/glwifxsvq.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gqlwpgrmu.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gavduqawr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gtgwzyxkd.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gqohssfsq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gsjbbebhr.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gmpkbvipe.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gcqfmtvwh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gbllepsaf.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gysutxoql.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gznyuoqbf.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gzixuwoor.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gsckodbhy.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gxrwdvpky.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gzmqxpfys.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gymlbyvjb.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gblnsefwk.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gwbkirfib.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gybsmovco.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gveujuhac.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gzskkliwd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gedtoireb.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gundogztc.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/givcwfjvv.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/giymfrtxm.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gvhhtpxru.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gjolsssqz.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/glppziymt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gscvfotbl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gdgpwsjep.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gnkiqszzs.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/ggvqedqau.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gedxfqtyu.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/geqsbwkny.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gftsdwrsn.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/girwoncrd.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/geqpwrird.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gayaqtdbs.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gtdddssse.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/glujotdpv.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gafxtklpv.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gtepprxmq.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gvcauuadr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gdooogdvc.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gqszohoca.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gmksixdnl.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gvywqaxue.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gjefgsbfh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gkxzaacwp.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gkhaqaehb.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gkmmiampl.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gkyeyluyc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gixicesah.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gbhkrhrfj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/ggqnfcipd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gloiuvaxy.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gxoecbgjv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gsxyhkbwe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gdgpjhafd.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gvztpmfse.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gbcnxtmns.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gdpjjxhno.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/glaxwsjsl.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gdqzvpnsj.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gmguevmdk.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gijgsfusk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gvvfnrkez.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gmivftgrk.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/ggpqsohbz.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gltixlfca.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gkvkfczfi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gdjpcghos.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gnfzslgph.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/glqfadiyj.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gwdueyclw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gyjpdezgj.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gcqvrpxml.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gywcoawce.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gqkcacjhv.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gytxribqp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gbkoggrhv.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gpnvntpoi.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gdltuawyw.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gyyjwagma.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gbzgqudba.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gvwjweajh.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gyltvcvke.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/ggcdgsqtg.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gxejcpbtw.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmenvoizu.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gdiuizwpz.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ggwwueirr.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gpvfsubiq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gitzmrvtt.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/ghfstmvce.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/glyvmbesk.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gxdgpbwcp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/getvwupnf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gesrvbxxq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/ggypqrcia.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gxdtsnlzg.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gyrxteqgy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/geopoijtu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gafinnfhu.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gmhuuhkdh.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gnjzmmnpf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gedktnxkx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/glldogver.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gubvbbcax.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gpgjuzjqu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gvocxobrk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gspxfyalp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gaiqxlnra.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gvpthbqca.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gduxmheuk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gntqswfcy.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gjyccqbtw.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gsnijktox.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gygwrwzki.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gpfqapwmk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gkkoedfam.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/guqardowl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gylppnobb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/greqhlucj.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gogvhjyth.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpiwlgfhm.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gqbvysehy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gvibranjy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gcaksyfle.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gojwmoxko.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gmidwdhuw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/guscmikua.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gprhvfaes.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gxomlkirs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gjbbqwyuj.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/geqshdvrv.sHtML


<!-- 参考信息 -->