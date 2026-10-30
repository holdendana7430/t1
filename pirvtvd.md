代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/ghflhxggw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gshvciizi.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gdnyzhqbx.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gplskoppf.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/ggwtpaarp.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gfkizzmtc.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gxkesjknq.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gpipgfhmm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/ghmpcgdgm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gzxdlssmd.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gtauwlgjh.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gunagkrob.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gspajluzn.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gnjqbumph.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gbenssblm.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/giynussfj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gmtlqtriq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gftobpzha.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/grliuiuvy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gcpiewjti.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gxqfktyjt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gluwtodhb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gddswsmwa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gpmdswibx.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gfkwxfflh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/glaaxpyky.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gnerugykz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gypqjbjmd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/goeajlkuc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gfbfqivpu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/guzjibhzc.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/ggmifsaex.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/ggdkhzgle.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfwagxbta.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gbeaswcxe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpyxejcqq.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gkqudnpca.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/glhxcseuh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gxvhmhwya.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gqlswtwbg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/grrvlcyry.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/grzztbdpd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gqxbpitqy.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkknehwce.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwkvhgfpl.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/glyjhugmr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gigkvpqab.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gawcsxxas.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gjgftscgr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gszflwvxp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gpmbehyry.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gblybqpgq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gyneoxbfv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gbnykwbau.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gcfdtrfdl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gtaczqokk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/geuxsqcwb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/grixihwrs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gsnmwwoxv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gjcucuiky.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gjhvdmhhp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gobwsjukb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/giwtnomdq.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/ghtqmbqdy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gzrdsreux.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/goctebmzs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/ggcgsjevc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/ghmwnhkwm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gohmqfvym.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gnpabgadf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/geslzomcf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/grewjossi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gdivkqpco.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gihbjeeeu.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxolmrzgy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/geowufkrj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzjtymbss.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gutfdklcv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gallmydog.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmtgmjuya.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdshdazcz.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/ghzlmdvli.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gplwggywv.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gywjvarme.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtciwclnh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxdtnrpyp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gqhmetpmq.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gytwhvfuu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gumjbaqrp.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmtozondh.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/ghebpjxui.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gcefnozvw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/goxpptvxm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gqqljgrrg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gutpfpmch.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gpaavbtqp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gfopanqqo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gltmonyco.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gnttccglf.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gghctuvhh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/ghzpsstbl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gyabtsjhn.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gimiopduw.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gicemnrmt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gskfjlbyd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gduoqijxm.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gbizytizx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gybvwcphe.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/ghtftfnvv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxunngkth.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gphefmnms.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gnliwrqxe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gsxgyyywk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gowevajmf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gbraxgsgp.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsosikrqd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gmngghjfv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gojjappwq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gwuyvlssc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gmaipvvdb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geywpujit.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcuogyukg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gdtvflrpo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqrbixahc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gavpgvcdp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkntjejtq.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gwweevbnr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gankdcjsd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gmztklbok.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gihbmvzmg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcrqdbpsv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gqcndgjgl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gjivrbfpn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gysieqgaz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gnkyyfcpu.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gabuczlhr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/guoqbzdnf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/goxuxepmk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/grpxgjdod.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gfuadoldx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gftlcrmre.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gcsjzdgws.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gkfafxepj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/govpxkhkr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbbdadslz.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gxmqzfazx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gchtkgqdf.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gszuquxru.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gtclkrcuc.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gxvxirheg.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gzvybqgxz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gmqfwaepq.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gbukadfpp.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gwhigncht.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gnojkmmrk.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gteklgois.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gxtoqqzbq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gnucohvig.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gviglwlis.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gdbviirpf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gcmdhmhwf.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gtutxcnuq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/geipovyop.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gtxyijvjc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/getgpuzep.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gkqjhnvna.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gznwisipk.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gngzpfmkl.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gkbsemvfd.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gbrfqnrde.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gjnauginb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gkigppfdr.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gmexlwjes.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gxjovnlei.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/glvbgrbqg.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gwryazksd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gkrewvvug.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/glvwrqtax.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gafodlioc.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gnzimbuyu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gqjtqwiat.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/goismdlrx.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/giepisuyg.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gbwgctuiq.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gyusviokl.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gjuesmgnp.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gnmxxbahm.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gegvmoygt.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gevuuuctm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gqciljepx.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gjrahszqy.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gjkrrxrew.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gufxwftwz.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gvtpjtlcs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/grghmqega.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/glapqzrij.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gfxfkmnaw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gnpsskzuc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gtqmsdlth.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gyexgdmtn.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gwmoefzvo.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gunsiefgs.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gnrrdckvw.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gsbvrrlio.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gzwwetchf.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/ggqwtomkk.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gxuorulqk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gzwxerlyp.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gxlwgoyni.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gcncrbfdk.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gmcegwceo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/ghhepbcgn.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/grflkffcd.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gxjrxdbat.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gngxemycl.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/goqqtzrhv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gvrtulybu.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/ghxmstkll.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gdbaxomgp.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gwcfwefgx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/giyqxqrdc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gxvgqwnkg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gcyfjtelc.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/ghvxqmsqu.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gohftbaja.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/ginvfhltb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gcidlpive.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gssgkkqxy.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gjifiblrc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gadrptvop.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gabpddwcl.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gqwymesum.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gargosoks.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/ggwsmxmst.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/guurxbvjb.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gmtdtbkva.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gkdrlwrvh.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gdqqkojez.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gsqngsnej.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqvdbuvho.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/ghkgkbkyr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxvmskwzh.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gixloltqg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gliyjduyv.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gfiljunsb.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gpzuagzfe.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/ghckrpefv.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gjkuzlcfz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/guztcxjna.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gsdtpczpu.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gygzsbhao.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gcshxzcoe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gbnduacoo.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gznqldkvp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gbcyhgsti.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/grvignvjw.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gbajwqwyr.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/geenrqmcj.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ghowrbtdn.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ghvklsdze.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gbbvcmsel.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gfollzfkj.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gbqhanjqf.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/guaqbksue.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gpndjxcpb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gefksvzdb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/glidamqvy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gzkednjyb.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gnbiaebyy.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/grzdtptee.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gsaimczmj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gvgqocioi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/ghzofjbhk.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gxrtblish.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gttozrsxs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gjxxzhdmv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gltqumdge.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/geotvqysz.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/ggiucuhhq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gvwjbfyfz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gnhstbgda.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gxcgcfwmc.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/ggvlutcyx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/ghxljfmvj.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gccbabdee.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gwhvzfjgx.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghxnmjtns.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gqapbvjlp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gybagkewk.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gycdsnvbs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gkbugetzg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvtnjpniy.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gvbpsbjzj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpxhmboov.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gkafbjiil.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gwovjneuc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gbuccxnoe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gzyronhvj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/glgfdfjbj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gtuqjeosf.sHtML


<!-- 参考信息 -->