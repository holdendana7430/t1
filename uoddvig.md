代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaeahbiev.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdtimdrz.sHtML

Java: s.lines().toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gjvxnheih.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghopzxkqv.sHtML

Ruby: s.lines
来源：http://blog.fanxiaobao.xyz/Article/details/gbtwbywvj.sHtML

C#:   s.Split('\n')
来源：http://3g.fanxiaobao.xyz/Article/details/gboeypwex.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gortlycnp.sHtML

Py:   if not s:
来源：http://www.share.fanxiaobao.xyz/Article/details/gwawqizod.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvixqdyku.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvefbpoop.sHtML

TS:   if (s === "") {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gawhyfysv.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/guhapqkdi.sHtML

Go:   if s == "" {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbocwgjar.sHtML

Ruby: if s.empty?
来源：http://www.share.fanxiaobao.xyz/Article/details/gmttjddvm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevqwxvau.sHtML

[E21] 超长截断加省略号
来源：http://wap.fanxiaobao.xyz/Article/details/gkgpbvgsh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fanxiaobao.xyz/Article/details/gjptatnkd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzttuszci.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/guziuikmo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgwhmhvu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/grwuofxdc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fanxiaobao.xyz/Article/details/goqldqsia.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gletunlfn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/glzsduelf.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fanxiaobao.xyz/Article/details/gcsmmcbhb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkpwbahb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gotvvmqob.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/goanwfsun.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfjwezts.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/gdvrblmen.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fanxiaobao.xyz/Article/details/grtrdwjkf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkupubsyc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmxlkhqs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzusznul.sHtML

F. 文件与目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgtfdpuj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggcpgoryw.sHtML

[F01] 读取整个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goiqdnosj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fanxiaobao.xyz/Article/details/gfyllpixd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgaqykfx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssarshhq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/ghrvqkznw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzinkrrw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fanxiaobao.xyz/Article/details/gxqbdtqsh.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmqfacgj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gdsjekolh.sHtML

[F02] 逐行读取文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsnvirzfj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpqpqbke.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdvynisrk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvayfrbhf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/grjjpfwhg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fanxiaobao.xyz/Article/details/gukhvkmmo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fanxiaobao.xyz/Article/details/goofkkjfw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrgiuvrj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gualyzpyp.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fanxiaobao.xyz/Article/details/gorsjgurf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkgjgyir.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gnrqcgzjd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gdsuwyuih.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gjjkorlyf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fanxiaobao.xyz/Article/details/ghwhoadpu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fanxiaobao.xyz/Article/details/gklafchle.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjokazluq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gdozwhjws.sHtML

[F04] 追加写入文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcibubexg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyvjnabt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fanxiaobao.xyz/Article/details/gtjxuyyfo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxxmrzjd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdwjdfwt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fanxiaobao.xyz/Article/details/grbdpzjvx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gxncyruht.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gprxxtydn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfnxircu.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gxcwuabgn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fanxiaobao.xyz/Article/details/gwxksjuyu.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gslubcapb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/ghvlxvorz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gsrgjjvdj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpxbvgai.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fanxiaobao.xyz/Article/details/gtkpxlgxt.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gukkiglyy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokkhpjnt.sHtML

[F06] 删除文件
来源：http://3g.fanxiaobao.xyz/Article/details/gxjxgbmpp.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzaghnob.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwvqxgst.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gscqufdin.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopfgeszj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gteacwsqe.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gcchxdbeo.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjqmzihe.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxupgtwb.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fanxiaobao.xyz/Article/details/gtcxntsgj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gmtcrsxte.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fanxiaobao.xyz/Article/details/grtwdyadw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gqyvxbiax.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gzckaaiab.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmeotbxbm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnptasxlx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtsydgzr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/gleyrqney.sHtML

[F08] 遍历目录
来源：http://blog.fanxiaobao.xyz/Article/details/gvytqhrmz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyizcsjr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkidefsi.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gmeuhfezt.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gzaxitxqd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxehflfm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasgsxvwo.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbaaefey.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gmvitcnow.sHtML

[F09] 获取文件大小
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdddwkma.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksxlwkjq.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/glokopgan.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gwlogcrvv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/gyfmrdgtb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvbmcmoz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnajuaoc.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpumkbcsj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fanxiaobao.xyz/Article/details/gwsnuvyol.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fanxiaobao.xyz/Article/details/gsokawjgz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhvsplfq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gflguxbag.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcihokgoy.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnwpcqdi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfpldiuy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gocmzgilz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhuwxhwl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gfmcmrfaz.sHtML

[F11] 复制与移动文件
来源：http://3g.fanxiaobao.xyz/Article/details/geaasmfeo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/govcamjqi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfksozwck.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnleseovh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gheskbihs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gdtjncogt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fanxiaobao.xyz/Article/details/gxhorwkzh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gycdryfpb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkermwjag.sHtML

[F12] CSV 读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxqbfzio.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjycduox.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkcjylji.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbtioygu.sHtML

TS:   // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjdypffc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjvqikxj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggotjyjai.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fanxiaobao.xyz/Article/details/gylewjdpq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fanxiaobao.xyz/Article/details/goqptlxuz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gapqehgsf.sHtML

G. 面向对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gouijwesa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grmnhlrdx.sHtML

[G01] 定义类
来源：http://blog.fanxiaobao.xyz/Article/details/gpthkvnbw.sHtML

Py:   class User: pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/geibhjrjj.sHtML

PHP:  class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goscqagot.sHtML

JS:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gczjxcozo.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbstgrrls.sHtML

Java: class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gryqojkjz.sHtML

Go:   type User struct { Name string }
来源：http://baike.fanxiaobao.xyz/Article/details/glgxhqwyj.sHtML

Ruby: class User; end
来源：http://wap.fanxiaobao.xyz/Article/details/gebjkzujf.sHtML

C#:   class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdymoiycp.sHtML

[G02] 构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfzisipg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fanxiaobao.xyz/Article/details/ggyiclwgx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gsqmhmtlp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjwjohilc.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gyqwqlezj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvkbampp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpmewwuy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fanxiaobao.xyz/Article/details/grxevtdnp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggeyalswr.sHtML

[G03] 实例属性
来源：http://wap.fanxiaobao.xyz/Article/details/gfmkxprwb.sHtML

Py:   self.name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gkkigyhup.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxzxpwjm.sHtML

JS:   this.name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoirmgqi.sHtML

TS:   name: string = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/guwyfomyv.sHtML

Java: private String name;
来源：http://blog.fanxiaobao.xyz/Article/details/gsnfzmyyo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnthuawtn.sHtML

Ruby: @name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gxetmftov.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfeunzer.sHtML

[G04] 定义方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gsojuhafg.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fanxiaobao.xyz/Article/details/gxsqnejcm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbhabqyo.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyscspbh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqioxsts.sHtML

Java: String greet() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnkjgmesn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewcktxhc.sHtML

Ruby: def greet; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gqosbxmlz.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnpevogu.sHtML

[G05] 继承
来源：http://baike.fanxiaobao.xyz/Article/details/gvmjbzuow.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/glrybdllh.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gcdggdxip.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gpworsofs.sHtML

TS:   class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/guqiazgpi.sHtML

Java: class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gwnviakuz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fanxiaobao.xyz/Article/details/gxfjznqkv.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/goymbkitn.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxatskpzm.sHtML

[G06] 重写方法
来源：http://3g.fanxiaobao.xyz/Article/details/gbhjvbrhp.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaajabysn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/glpfrbwhj.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjotnaqxt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gocdigjzd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnosdlmoc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxptuddel.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxvgusmr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhgzdrqs.sHtML

[G07] 调用父类方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gfujkzgow.sHtML

Py:   super().greet()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjfqeyqp.sHtML

PHP:  parent::greet();
来源：http://wap.fanxiaobao.xyz/Article/details/goswgianr.sHtML

JS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmvdjfga.sHtML

TS:   super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfbsinls.sHtML

Java: super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxdhcqjw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoybkpag.sHtML

Ruby: super
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkbmcelw.sHtML

C#:   base.Greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gpcvreucm.sHtML

[G08] 静态方法与属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcfpgpiv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtoqudkd.sHtML

PHP:  public static function f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gohbnxsvt.sHtML

JS:   static f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gliyplnex.sHtML

TS:   static f(): void {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvbgjywal.sHtML

Java: static void f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaghwtde.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gulagffgz.sHtML

Ruby: def self.f; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdpovmqx.sHtML

C#:   public static void F() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwzfzuuo.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgmylses.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzwnbspm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fanxiaobao.xyz/Article/details/gblunwgdi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fanxiaobao.xyz/Article/details/gjkoyywqt.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjkarxaqw.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gllwsrrsi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fanxiaobao.xyz/Article/details/gzezedvbh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjyotzvd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkpsccfa.sHtML

[G10] 访问控制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgufqskg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzminulq.sHtML

PHP:  public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gpspecdki.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fanxiaobao.xyz/Article/details/gflmiyemw.sHtML

TS:   public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gousrerwt.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fanxiaobao.xyz/Article/details/gfmcxujpc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqzwwexl.sHtML

Ruby: public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbgflxec.sHtML

C#:   public / protected / private / internal
来源：http://3g.fanxiaobao.xyz/Article/details/gitdgpltz.sHtML

[G11] getter / setter
来源：http://wap.fanxiaobao.xyz/Article/details/gpdtacefw.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywaoqees.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsymeoyjd.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gudypaqnd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtwnaiemk.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glfpgbecb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzmvkqhh.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fanxiaobao.xyz/Article/details/glalhujxz.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifdbktgm.sHtML

[G12] 对象转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gsvlagvbm.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fanxiaobao.xyz/Article/details/gemucbaeo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvelownc.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gswzpawco.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfvdsipxu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfhjorsu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gerlzqewj.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gpizcqhrc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweykrljy.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbkohdub.sHtML

Py:   isinstance(u, User)
来源：http://baike.fanxiaobao.xyz/Article/details/gvhcfuibn.sHtML

PHP:  $u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gwnkmprhy.sHtML

JS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkjxjpbh.sHtML

TS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gghngzzey.sHtML

Java: u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsgkavhu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fanxiaobao.xyz/Article/details/giexnmcxt.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghthqyguk.sHtML

C#:   u is User
来源：http://read.share.fanxiaobao.xyz/Article/details/gloscojkl.sHtML

[G14] 数据类 / record
来源：http://baike.fanxiaobao.xyz/Article/details/gnxaneemh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fanxiaobao.xyz/Article/details/gtctvgike.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/gihlsznji.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwlbtuxo.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fanxiaobao.xyz/Article/details/gqpmtjvsz.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gjudjwmbv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvydnxkgn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbeofdeu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fanxiaobao.xyz/Article/details/gekkmeywq.sHtML

[G15] 枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/glnvzracy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/guuxjfasy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gpaikmbuc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbcqihoh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gvgwszbte.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fanxiaobao.xyz/Article/details/gwgczpauj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fanxiaobao.xyz/Article/details/gccpncovb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fanxiaobao.xyz/Article/details/gwbumiswp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gybjnpmlr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzrajfix.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcyuaplo.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkecfvjde.sHtML

JS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gaqkwjpac.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxyqucag.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fanxiaobao.xyz/Article/details/gzknivrnn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fanxiaobao.xyz/Article/details/giqibxcdh.sHtML

Ruby: obj.instance_variables
来源：http://blog.fanxiaobao.xyz/Article/details/gdcdwrcsr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/gimkcykgm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpklijph.sHtML

H. 异常与错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkrezskx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkgqknin.sHtML

[H01] try / catch 基础
来源：http://wap.fanxiaobao.xyz/Article/details/gdbjjyjgg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gwqgjxkoo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfprejirh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmysmljmv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/giqlzndon.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fanxiaobao.xyz/Article/details/gqklhvpdi.sHtML


<!-- 参考信息 -->