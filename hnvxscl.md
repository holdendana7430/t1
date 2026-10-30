代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/ggviephba.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gugnuuyfh.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gwabtzmwq.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gpzsbgqca.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gelcyiiml.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gdhmcmvop.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gcbwjavbj.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gzipiqxic.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gdvwyntay.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gjczikssb.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gjiuurunv.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gbnzkjbao.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gzkghtjze.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gslkkrvgt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gsppbyijb.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gsfgzbigj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gpfdujbpo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gqpebywcr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmwpctpqm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gbxuuonhc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/guezdqdhq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gaqvduoyd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gdlhrqwdz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gmvzuefws.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gtecrgamu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gdvsvbcip.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gyvajdkwk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gzsudumwd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gmfhoyirm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gpvgungwp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/grvfuahxx.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gncovdstq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gmcuvrpuh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpjinvgbp.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gebxtykxt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxqaujvzp.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gncybbwkb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/grmdmebyi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gyqezdhjm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gcwvsylaq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gpszenjrr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/ghewviive.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gpfrqccql.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/galepkdaj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gvxpwusmx.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gmuvjtbvt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gaebclwuy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gedcwqphw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gneapefcc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/grdbuzdkv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gfkmcniwt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/glswwiryb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gihrpspsk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/guxopurgi.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gnhpmoggm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gtofchpyy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gtwmxwddp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ggovfgaoz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gbpnptnkf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/glugdsvwb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gagnstpwj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/ghpmstpbr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/girojgmrp.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gmidhjvjt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gqeswynlj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gmvwwgcmc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gaqexqhfs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gfyfqaaqn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/giekxvsba.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gwqtsdwjs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gepgmmxjq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/glybgxbwb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/ggdkmjann.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gafnjkpqi.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmfeqsbte.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghmvgqznp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwaajzxot.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gndwepqbg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gccafvimb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyudluzkh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfyniytoy.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gjqfhpynp.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/glhkebgox.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gakmvkcfe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwywxdzwe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcwudowue.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gwigsmcgz.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gookzvdei.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/grozcmqyz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grqtwbpof.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/grpjwgeck.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/ghwnohghg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gdqiwqner.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gljmirnqk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gfhaaevct.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gfwfbgjlx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/grnfpisbi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gtfnrtqqj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gxvrxmzfb.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gxgyqxjxv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gzlronlmf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gmoagowdp.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gnexoszya.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gprjemzav.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gewffrrkx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gbmvtinoj.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gwmstvfjn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gruilmwhc.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gbpzygudd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gixfnfmhi.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gugmbgvvw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/girvacaip.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gtwmxjpzr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gbwabekfh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gasekumys.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/goypverzo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gfmgedwcw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gsydoocfz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/grmdptbjb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzpbvdrah.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gglndldub.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gisgnybao.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gcvjfjgfp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdpcumjdp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcjgubkft.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwaaptiqy.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/geoolpqdk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyutqnzsy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gpvrzifng.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwnrhrhta.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gezmepshh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gbhpsazvk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gmqdqgivc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbrfwypsl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gjaumntnl.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gerpuagjw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gtemeulxe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gzizfszam.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gvzubffpx.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/giztnnjpe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gilgfimcj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gmqzjoamo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gvkmpcvxd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gdkerjzyh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gejouqemn.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gzwhnxych.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdcrlhhyt.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gtpdayaan.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gbwtxupcd.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/ghyrqclsy.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/grxvfnxte.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gptqhdprv.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/glrtpadse.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/ghrenktaf.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gpvbgbzie.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gisfingzk.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gpmdzmgnj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gmfbxstgp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gxsrunnju.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gnzvoxhti.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gatddipwt.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gkeikequp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/ghjnwzisd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gqnuvatai.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gcmrwucqh.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gkfdqkcvv.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gskeykqjd.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gtlbtdzra.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gbomhmzzf.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/guktmtiol.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/grjewtwcm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gaqsyzdoc.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/ghtqukavj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gzxtobazj.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gnnypotcn.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gysldqmhm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gctgfobfa.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjdajzph.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gevzwsakm.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggqcorzgp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gsldbdnoy.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gzxwzjyoz.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gdjagcwoq.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gdjhhlxll.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gkcweuoxq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gqaextjap.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/guznsqfmo.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gpwcfmlmr.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gcljlagoa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/girndfymc.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gyucgfawz.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/giibjxahn.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gbubiwnud.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gjmuoxfcr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gpnqtlrqe.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gczdtmsrt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gzuxjsmjq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/guaqnuzmm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gwoysppze.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gkdkwzjmj.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/glvcbriwy.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gkgnttthz.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gbooabgzu.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gsnwfzwka.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gefkmanfs.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gllzgmdky.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gkcshhnwf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gvuxmzfcf.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/greduduaz.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gwjisicnq.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gcdfbvppp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gxukykxgf.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gcdkusucp.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/glayxwgxc.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gbpfnauex.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gneuoluwk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gafhkojuj.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/ggwzcfwbg.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gqistlqsc.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gaijvsznm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gazosxsju.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gbntojolh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gytfaaqhv.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/guhkibeiq.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/glrtcmhov.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gthsjaysq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gfkpyjvzg.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gtqmnonbh.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gheiopkyd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/glrccfozy.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/grmzpyrag.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gracmprfn.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gpjarppdj.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gnghahuea.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gnjccdhla.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/ghwuksqmt.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gcdbrnksy.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gruzortvj.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gktuafmsw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/glvytbbdw.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/glpgcvcio.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gmakbepgh.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gzylifdkz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/grfkregwy.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gcpjbvqsy.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gpjescupa.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/glsemtytv.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gfgjtmprp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gkrissuit.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gvvrrszmo.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gqayifmat.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/geuqvlonz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gieuwoldt.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gcmtairmc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gyhdsfeae.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gfbmzzzzg.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/grianbilq.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gxcuortbc.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gmmzbdjvn.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gpbffzyci.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gqnegaeul.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gahwgdlmv.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/glihseuop.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gvgikogwn.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gsfhesxfv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gurpzgztn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gipryvwth.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/glinbodsp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gwslksfsx.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gtecsxuhc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gpdujgtkm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/grrhynacs.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/ghambxstf.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/ggdsozwij.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gyzdxkxnw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gczjjrgfj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gxjhnoxmg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/geetbpeaa.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gtrsppixk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/glnjdprgx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/giglnbmjr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gjyuruavz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/glatbloax.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gucqxaill.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gwohsxygo.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzmxjnnat.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/glfmaywmj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gkidjmenn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gvitdlyhl.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gljqxobft.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gdfzngynw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdavmjygu.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gbkwbcctr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gckbukqno.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gdnjlfaqf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gvbbntfkc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gbpwfgjck.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gosofqlln.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gxzziprnd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/glnfonofa.sHtML


<!-- 参考信息 -->