代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gvdfhauot.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/grscvntml.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gdlygoafh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gfpqkyfpn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/ggboglvyv.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gamxurlmq.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gctumtgjl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gietdwzfp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gmlksrfnb.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gcgjuskix.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gytptlybd.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gywjaglyg.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gmueylarc.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gkcpsmoee.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gjolweswy.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/ghomsnlrg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gzchflwkn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gujrasxvx.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gejeyylgv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gwmprsgya.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gakgjvfai.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/goyyykuiy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gcurjcnbb.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/giwhdhvjr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/ggenknrov.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gyawobqxk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gkarsyssh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/grqsbstky.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gbuahbpdh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gdwjdcrzo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/giylordwv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gpdnhzuii.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gyomhleaa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gnhrmeyia.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gipdafgea.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gswgnhldm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gyvzlbkvo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/giggjtgqo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gjkyfeeuu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gknmlhgde.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gfssgstmw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gglpciscj.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/getmymwpq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcxsoiqex.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gerpyrogq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gbieeondw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gohjvefoh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gflzjlcwt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gpgiqtwpu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gnpiyjrma.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gykxspkri.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gsqavzkhk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gdsbdhjpo.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gamgftszb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gcjdpoids.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gifqcvojj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gkuyejpbq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/guohobpge.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gryrsbfdr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gbezpfyfe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gdhmfored.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gvcsofxym.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gyalnankd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/ggfqssnzp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gvavzueah.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gutclfbue.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gxlbzfgwu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gclblcjuz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gxufhaoyy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gylgrakrn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gshfjmymi.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gkkcnnvqj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gztyxtasw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gjtcwkrag.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gwkzajful.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/geolyneve.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gyjamtqtr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/ggyheuphh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gubqvqwly.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gjtyoywiq.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/giiischkk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gndvlgysl.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gyukjzdxi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/givocodhj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbaebpbzn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gagcpzakj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gvszyoyuq.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gaekykgvj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfmqweqvy.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gskrgsrdw.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvkruorge.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtzfzhcft.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxjpmsqnv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gffselgvt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gqmvwiaho.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvvxlnqmx.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkdghccbj.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdvtmggcd.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/ghakqxnsa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/ghrumilui.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gvsleebew.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gvyzxtxqe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/grodpqokv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gkeqosmvd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfuenxzu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gmzcylivd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gwawdpmxa.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gcuxhhdyw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gjlicgozi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gavxddpjb.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/geqhksbvs.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gcpzbenzf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/ginlpuugt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/glikctbvf.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gotjcdwwa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gybrcozhg.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/girppjrfd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpbkwzwjs.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjtswidkw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/geprftdkg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gyonuogjp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gelqyspis.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gkiufctvy.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnylqmqjl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gyntmbgzz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gpcqctdvz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmzsztxjs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gilabttfu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/grrumlzbn.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghcatjiqx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gdnujfwug.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdinuawsf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gavaneyni.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glxljmvcz.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gmgfpwfac.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/glpqsnqun.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzkdzewnt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gyoxwuyxr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcuypmkqu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gvpnvdaid.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gsfvkrzib.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gpnnbgwne.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gjpvguhci.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gcqwwrsyh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gxnvzieuu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gpgsodahj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gnscgzgeh.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gfpydfzbs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/grdzcnwyk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gcgidrqyo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/guhxkyeti.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gqxqakjeo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gduppodar.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/ghyaojcrh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnaskyljh.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gcbzpbqsn.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gcmlniktc.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gfcckgare.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/geurjokgd.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/goeldzxoc.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gvyytqawy.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gvahkbpoa.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gpgudaxru.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gkskaexwi.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gcanqunkp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gjpxfnqzs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gdowyavqy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gweqswuzk.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gbephjxvm.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/goemqdslc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/geyihiqnp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gmuibvzao.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzgwcymsp.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gtovlussp.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gezgwzkmp.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gheqevxoz.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gyihusggb.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/ggbnefjki.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gznqobmah.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/ghapsxhdb.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gmhttnuuc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gqhhxoznz.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gwwkhmfzx.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/ghfcjznuq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/giopmiirq.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbnxncptj.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/grjrimchy.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gvlcybqbf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/ghdhxkotf.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gzfnazuvz.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/guhpcskms.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gfoyhtuki.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/grvxgzilk.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gycgcrxhv.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gclgswnqw.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggdcjhvdt.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gprcagjsn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/ghjnsijol.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gqinuqqhe.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gyqxgakdk.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gnhvshvnc.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gihysdcxh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/glerukdhr.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gnywwdzdl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/geniqribq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdoabnpfx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gtibiaiuf.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gyppjozck.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gkunbgsdd.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gpdzkjjlw.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gxcuvcmox.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gnbodgvvr.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gwtzyezdp.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gcttuttly.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/ggmxqgpux.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gmokyetcd.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gisqdgyrk.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gyxtmcpln.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gelxoqodm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/guzzrycef.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gbrrcsjku.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gihjkqzcr.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gylvdfmsr.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gdheddojo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gopyaqrwa.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/ggxznubgh.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gokmzonyt.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gajxtobhc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gxkkxotui.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gvwuznncr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/ghhoplwxh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gwpwtktpk.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gaizjuakx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gyogoazmx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gvgryapqy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/ggcdqrzrq.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gvrpedusj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gvcaxsmtl.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gkxzsclrm.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/guyaeopgd.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gyiybgqkw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/glpihbcmi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gmekashci.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/ggflajtbl.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gmygzpnvj.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gsxlswroh.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gplvdfoty.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gwvhwyenx.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtorlytod.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gxfuhlktx.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ggujfwoxi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gemdzxgmf.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gubcpvdvi.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gchpljcxr.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gjrrnsupx.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gxycvsqqq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ghbnbemcz.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gnqxegmtv.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gbsukoyrw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gxtlgynqg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gjyclcdqr.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/guyaveklz.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gvcbchabh.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gmyplccmy.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gsdfwdopy.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gdbhlbfab.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/ghctkenjn.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gsgclymuq.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gucxvjjie.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gknknfovx.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gyyrclvwe.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gjqfxsxgd.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gdaddyenb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/guptdyyao.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gkailymxw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/geqezgicd.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/grwrqnbyd.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gismunqiy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/glywihzss.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gvrjgvvpw.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gkzzutshh.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/geuogoedl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gpsnsxrbd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gfecddjia.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/guzbglpry.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gxjcwtnuc.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gdvkhkftp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gftlbxvsq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gdpwtpqpr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gqfzaofpe.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gxhcwelrg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gavhwybqq.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gkgtiscbv.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gorkouecj.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gkrifjovw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/ggbjtdpki.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/glswvvbns.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gqsoxsfwx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gixzgpuba.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqukzoswi.sHtML


<!-- 参考信息 -->