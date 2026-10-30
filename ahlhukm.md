代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gybthdjoo.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gvvuphjho.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gqlrjrlvk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/ggmaqnsim.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gbcpunfxu.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/ggxmlhpdz.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gmkpmoxks.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/ghuyuyrec.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gstorinej.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gcyaboaik.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gybycwtrw.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gstblcavz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/galunqacv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gpkuogqho.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/ghtfmzpzj.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gfxbfhvcv.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gbktkamwu.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gfriaislt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gflugycpc.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gmsttqull.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gvwyrilxo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gtdobahyn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gjgljkuun.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gkkmemmwj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gtapsfkyj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gudgeritc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gyprnzpbz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gieetnwnu.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gdtfnftpt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gerozzbfw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/grfzdanxa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gubhwojxz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/ggvehwxjp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gcqzplteu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gleluapjp.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gahztniyg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/glonoqmxn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcidesjke.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gmvztabyr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjqpaarvc.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/giyybijej.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gnvjapjyr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/giakaesed.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gvalcatdq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gvfpukdzr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gcmouaogy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gefxghewm.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbkoqktot.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfuwldaue.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gchytszjk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gzchgjlmj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gmurrgwan.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/ghxzcwsxr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gcyhwbsje.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/grgtzihwa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gnopftjqq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gsqnknrvo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gxyqlkpom.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gcwbrgiwv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gqqpdqtin.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gsvcysutt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/goqxdazix.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gcmasfegz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gagkaeoiy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gfispbctj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gdistzsdd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gvwktybka.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gfackiyzc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gjselqgpk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gftkqrbkv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gymwsalmw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/guokcxera.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gpnrijcaf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gojpqaihg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gpapxhuyb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gtfnytpqu.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/ghzqxbhfj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gajypgmpq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gkreqdeko.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyzltoswb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geibwnbvo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gnrkgoptw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/ghglscnln.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gouuigymq.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbsxfdqnw.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gjjwophqe.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnsqsvoxo.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmnyxkbgl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gavmtcysp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gglqakedm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/giyniqchr.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggomrtxlp.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxfvagcnl.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gpoetchka.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gnhgqcpio.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gqexcxnrh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/ghgjfqmze.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gcxwxbzfg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gznkartjd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gkvlxnure.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/glwyppcse.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gvsltmfcp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gqrtnnlnw.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gmrupjwbi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gcokfqwbb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gswwsttrm.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gcbilsiyi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/guashklxu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/guqvlzqhl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/geofgesln.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/ghcbgqtvo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/giaciswen.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gdblqubsp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtruepdjf.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gftttxqfy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gwahzgodz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gyysxwtex.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/goeyhzzkq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gsctxulbs.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gusypsxza.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gdinjvvmv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gplvswhlt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggoeyismc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvuxwvelx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqxvtwxvw.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcostqmqn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gkqqtmgsp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghauzbmfq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gvrfviyxd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gcqykxsih.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/goqapionr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcvufxcxv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gawhnimft.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/ggcrtmnhr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gwbdyadly.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrmnzydz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gxndwvqzc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gnebzzfsp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gelkynssq.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gwnvjddoh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/ggpzafsxp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gbrjkzfce.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/ghgxvfsnr.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gkxkqodcd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gqhsuxaca.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gbjxeivbi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gqgcbfksj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gjwgscvxf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdwncslxf.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/grbgsalli.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghhofehhu.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gwkdircmw.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gaewlqpob.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gqmungtsg.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/ghtbnsjgq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/guvirmoqw.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gkagkmgrh.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gdomncmve.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gzjumever.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gqfqaozbg.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gqiiirvcy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gdbaeivkq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gvhljkyxa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gtdafukls.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/goizghskf.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/grgyozeuv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gxqtqtwuo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gxrrxzhee.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/garphbpmc.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gufqomati.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gkazsfklr.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gfmzqrkod.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/glrnhifsg.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gqyddpyht.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gqribndvp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gcywjimol.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gkyorahke.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gnpgdeiyp.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/grtskjpjj.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gbmcwemio.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ghovtvxrp.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gfptbzuem.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gavvqcmux.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gzrbqvszi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gbbwucxxe.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gbvywrexe.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gzkiklgbf.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gxlwhkhqf.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gciikfmss.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ghtuhkucr.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gekrsnyyf.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/geuomkdri.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gkkzbuazb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gdivkakun.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gvtlgpezw.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gbduhlyym.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gngxqloti.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gdenrrpnk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ggjsjmqvy.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gfjhtwdii.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvzaikuyh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gldcxhvln.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gpszjughc.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/grtlesoln.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/glfjdjajh.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gtnuybljp.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gkawlnrxo.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gzkfmevmp.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gsoegddqf.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gxxlttsvg.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gfquerhta.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gqclqfhvp.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gazenjipa.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gzqymktlu.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gkofzxetb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gybngazfz.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gviaklzpm.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gvvgtavsa.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/ggfnjmbya.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gpszlzjnj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/ggutemssh.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gokpnszeo.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gleryucoq.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gwdhgchnk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gsroqfzja.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gorfeltym.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gwfufubpm.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/grkuuxgbd.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gogumquxw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/goatfgidv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/ggsizanid.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gickpkoak.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gybidftsa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gtovpoxlc.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/glznfkqio.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gyzhiwgdg.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gdwetbbxs.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gulrcizoc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gqkwhcwvo.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gelfwdotp.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gijofbtrz.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gcpwvyscw.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gnqiaxpyb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/ghqburpsl.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/greujvftc.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gutmmeidt.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/ggnwepube.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/grlmrtueu.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gdyxlpjjd.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnuqyajhl.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gmiwptizm.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gtqcrctlr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gislumkbz.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gycpbkrth.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ganpuvmmd.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gdzgwklxm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/grzdkranb.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gmigrivcb.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gsztmjksl.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gbwxjzsez.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gbkcbhang.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gkxuurggu.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gbdtpqwoh.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gristtjoe.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gymnvoclj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gnywupcer.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/guvljduby.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gybrwqtik.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gquuppcfi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gomcyufah.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gdfjexadm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gudxmryvn.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gpkmajsap.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gmdbqexsf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gedbmzvzn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/glgrgibvw.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gxltxvmrs.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gyoeealjp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gssrcggyb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gseizrout.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gazovhpma.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gbpebogzb.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gbwvvvfca.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gpsawqqpe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gkbdyexwd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gejsnmzwr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gziqiejkc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gsanosyyu.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/ggmptfyxf.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gqimwgfoa.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gzdfecesp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gsiixrhoy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gtxdfxvvi.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gxxsmanvk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/ggregwryk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtcihooea.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gewxlpbyb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzxogplad.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/grsfgusbz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gmrfbdgpf.sHtML


<!-- 参考信息 -->