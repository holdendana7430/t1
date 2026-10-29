代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gztblftoo.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/glmfnmifd.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gbjtbeqjn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfdncwvkf.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gbvyciucl.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gcixjlkoq.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/grvqphmeu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gslgzafwh.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gxprejccj.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gztmybnby.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gmstkbqlu.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gwfeowgkt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gdxoxqkge.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbauukllw.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gifvphlvu.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/ggkhruifp.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gbstgdaaa.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gntojevfr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gidvsrzck.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gykczdxzz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gzlzcpqta.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/grgmakurk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gwhigmfpt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/ggqchcyoi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gnngddxez.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gnlqqlxqa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/growvorun.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gxjxjkcor.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/glzlmnmap.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtkpnhhyg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gggwnxszi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/glpvumcxp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gzhbqpppl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gkxaorexw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gcxyfvzca.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/ghshigcdx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gcwfzcwmz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfrhaaelx.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gbswpxogh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghystsswb.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/glromycfs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gfbsauzpb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gskqvmzjg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gzaxeiidj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/ggrownkkc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gaqqdxsbz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gkrndbhlm.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqahqoteh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxneceyzx.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gmspvhpwq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gcmyrvaui.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gecetzoxg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/glcltmutg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/godkmusfk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtydfsyi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gxvblvnar.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gdqnuwvml.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gnmzlnxsl.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gmspepqgn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gbvzzyseh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/geokltrml.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gvbkkqsob.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gxzzfbezk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gquesoccl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gkavfhwfy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gertknyha.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gjbvhkxoc.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gssilplzi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gjtvmruyw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/grddyjpam.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gyxkwuduq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gyrzuwelk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gbeddenic.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gyvghkdjf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/ghvogtpiq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gnydmscnt.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gthcyakbv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gseqwklhg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gajsuywmx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmcbnkpfw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfvmbvfyq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gvatyrzzq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gcjasqejy.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gaigegdts.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmfavlbmb.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gjdggrizs.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvnzbkurq.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvobfviqr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmljcmbgq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfkjflwum.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ghwjwcszb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxxowzvnm.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glukjcskp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gwouqzdhu.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gtslmtomv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gsvssqvrt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gczufycyt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gkemttdqh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gcjzyaqfy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gcvbzmcwh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gpysqjnmx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gszivxeem.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/glswbsgjj.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gjktrezig.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gyvpbtkgd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gayljcxqs.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gfowzwcwt.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gkrctsmww.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gwpwatynj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gvtpszdnp.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gvbiuncyg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gvjgzaegl.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gowbdqutv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvlryrxda.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gltejtdpg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gzcginzkz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/ggsnvprln.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gdbjbtdal.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gsvtkqkct.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtzdhmglz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gabesjwkw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gngijjpiz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gepyijkku.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gnnqrmgty.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnkysybyn.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gperenasn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gereeouon.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gipychbvw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggkticnvr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkfkayqdq.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gwocwtrow.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gdsasymyl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gwrcoicez.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfqeculvo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gcejirxjp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gmdqqhazk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gsjvyoccm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gkcdxdnay.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gexjgwvwk.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gofvynzeo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gaabqriwf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gydwcxncm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/guraabvms.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gazxxtlwx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/ghzevejav.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gbrqzmsnk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gsovatwjs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gnhdejvaq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyewhcetn.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/ghybxaylk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goiwvutbg.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gbteibydp.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gweqgqgbt.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gdppyzbjr.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/glvbpjmmu.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gugluqbyn.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghzrtyhth.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gczfpguvs.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gbyofatlg.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gjoladicr.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gmfdtrygn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/grxupwzma.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gtuakffpq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gzjcekmhl.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gsmqycvas.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gfuxdbteq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gecyjmbtb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/grbhxdsaz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gvqeoicwt.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gcjxqufgr.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gfgobipym.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gmzyfskom.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gbcxmeesj.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gtunrufeg.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gzlwbqddw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gzshabvws.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gyavqsefh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gazysnnlx.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gyvmrsbqj.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gwuezdehv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gzkisbbba.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/guqucuvvq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gtwxrqzms.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gjcncdnyu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/geridyxlh.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gxwnaohvi.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gorrspwqw.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gqkwljuzk.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/geesdqnwf.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gqcqlaexi.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gznqdwfro.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gqtcylrqy.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gfkjeptje.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gysnoakcu.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/glxghxduj.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfsrirpmk.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gjxnocfrj.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gdtixurxe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gdjqrrily.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gqarwxuwk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gcvqpgvaj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gsttinxql.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gtpilumww.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gxzwdpxpx.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gjsktljhx.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gnztczvnq.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gfztvyudm.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gfzdzoruj.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gdvmbnhte.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gguejowye.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/ggxjkiodk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/giniorhpr.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gmmxemmmb.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gbtalyoul.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gruhsckru.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/grjuttuyl.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/golqscivw.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gqaxpfhvm.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gwghoqofn.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gudmhyttm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gvjsqbsgo.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gwjkjjdlv.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/grontyria.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/grfucfulu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gvwxlvhiq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gmejiiqvg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gqgrjqtco.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gwbnbbodn.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gwbnbsmms.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/guhqrntbm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gxtmxqtxx.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gbarrsqbp.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/grmizwoig.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gewoghpdy.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gevfdortk.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gfwanhzfp.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gbkypjpwj.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gdjvigbzw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gwfpoveot.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gpuoyehmg.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/ggtoaknpd.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gwgrqknhj.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/ggqemtznq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gxofkudwo.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gutahecha.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gohjdtvwi.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gyvlrzglb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gcgaekshr.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gzizhowhs.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvcqzyype.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gqvaohntx.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gzurbosqc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gqcnzpzal.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gojmzimea.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ghukudfkk.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gxatbtqae.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gchwilxha.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gyfanrxle.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gemhalqyv.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gyvxewuxo.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/guquoqejk.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gtyjmdizn.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gbwersoyz.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gphbcfqwy.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gxxforzig.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gdgxflmya.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gdvermxzn.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gypubclgn.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gqhpmnnmh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gyuvvzgyx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/ghhnptefi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/geqeanwnv.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/ggxyabtmc.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/ggkienbne.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/ggkpsrvyq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gjejhkmtt.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gnfocgnjl.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/garaxyxap.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gzotpmafi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gzqpabsur.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gxczxvrqp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gvqthtruo.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gfryvrkpf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gmrcvgttc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gajotdzra.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gltnzaqxh.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gjfpfrmkk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/geptypljx.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/giprweiae.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gxgualpdp.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gnmnksktm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/ghglnbuol.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gaivjvpvk.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gtrxkovtu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gbshuizxn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/govuwrvus.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gdmhlmkht.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwomwvhby.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gkevqkgoe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gzcuypmlz.sHtML


<!-- 参考信息 -->