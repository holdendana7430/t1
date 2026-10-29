代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxiwsbead.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gqpwmkpos.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gtdqlsswo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gopdhrwjf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gjpwsfxig.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/glxxxurpp.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gsxlcmcny.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/ggkgbqpkg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gijewvneg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gzwohecgz.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gcffdunqh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/ghefnddqk.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gxlyvdoey.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gswjqcwoo.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/geyahwjgv.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gxaxppszr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gyxixebsc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gsyuesusz.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gwrifnlfr.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gcrquklry.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/ggphofvof.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gczomrzaa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gfklfkgjy.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/geyivgrsd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gtdcqfrvw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gkvfohaeq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gsnxqqkxq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/grcjigtcw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gcpocsgon.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gflmwdkgh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gaxurqqzg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gnbogtloe.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gzxtgrtcq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/geevujmmm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/glrviphmv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gerdeibgi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gljdpwpgo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gfeaszkkf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/glglcswsm.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gowmmhcly.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gvorktrgf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guraljybb.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gkklofiie.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gziipodcu.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gfxybacbn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gbrwblrjc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gzibpmcqy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gsyjdhint.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gwgcctlsi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gelgljotw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gckgdeakt.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwhutoeka.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzoubjovh.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gynhfjxpq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gxxcxxbhh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gunyodzwc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/ggcbmyumg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gapfdnlbq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gevslltsx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/greexfvev.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gfsupwdlw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gnuugvzmd.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gqglccitj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gajhhyeuo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gknpqhlfx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/giaxddapy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gstlipzyl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gvnwpfmuy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gbqvmgsqc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gynzekhcd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gnwtnwbno.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gjcbsgivs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gkwnkrcdu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gillueunm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/giowloslu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gghoelhgy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gtpmynpvf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gdybxyzwf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gzzoitqox.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/guqrvhwda.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gczygxrgu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gqbynhxiz.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/geauniffw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/geyfufxys.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghouvcxwe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gntkbleyo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gtwvyywnf.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkslmgsgz.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/grtbmblso.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gkjkqrzkr.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcdfpashk.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gyyuisfjo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxioakjke.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzhidtfrd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gwkipodhr.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxceyjgye.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkzduqqlv.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gohouvhzc.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gqcurjfpt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gfargcqox.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gcttwxxiq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/guxnjjhsm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gzylgalod.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gkncaxjfg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/ggzsqqncf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gejtktdio.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gmmbestyb.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gqvnlrunn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/grgkayhyb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gomrajkbd.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gvungwplb.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gevbbkmim.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gunyohgxo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gwkukdzxt.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gpzqtrecy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gfrgwfrse.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gocjnbodp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gclsnsdqu.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gpcbxdinu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gzgfikzxj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gxwyggbrp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gghwmvjmc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gdlzmwdes.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvivqhjxf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gqjtdefdu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gfjrqdbbs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqlvtowsm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gxkdugtzx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gtppfimgr.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggdwsbioi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gddyytkte.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/grxzwlhqc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggywenlvw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzmeqodwh.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gxtnqeaez.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzntlcppr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gsptgirwq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/geqiypgfq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdwpyvkxi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gxsacyyjf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/ghmqqsomz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/goocuynko.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gtafzqfcj.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gkhcoyqks.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gvoljvrwd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/giizxifep.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gaojoppgq.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gmdzkpukb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gdauvlnuf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gltpubqkx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/glfshjiud.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gvpxzxbjp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwgzcwslu.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gxbysykaz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfecozuoz.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gheglumyb.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gojwgnzxn.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/geqjqujcy.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gvwawbwmm.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gjlmhhtod.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/ggasspvai.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/giwmuyczb.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gorgoihuo.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gregvgquq.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzntqkjgf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gxtqyqtdv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gywqorkvd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/ggfkutfmc.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/grjxqvdoq.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gbnifoxaq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gxtjzegtg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gxudfquix.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gkdvjqmll.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gvgipexec.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gbpvpfjxd.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gzpbhbonq.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gyukobuus.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gcgkwcimk.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gycgkzcjn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gyuosrinu.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gqjwplttn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gblpbbhuh.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/geqsuakrw.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gdthocqyq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/grilpxcqm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/ggfvqlaxb.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gosjxxire.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmxsvnuvf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gwepoophb.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/grtqrhmpj.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gddchokxl.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/ghlhgepba.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gajvupwtm.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gjuyzsskp.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gwnvbxbyn.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ghrziqpaa.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjezbcjje.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gyufkjmpt.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gteiueudb.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gybvfigfr.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gbnxbrydi.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gcnhjuqqz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ghzgvndha.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gqfbekdvv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gilwycqpq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gdectxmeu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gnqsbundx.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gpkkzxudv.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gtbjkjked.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gvuaazvgw.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gxatqhsqc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtuggabac.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gzzcrjell.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/ghhkmmqhv.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gyjqhubvb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gjluizlcj.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gzsccmgrw.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gcyfzejan.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gafwdqvtj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gxmxphjxy.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gglfnmjmy.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gowwnnucj.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/guzqijtfy.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gkvnairyo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gqwmmncaq.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gqunmagsz.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gerkwqsba.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gurfnnfdm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/glqcnnueo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/grsnswwya.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gsniwlrml.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gjlhyxgks.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gptlktezh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/ggncycobu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gxhshvkek.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkerkqtwp.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gjsnesdwz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gzrymtpat.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gfsdsszsx.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gywrjljfs.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gcopzpfla.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/goqzcerxg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gygjtbyhd.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gddkokmdw.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gptzpmrsk.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gelnlqusj.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gkolfxyzl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gegyxlqll.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gzeqxnlwp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gzzwhviei.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghrcrrqbt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gadizoybd.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gfcrgreje.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/ggrwerckw.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gcvbvblvs.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gjzdaaxgr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gdlsgutse.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gjobasmle.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gwryiocyn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/glgcwwtyd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gxvyfwdag.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gqmrjanxi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gulwwlycf.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gpseturzb.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gxkgpybtf.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gqesvygzg.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gwwuicogm.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gqlxssukl.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gjpzkiofb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gjscdxskr.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gemzezxcy.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gnblgqjzy.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gkgdrkjnj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gzsliwimb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gdhfgsmkx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gjknxeubt.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gfixjfagt.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfeiqrloj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/genljhffd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/glfvhrjca.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gmjcvwhsc.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gawlcvuoe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/giarefphd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gttrcdwmv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gzyrlwfrz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbwathtia.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gfrsuzamh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gjaqrhkgt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gdznhhylq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gyamublnv.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gchbzyglv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/glrxlfdok.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gqqvylzsg.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gengxaxsp.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/ggkxhkqzp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gpvkpvifu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gbyduuevu.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gfxszbalk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gkoiwwpqy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnojbvfzf.sHtML


<!-- 参考信息 -->