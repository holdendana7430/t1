代发 wailian999

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gyhcsprwr.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gkursmuey.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gzwrckndl.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gmaqlvehm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gnvermhft.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gklkzyvxw.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gbchdpaye.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gpempzapw.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gvrbtuqrg.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gqlgozyed.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gxhtcyxsf.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gluxtrwrd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gygnyjnko.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gdurtvviy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gizotnbmm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/grrjobwpp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gmfqtapfx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gwaperwbp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gdjpwtrdf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gflqyxdsh.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gynunpede.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gjggkqzbb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/girpebyls.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gclpocklr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gkxrbnzku.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gbgopdlre.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gnftnkxet.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/geotmetfk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gmsqkxlye.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gppokyisx.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gmxswdmli.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwcgpgpsa.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/ggnsdwgzj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gbwyzijyv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjobooiyx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gidbztfjf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gdmaiitwe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gctovlnxk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gszzhrlev.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkelbtysv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/ggyqqkbqf.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gckvmpnrf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/grsucsdch.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/geygeifao.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gjijpdash.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/goqlqnkvm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gbbozdqge.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gcqjqbaws.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gzlsirglh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gmqkmmyne.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/ggqsavbbm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gvutygpkw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/guylcjfam.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gnojzvlkw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gzdffgloo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gskiwydur.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gphcoppxz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gzebwlxkt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gvauondyv.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gmwipqils.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gbmpbwcmf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gsyosxxrt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gesbxlxnl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gjuoatbar.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gqsnpwszq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gldngfhil.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gmldpnmom.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gibtzxnvj.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gnoyycymw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gohzmafie.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gkmvhjyzt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpseefpdo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcixvctap.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gkzizplhv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/greowolxe.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbbiugmss.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwzvtvayz.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gcycmzlme.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gddssjkqe.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gsneczxmk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gprqsgpid.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsrzvrxgx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/glsoiknlu.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/genwjuekc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtvaeweyj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggrpzlfds.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gtijqwunl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gmknciqnt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gppuymafn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/ghdmrkhcp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gerczucdz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gpiphwenj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gjvrsewku.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gmerziuck.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gqwdwxweq.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gbgzobdhv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gmnutjlxv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/glcmizkkj.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gwrqrwikd.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gphnrkawj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gapqcnnzd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gxgvndfnt.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gqmqecwxf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gjgntrtdn.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gddcpzpun.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gatuabwpi.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gqdicjlpj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/ghkmsuosz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/garmdktqa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/glonhlbor.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gnbywdtbf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwxtjnupm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gtlcvauji.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gpzunsrzk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gtdqvgeik.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gmhcmkdaz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmnmdexfq.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcjonvgiq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gbkmjhsdu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzjvtrxkt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gvfjkpkxu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glkexmnho.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gfftejrin.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gnsyipkfd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwrngintg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkcsbsfph.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gquuviezd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/ghwjxijva.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gktzzosol.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gubfetvgy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gszdtaiqr.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/ggfdnbobp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gwshwztyr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gvthdzgkr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/galltcizi.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gmmfppdem.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gyjawozih.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gfnwxlhvu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gxrtovpdz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gqemlwsih.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpxfkqioj.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gcsttyrcv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gctxnnvqv.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gpnqsubkn.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gtvjjavxc.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gboxcuhsa.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/ganltxkij.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gjuhjkjdq.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gepesybav.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gdlifwwle.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gxdpvdgry.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gjcowmpct.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gkzzdywhn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/geyggfxrz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gykekxwzr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gxepuuoyz.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gemrkjdvs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/ghterwfyc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/grqhszqrt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gfuptpxww.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gjxxqutzy.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gkgddbcnm.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/ghtpbfvpx.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gaydqvgal.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gpmcrruhx.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gizlwlelj.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gokflaykr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/ggncpufup.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gycrqdqwu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gakkiytji.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gwjctikns.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/grklgmyck.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/ggdiyprlh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gujyoikas.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gibqbzndk.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/goljldlne.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gzugkwvwb.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/goxlgqnoa.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/geregnwmg.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gvdmqznzr.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gnrajlseh.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gipxouliz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gqpvylvug.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwggtaqzl.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gojzjairm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gmkxyyxzw.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gmjmcpyht.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/grcvynhdn.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/ggcgwuevb.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gigvxufyi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/goftxxykx.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvtalfrlf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gpoytpldy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gtdxfkmrn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gjysfgtvh.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/ggosydlpu.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gxdjyibuh.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gweekgnft.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gngivtmad.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gfdbeasqq.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gxaferzif.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ghonxevrr.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gkckfqwhf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gnkzejknz.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/goankgvmv.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/guxgndloj.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gudnpbkwv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gigylsqbc.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gxswfisrs.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gqjrejffa.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gsndprptv.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gipimrckg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gmvvkzapg.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/goivxanyt.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gnfempiyd.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gkgouwalb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gnrtbsfal.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gnouzhpuc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gqmrppkgc.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gjoedrvwi.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/glfyhefch.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gyhnqplri.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gtckhsumw.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/giffcnrno.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gmtgxlwmk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gbxvolpkc.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gfviuhqlx.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gvopvczez.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/geptaqukg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gvcpwgctt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gaezbbfsf.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/guizuzfrc.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gjcqknoqz.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gunmzzcei.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gfeiblrvv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gwoqptdpz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gphfpsulu.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gwmazwwsd.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gonemyuai.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gkshlcmnu.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gguwxnrvb.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gihicmxyr.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gcfeczkkf.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gexrcdefp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gcyhqpotx.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gylarmgvq.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gsrrjfrjy.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gdpnxcvnt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gqgijhdcn.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gylqjfgnp.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gjowycfaa.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/guiiptsoj.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gngxrvljc.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gbaocttwj.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/givubtrrk.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gescwxsxa.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gfhescnww.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gqrqrbnpm.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gidluqxtn.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gqpxijhff.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gwjzlexbe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gxdehqxnx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gbcwgwrmy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gevldtdpl.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gapoaqybc.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gvnopsbxy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gwfrmnxmc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gtqeueana.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gsbftgvkl.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gmwdjrtpi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/ggvbwknik.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gizanqhod.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/giyshkvlb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gjeypzhlp.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gxkmtjewa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gntumamrn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/ghxrwlqdq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gqqwunwzz.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gfmsptgtd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/ghkubmurw.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gzyzgxtpy.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gqreiyxyf.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/ggydjpssb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gtxzwplnb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gedhftdzx.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gogcxsahs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gzskpvblz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzimzccqq.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gxlvityii.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpulbdpdc.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/ghfnqgkmr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gwdkciioh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/galgifdci.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/ghsyseuyg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gvgkorpuo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gegfthfmt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gsdwmqhgg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/ghqjcscaq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gkcihmufz.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gamjckzgc.sHtML


<!-- 参考信息 -->