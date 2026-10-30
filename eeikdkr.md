代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/grfclwmcm.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gdzvbnacw.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/grupuxwhh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gcjjgkexz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gfezvhawc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gvcotjsqu.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gzgirkmpl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/greoubbpr.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gfpikhfdu.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/ggueovefq.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gretvowsi.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/goipsokoy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gmtcvbpeg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/griswdrjt.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gdhixrako.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gfkmjotli.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gyhrrlkdt.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gtoihtmdc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/glnexmcyo.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gdohytclr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gjendlxxc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/grmiarlnk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gcsqcbkhp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gqmkxpeby.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gfydxacfs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gkvbfqpko.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gecvqgvhz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gduxvphyi.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gpjoudgxx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gneytzejz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gltxvypxc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/ghoufhbdo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gecpvlabc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gcntqyvkg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gbuzsbbkn.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gflavaxbu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gzrkqzjyv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkjelpgdn.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/givwnzsoh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsdicgpep.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gqntddszq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gzzncyxgm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjpnfbyey.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gfugxzvjs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/ghhtyucsv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gszvwfoyu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gyilqcgfp.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gjijmssji.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gdxihpeyz.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gldwclepn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gtsedkzoq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gqvpnhuth.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gnkkybpuz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/ghknofmsy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/glnxpteiy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gvahewrhm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/ghpysdifc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gddfomwth.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gozjfloen.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/getlxskdy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gannyaoyr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gituolsyq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gcbehepyu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/goepziywo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/glhundssk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gkdywnerz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gveyitgex.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/ghvbjltof.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/glmeaezsd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gncvnkrvi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gukdxdwpc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gnmwscwld.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gihrgodrw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gnijlkvpk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gykhjpttm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gogfqsdwr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/ghuxtukjz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gvvheexfn.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwvekhgqs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gutkljhhj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqvwgmbzc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gghvzdojm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gmjejjebi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ginkzfvnn.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gnvbjqdqy.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gvixmdfbv.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gufvtpojf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnyjtkzwo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfhelgxnr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goadkhiod.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/grzcbcucc.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/grhwsubam.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grofdvvuv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghlnkbnjf.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gaxbyiypb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gxuvlpuui.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/guvhyvcyu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gvddfqfmk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gjjbxgeor.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gcufuoktg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/ghpcylhhn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gatklmugo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/ghmpdivsq.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gnkiexbrk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gamzneoyb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/geklecwod.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gscjstcvm.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/glekwzjoy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gretpnoxh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gdncbflmk.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/ghmpbdzof.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gpjuxpcum.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gqplqwzdv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpkhjwmym.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtqxyasml.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gbpfzqmmy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/ggnujllvt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gpqykvlon.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gutvnxkwq.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjkqsaeei.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/guvtfytax.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gzqilnmio.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmtrmsqey.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gzqutwthy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gusyemafy.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcvthzwwj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gnewxixzu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gawzzglvv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfjukvuyj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfeomfhzl.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/glzkngprh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gsgjxchja.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gzkrcriyj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/galyjzoum.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gjejlcqqx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gncskvziu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gpgnhnjnz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gjbunjjyn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gklnyeumd.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/giusezvyz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gngktpizk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gvokfzvep.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gsvooswwb.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gecugdzax.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gnjbdaiqh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gikgxcswx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gwoxexosk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gyorndlxo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnfzqcxjv.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gdcnjjukz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxwrkxbgt.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gtrcgffux.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gkabsmuqs.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gsdjsjcaz.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gqsviekiv.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gugeyqicx.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gvyaofjnd.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/geqysxlqc.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gaijwbjvp.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gcoeratql.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/grdqgehwq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/glzwtffcf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/glgvzyixe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/ghbfxwmnb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gpmxzkfkk.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gewcnyfrs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gwxnlfxyu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gbysjctbc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gvexfzdgr.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gkbfzpqoh.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gslrpgrjt.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gxorqmuya.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gpoxyaphf.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gpjypjiml.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gtlhwszut.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/guncmihgv.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gzqnontlj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gojbpsqjl.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/ghndkxwvs.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gffjylilh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsrqdzqiv.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gocdfiekz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gsmubqcyb.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gtszuddvz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gilkttudn.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gpctwhuaw.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/goirjlpwb.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gypfazkjo.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gmbibuova.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxdfdijrn.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gbpcnjnil.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxmunwfsb.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gwgrdhqja.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gprwjjrfh.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gnlynqdop.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gqnrnzymf.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gbzejfcel.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gjvckfxpz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gsxhhpfot.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gkzwojfgm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gzhwuquzm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/geajibdfs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gvsqbydrr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gocxjhpdi.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gwjjwxeks.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/glwcknuzr.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gaydjudfb.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gcicufmnk.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gvarazozu.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gmmjumrxa.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/goiqinjoq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gmzhtqknu.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gjfxjshts.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gtgoxrhny.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/ggjvnpcvz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gythmxtdt.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gtkzjpkly.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gwutnarxi.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnwqomiuy.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gdwhvrxnl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gtjqqqijg.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gmzgotgso.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gfzradgvs.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gusqtfojm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gyrnvwstu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/ghpzbeyif.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/ghgkcicun.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gqyzxuifw.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/godxsesny.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gzbxevqxa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gzzbeveog.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxzpycxwh.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gftbxxcxw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gatlxmgum.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gfspqkqzz.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gqrbrzvvm.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gsopzxajw.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gplcopias.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gqdtuwbkr.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/ghvmcvpra.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gysztuxln.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gbxdfyjwr.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gjsmlyrte.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/grbqtgzqa.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/glkeqxzsp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gwhpajllf.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwycvtpwv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/grqxsfbyy.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gqgpgpuqs.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gitsgqrml.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gjhqcwqoc.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gxpfvwhnr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/ghnymnmqg.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gmjqsxluc.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gqnaukgay.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gipritple.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/guwnldjyd.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gjkmvieov.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gjfqittps.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gztvqaxep.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gbohizbsu.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmywcaxuw.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gaczzenje.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/goboqipqj.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gqqnrphmx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gluvrfklu.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/glbvlkofh.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gdqtszxnr.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gtyekprzx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gzlkimowz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gklaacgju.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gagsmjjhy.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gpulfoanb.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkugfhiuj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gucabpmqz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gpyjowsel.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gnnuipyci.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gcbqkgexp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gpdzpgile.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/glrjnceku.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gktaurnjo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gmummjqne.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gxweoarei.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gnqycxegk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/geiiqvqfl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gnmunpozm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gqlgmthno.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gyjsxmdjj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gxjhoeike.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gcidlkmqk.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/ghfkltljy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gaximeiev.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gqdhrqgxm.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/grlzqdoln.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gleagmidw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grbnqiesc.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/ghjhfchdb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grazojios.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gunyzeddm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gghlvvheu.sHtML


<!-- 参考信息 -->