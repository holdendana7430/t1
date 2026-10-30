代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gsaxbdduq.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/grahlzphh.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/ggdeswsov.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/goucqmnwv.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gqpftesdc.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/grsxxqrxu.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gzafgytes.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gvfqkkepk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gjvstqbat.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gkcsjdnmp.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/grkxlqqua.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfvhbwsgk.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gpkygxgck.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gadxurzwr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gcegkwtue.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gsmokrddi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/goekhtiyu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gprwhuijj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/grlanhvxd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gyikyitfz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/grftcaajz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gzpprhnxb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gylufwlgi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gjcurqycw.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gjazfucsd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gnvgjdrtb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gozsnevjl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gnjqvzpcc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gpcrlnxvu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/goxmqkive.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gaxtfwuga.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gzeihruzv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/ghsbksgpd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grexefvlv.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gpzcogufb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gixupjlal.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gwpvxstcr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gvtxcyvdd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvhkqfclr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gmvgpnqzb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/grahlschg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gyillwbck.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/givduqmpq.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzhvtnvyl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gohxiczmw.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/grvkkclon.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gjnjnhvuv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gtrhyvxgn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gplbkffey.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnnnuiwql.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/grxbpsmry.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gpiqmdjal.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/guyyjhrxy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gomrstwkz.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/grjsisaid.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/giuhpejkz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/ghypaxgdz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gnxzeehfk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gxjbqsxug.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/glokbzzci.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gckunlhpi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/ggrwxhhia.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gmhdwvedr.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gzrvgaltj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gmqqaphjs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gihpehbii.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/geboxexyx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gpwmmqjbw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gsdgiexxn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gktpzlnjq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gnycpapit.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gzwrawxcv.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/guxcvykxv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gczbubald.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwwrwjfkl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpwywsxon.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghmwolbuv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gkaaujroc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gfxpoxxxn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gimhicnqh.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnzxnfxfs.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gypzxwctd.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gexcbyyos.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkknpvetw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glragclwj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwhxlkfxh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwqmhhspo.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gelxckkee.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxzroyrrj.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gepfrshyi.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gsehdtuai.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gulggplxt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/galfdugnq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/ghdufuuxf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gryxfohgq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gdfwjodfs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gjhbatgdx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gquqnlinv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/ggmpilbjj.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gidmsywxv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/goreopqpn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gezsyxlie.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/goihhfrft.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gxhwdodpm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gftomgvps.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/goxehfeho.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/ggtvwetnq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gssizytlg.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gczninpsl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqsvgtkpk.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxsarglcr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/geeekfrot.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/ghdpwhdlf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gvzfkvxfb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gfjrnfoiq.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmisbjjmo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/goelxqnub.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gnhicrlfv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpkwqardj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ggzrnuvfl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcjpbkmpw.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggjjngxuk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gvxrolisl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfozrpffw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzejxidph.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gahgipzrn.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/grtzbocuz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gkithllca.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gautaeuxc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/geroawcnm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/geuqdsulq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gilxichcu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/guzirycnv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gfswnjfzv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gadovsbfi.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gycpcrmpe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/galznhthx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gftjcgken.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/grxdwrren.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/godjfagnr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gconmcrvz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/goumiwqle.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gnctknahi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gmwqyjtmf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmgntyrar.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gghdibzgj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmazrpdaz.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gapdbjhit.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gknaqcshu.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gznmtwnis.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gldejldwf.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gwxldqpqo.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gwzvxgvxw.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/geljkqqvb.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/grxrgbhyy.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzotwljzt.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gqjfulnuz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gtnmnzgzz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gliwgeaul.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gknuwrxsi.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gwdnrmhnq.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/grgzzazyg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gvpjvlwke.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/grwadgqys.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gfiqdmvwm.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/goxedhsoz.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/glxoylqvf.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gaybblflv.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gkusrxkyt.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gznemyohq.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/grmewsrfn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gsrlgnpmf.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gfqvtnayj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gyxxqpiru.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gnptypaxr.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gvpeknzym.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gfqxzosek.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gzfnzhlti.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gxlvnopcb.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gemiodqdm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gugcefjie.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gifgocyjh.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gdznpkqqf.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gmpiwngvc.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gfczwbtxm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkbkuozox.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ggrujjshs.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbjuvbzbu.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gfxjedkys.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gckklyxdj.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/grrjnolpv.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gdtglrnko.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gxyyoqufz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gwysinldt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ghbmntegi.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gmhdagnsj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gcaugmniu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gaqehdrkt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gvudorqur.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gtudmngxz.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gbvkamuph.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gcxtpphza.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gxooxrkfw.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gjqoubuxr.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/geacohreu.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gcoqerfno.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gxhnrwqzh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/grijneaad.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/goslcrkeh.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gsbsrndau.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/ggznuksrl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/glnupdjht.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gtejxjnpa.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gakyqgntr.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gmeirlckw.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/guouxadfd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gxstsofqm.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gixgvxnzj.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gfkxvywqi.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gfnvaypra.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gwxoezpmm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gnupscqaz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gecucqmfw.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gjsotivry.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gnxnrbdye.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gyyichpit.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gifmlrvur.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/grfslyoyx.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/glpixutap.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gxxelaqki.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gdbtisnzd.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gzyddgqni.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gghszlgyd.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gltphxbci.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/goxpkqzxq.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gglnbphsb.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gaxruhvoj.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gbryjsqah.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gjjnhqscv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/guaxxyapu.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/ghfhyrrxk.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gxjzcvfap.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gkkwjgbqd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gzuiyaawf.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gokxsxopi.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gifvavhsi.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gdkzdribx.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gjlhvipil.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gkxogsblx.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gjnlovrtz.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gkmoxdzhd.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gchhejmzc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gypkhsqrr.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gjohdzukj.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gyxvprufy.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gyfsvezog.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/glqxrbwqs.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/glnhezuak.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/grzkclxtn.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gtauhudtt.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gsqstbhog.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gcnorayji.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gsocnesnc.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gfejstayt.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gdlwzhwxz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gobdlkwks.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gyonamdhq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gtedqjuey.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/glhzvqvpn.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gvwxszacj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gfmkblivl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gabvfjwyq.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gyrwshhrw.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/goofzpwcz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/glvsgjqmn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/ghysumrlq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/ghieyapme.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gincwphti.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gmljemzrw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gfefjjukc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gzfvyenxy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gzcvlrthi.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gdpyaiobl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gqakauppu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/ghjvdpdyo.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gfnirbkdi.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gkkikvfsy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gplywgzzb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/govvlfyxm.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/glsbihrxu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gyaqiskax.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpiiovkhc.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gvapxsgvm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gepeoxmfr.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/ggrqfgowm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gqfzhizna.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gyagpsypu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gnkivlvco.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/geyqufveb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/ghxvascem.sHtML


<!-- 参考信息 -->