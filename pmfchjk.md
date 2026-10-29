代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gzfidlbqm.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gowcrzhjv.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gkncxrwtx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gcewzejvj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gdtbiyxvb.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gfzyqzyuk.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/ghnvzescm.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gfmkdhmvn.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/glqndhqcv.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gwlutusmk.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gzmjtfrur.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gmfffkxre.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/geqjehmpf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gtihsmbms.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gqddylvqb.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gscjhyeyi.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/glqmwityk.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gxqdpzuma.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gcrjgrssb.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/geyxjvtbe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gzytrlcwc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gqnurmxqu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwdikcjcq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gxekegqwi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gglcuhfbv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gmelnrkko.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gvicusfhv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gzyfgdamu.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/geoefntgr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gvqnhjwup.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/guacwnain.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gicrcgicm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gfkysmxsy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gpnbavknm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gchlwnltz.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gqfxxyqlr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gjqberady.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdwmcupoe.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gwuhrnqpu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmmbdilau.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gcwrsfwds.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gzbaalyyn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/grptnxpof.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gaisgksnr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/glrqgwcxm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gvevaxfzi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/guyfzucim.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqbfseyfh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxxzhcivj.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gvtchwxqf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/grmitnfxa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxspmjzw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/ggntbjcft.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/guuxhiqeb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gfdpukrtd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gyxnpwmxe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gllkgzyzb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gzrqdvevu.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gpcolbkpx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gjzchvenu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/glyqjblwo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gmdefufvb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ggmeyitar.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gzyfrqqod.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gqukvfexi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gyfdfmnvt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/ghfatkiqg.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gzzqnxllh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gguonplqz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/guivnrxir.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gjmkucnvk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/glhsiaohw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gcjjlcfyq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/grzthcodn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gwtakxgos.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gnbctkkap.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/golrxokpe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/ggouujrfj.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gsynleari.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmosnbttk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqkzwefbc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gdeansmsx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gelteirau.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gahjfofyu.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdigakgdy.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/geduczepz.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gowpouyca.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gkicxcumf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gucozflez.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gffrutxgm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gbocdmjzk.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsujjvdwv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfeluyvrn.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/glbjgvcyk.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gswdcuoyj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/grqsvomav.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gegwlhbwf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gqxdqnmes.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gyxnigtvl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/ghtejhymd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gbetxpgym.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gyrfxbxpc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gboeixyne.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/ggjalmctv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gvkcddmwq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gujngnjyc.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gamdoqwzt.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/goseyasrs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gcsklcrkj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gdhqzkcyx.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gbnbotrgd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gcdzmmqnm.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gglqwwpdt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gknxsomtz.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gwdbgzwxd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/ggxworvrg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gwrwiiuif.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gbilvfwvn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gdvjsgqlv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpowcnqul.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gsrghtmhi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gxolbzdfh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/giyewsrtp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/ghatfoixq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmtqlggtc.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guglwepdm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gjspjupki.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gffcusfit.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdckzqbuf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gozljdbes.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gjwuhccfl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxjtloamh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gipgolxzm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gkpzlrnhj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gqzwjmbtx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/ggjvvnpzg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gcygzysqz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfpbndjbn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gymynrdxz.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gslcskzty.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gnfmtktux.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gevnagqqr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gjmefnhyi.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gfgyzlmeh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gwztrsiks.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/ggeyhleps.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gcljfbmem.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/glorurptd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmwhemmvk.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gzpsiwtaz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geqqwrowx.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gqpenhtbz.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gsxmnmxxl.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/grobmoksj.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gzymbmbei.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gnwgzrnvw.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gfkixwyob.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gmnhqvxve.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gyxblqaod.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gbuijvuzf.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gdaqnfolf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gniwbiarj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gzvpcfmxr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gptrjrirg.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gcrygshvs.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/grlijgxff.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gftxbuzzw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gvnrhxxna.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/glccrnoxo.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gzkcfacyg.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gfcdaxtup.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gvsaeuebg.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/grmejbxva.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghxlfjhhw.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gohlqqbob.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gdlxrvmbi.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gifvgrjrr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/ggscgaecx.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/grbgzhdvl.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gagyngucr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gjdvduzmk.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gacndnmcg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gflntpwqj.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gyiegrfat.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gmrnllsth.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gckvjfdpy.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gaobjddtv.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gyqasnptp.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gxyimurlc.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggjqsduej.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gemblebun.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghozscezz.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/geblcbpbv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gdawtryzz.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gqnamsmbg.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gmiokyoim.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gwmesycqp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gqjtjvuqo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gwebmcjyd.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gpyfegvqs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gnlurrbih.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/grivnvely.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gjjkxxadt.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gdifqafga.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gcwkzfwsg.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gnetllypn.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/ggxlnmcff.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gidsumycb.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gokmqrcmw.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gwradpgbm.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gfucfbumo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/ggekfstsh.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gnotqqnci.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gtxiyhnyq.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gthszccfw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gepiohnhb.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gvofwuzhe.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaqpjnpor.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gawmjiobj.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gecqekryx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gianbbqdz.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gilasnidb.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gralicrgm.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gjddemiwi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gduuhjdiq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/ggktetccr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gweiwzunf.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gcvwasehd.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gyqpxvdjb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gahgzjjdw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gcpcudgyd.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gecuuhgun.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/ghksnenbo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gmbxadaww.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gquuhhkav.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gaastplli.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gzthcvkju.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gckhbmucv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/goxrugipk.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/grkjrdshm.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gkvhwxheo.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/ggbjomqkw.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/grxliradd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gxrcdmcuu.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gqcgvgyhw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/goqruizvh.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/grtbmakqn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gdebewcdn.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/grceslpyi.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/grbfgjklf.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gngngtbce.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gsilherma.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gznpzuzmu.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjgvgktat.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gyrlsakzq.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/glkkwsbdm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gmjtzgszz.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/ghtnhyujr.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gvpfzprok.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gfebdheev.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gbkdgnuuo.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gpotquryq.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gksbfzsmn.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gqplcpkkq.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gultgiswl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gczdjobvj.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gkcetutts.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/grmgfjsci.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gafrqvjlb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gxdcsfnkx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gdqwkqsvo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gtktmzhgd.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gybztlbaz.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/geepopawn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/ggwtghcjs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gixvlkpgm.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gdgcpnclc.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gkhxeflvf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gcxkgordb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gqnmshxpo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gyiqlvrfs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gmugytuud.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gqhsmpidx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gyejlkust.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gfwcqrjio.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gzjnlgaxu.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/ghhysnvim.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gjgqiitnp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gajizoisz.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/grtibkvkk.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdcyvvhcz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/golatrirb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gwaxlracu.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gyyxysmhc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gzvvkeucs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtygbrnih.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gqjkjhiou.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gstuquuyx.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gydhcmzla.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/giwzpwzgt.sHtML


<!-- 参考信息 -->