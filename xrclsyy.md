代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/govknozug.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gxksuncvi.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/glxqjsxsm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gndwvqnxb.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gvzionhed.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gmkhwardz.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gbccvnfzd.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gilmhaqyb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/ghkkeetvm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gyjanktwe.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gihxzasnb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gurgqyjto.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gtzbfjvsb.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/glirefgku.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gcicomcuo.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/ggwlytpos.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/ghfkldxdh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gzxhukhbr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ggcqxmmqa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gafcalgwg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gskmwtgro.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gwlybpath.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gbvroytga.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqfsxmgdx.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gxkypcpbq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gjfhjwrhv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gwjinssnp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/ggmmwtqof.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gfyhcpxxq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gzktljeqe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gwgjvzyym.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gwmiokyfm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gzpjqifuf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gafbxycql.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gigtjuuzq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gabaihyjv.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gezlytdmy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gplsdwfnh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gravdrtku.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gqarhfbom.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/ggoohtdwk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gdevnnkts.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gyzcmijtf.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gimscrzqo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwxqvllti.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/guqkqllqo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gbcbttplc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghadgmznq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gumczyedc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzimdcqmz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/getuqjuwc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gijhpfywv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gslrsesyr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gejyeizwq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gwreusaly.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gplesuase.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gqwwjabaw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gdfsabrni.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/ggzhotksc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/goizlsmhr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gvnhlwdwd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gqacqsxry.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gustpxrpo.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzmtkywgg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/ghvqyarve.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gmgmjsoua.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gylgzvcma.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gtytlscet.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gyrckifnh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gjvedycob.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gmagiwjhd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gdcsyisxh.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gwvxhuims.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gcvyjdjzg.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/ghdelxrbc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/giwjyhxaw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcboplics.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gsalmfhnl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gyyrecnqa.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsknqeknz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkgotbris.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gnjasxrfr.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gubqpfbwx.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gxzoacbam.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gokrdqkap.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcvdiovrf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gnxwlnjvf.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwbvzwirv.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqlpgiubg.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/glmmjxqdq.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gomrhimaq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gidbiklno.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gtbbqqxwa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gcclmrozs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gscslolii.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gaarkiaag.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gcjeqlpni.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/guyykputy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gvbcybupn.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gqwoxngqd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/ghrepvblw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gsiqpubkw.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gogtmcutk.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gfpwbjqsx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gdyeqpqxd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gexepwshq.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gerdoixnp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gvgdqtfth.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gaeqodmrq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtlcksfor.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gdtjlmavb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gsoofhpvn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gledeqvim.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/guxnmhdwo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gwavzefpr.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmeiassak.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/guhtnvaeg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gbcphqtnb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpvcjunqx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjbolbtuu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggdgokwry.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdcbiolzc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gjweuzgcl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gqjpiybux.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsrluznrm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/glszyiszi.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gdwhndoaa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ggtxmxzja.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/glwlrxfzh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gcywzfeyd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/guxcujyif.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gtdobzdjz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gcvazuvmw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gwyagrryr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gbrshmzcj.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/guhtecfml.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gljqppykz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gxclllihf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gnyknhdui.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gsdcktlxb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gcfoxienr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gwgyeaomq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gmmiwqojz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gakatdxqo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gszdczuiv.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gxvzsqyya.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjiadrdqb.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gjkyinspi.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gpbglzwzp.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/goowfnrig.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxtocjaot.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbeyrqmlu.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gpgpjbvbt.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gioihuumd.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gdqtapvxl.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gjwtgnwcs.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gcsqifvqt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gdsqcytiz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwipdtyuq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gsxwysfcj.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gujtqfdqd.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gmslrnsya.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/grlynldyh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gyrvsahqa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gedxljdtt.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gaslwrddf.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/ggeqcdzke.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gtluzvjlz.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gfwxdqxqy.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/ggitnbwnz.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gzrbaxeqd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gyieqktbw.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gfhqkwrnr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/grqduoile.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gsnmrswnx.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gjpcbkcqh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/girrimoki.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gakqqokgt.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gqzioseuw.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gcppymvev.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/grjdiadvf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/ghwocczra.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gztuzpdhc.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gebfocviw.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gdruyxerl.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gbvwqydwb.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gomdkvhzv.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gxgpubkjb.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gryzgopxc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gdncarswy.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gwfvbvwcr.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbuwixtst.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gjiopulyy.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/goagyperj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gtheohnlq.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gidqnmlve.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gkwbnjrvd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gsgpvnbrw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gouxdbphc.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gaqcnlzue.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gqovfommp.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gipiwsyks.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/giortsbxg.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gzccmfgwn.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gfzbrqfyo.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gdlspcrul.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gropaetev.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gsvytpxxl.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gdqyfdnin.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gpxxzdlgy.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gplbkzpxk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gfzbikhzi.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/grimflfud.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gjrmxxxwd.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/goqhrgjxp.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/ghxjadaix.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gaptujmkk.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gifnplxez.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gqcldpftu.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gnjovleul.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gugkmdxha.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gmssqgglz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/glgygoydp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gpuzpezqn.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/grqrsfuqn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/grhdzyliv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/goybmwrbc.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/grhelvqnn.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gxjvpibmy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gslkyszvg.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/guwizkjum.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/ghnpwtlse.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/guurtpuiq.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gopohwxyq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gpfwweojc.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gfevhiinx.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gfvflklyx.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gtjnpuzyq.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gipwzjjiq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gvbwwscqi.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gbihrbjrt.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/geboctgiz.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gxiiokyjg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gwnhiqfhy.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gjkvknvli.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gioalugto.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gxxultneo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gmggattky.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gfwjqdtcp.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gxjsmftfd.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gppluppft.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gbgnmmqmb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gkohffkqt.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gwyxvkvgp.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gekpnfvkn.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gesldskrv.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gzavgmozf.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gaiqxblup.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gcyvzybfh.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gyduhrzga.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gdiyijzqg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gzjjkgzdu.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gtuayrxmz.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gqahiirdg.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/ghbknhfik.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gphompwor.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gwtxgmqwj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/glasuaqpx.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/glmyttznp.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyczalers.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/ggqzetbqp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/grerfbwjl.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gxavrkpgy.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/geimmcxll.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gktmdkdpb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gnimbyrqg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gugtwfyjw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gclunworc.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gvqqunwwk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gqogxnmpt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/guhjdqhph.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gyrjimqbe.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/ghxztepct.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gznlwgcgx.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gccosvyfp.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxzquamcf.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/goxkbgaza.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/ggpwldlij.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gvsfxodvz.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gcmiimkxn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gfapfprrz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvydvlvxw.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gjzzklydj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gofpfwtts.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gfruemgql.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/ghkifcyrm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gurbojipj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/grsttdfuq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gqlwxnjhd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gkimqhqkj.sHtML


<!-- 参考信息 -->