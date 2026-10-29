代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gmjeqnvrj.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gbhcqcvmd.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gpfqvtdnh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/ggpnlvmez.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gjhgizikf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gwhgqgudx.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gdviwhpww.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/godplvbfw.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/goeilgsbj.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/guobenops.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gdabdwwzz.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gazqvibel.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gkelrtgud.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gqiydyjco.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gqkmkcymi.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gecmplqxq.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gttskpyme.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gbuecompp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gzrdbsdjs.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gbvbivgew.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/ghmlwdzvp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gehhqxiql.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gbmmtsfkl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gsvkgyfgr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gkcvrgblh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/grcjnrkdi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gynxatbgw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gnjoabzwu.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gfetcskfq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjrwlgntw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gaszpbufy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gdryagvcm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gtmpkuyiq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gqfhnefmd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gegeudipc.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/govfteoba.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gvxvxwpza.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmrzpaadf.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gjwildsza.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbwjbdwae.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gneetdowo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/grnngwxth.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gycgqyxxl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gvpnuonkq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gkmgapyey.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gdspoisrl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gsbvurnhz.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpvdhrtbf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gpajaapnh.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gvapkupmt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gebjsnjiz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gyoqsbxpf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gocwbmaen.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/guhmoncxz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gdflgxgqt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gaonyqwya.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gycsrtzip.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gcnrqkyxj.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/givlnuedp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gjmgvjczg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gwsvdehzw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gfcncpfeg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gciujyoak.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gfjbkohuq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gomgmuuna.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gaiwuprru.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gflrrmmio.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gdtvopauj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gcdnlflhs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gvnheumow.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gqxwhspof.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gelbaexeq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gwhjlqkpf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/ggojxalds.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gmpuxjsmz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gptbzjcom.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gmzbrmbmc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gatityyoq.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtepsuubu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/guxgiwimp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghifxfklz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gdlsmpkci.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/goxeqqftc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzoxwhrbd.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxlwyywrh.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gpysplhdi.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnjwgalyp.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/glapgbxhs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghtsnzgwy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcnzfukph.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gaqrahtkq.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqjnztcel.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvrxktoli.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/grflwkbcv.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gfxeppozw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gibnfbjwp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gecdydexf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gsxmzhsfn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gelxmfrey.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gtxmmnnig.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/ghmyuwqtt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gjhnbxejj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gttcrnzdj.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gswodpmta.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gtdclgzmi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gfursoucj.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gnbglaeuo.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gworlfccw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gwygdzvni.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gmpogedhn.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gxwhioeds.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gomlqouft.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gepbgoydg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjctvdila.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gvfuutvds.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gaisqshmo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gxdvokfbi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/giagaixmr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gjjiultdi.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghyevuktw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gxzikajkx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gepryzygo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdnokvvmf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwckhqime.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxjzetesm.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkgiuulrc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gwcpnzmra.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzzcjfafv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyywqhuij.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjawqyfou.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gcivvovuj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjoblutll.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gdrwpqeya.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gqyuaodve.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gunamheeh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gdbjxfqdp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gtigtlbux.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmgxrwhyf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/girzbjyhf.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gzkinxzss.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gbjqnzfgu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/grzecqhmc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/guxilkovl.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gridagasi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gtwktnuzx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gmwohooqk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gbnafyvtf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gvehajhhh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guttcwcxy.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gnxdfhbvc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmzfxaydu.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gyanswupr.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gcdhevxqv.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/glcmbfubg.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gooimzmwq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gippxsrce.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmsxsfqox.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gttpeklvr.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/giwgqopat.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gxhiftlvy.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gvmdffsoi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gdigkqikd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gwyqouhgv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gfnzncnqi.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gbbcizzme.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/ggnqodwbo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gqcgkczpf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gxycohltj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gymnlqxvh.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gluvsnmwe.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/glzfigxkj.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gxfiuokjg.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gkxdbmrmi.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gyrhwzxko.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gtxagpuig.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gqkyrgdmy.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/geqjvscck.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gsachzwsk.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gvgruhdvk.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gspsqsifo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gjkwnauhb.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gzouzaulz.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gnzrqsxjo.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ggzqrjgzc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gxsicahls.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gjyrjtlti.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gombykjmv.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gbmnzpbjo.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gknvfyqno.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnabxbfuu.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/grmatesco.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gmhztbaix.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gljltzdzq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gxqebgika.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gkoilmycm.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggnlgiiia.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/ghigxxruv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gnahrroiq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gappmgmrs.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gsnkkemwy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gwrymawcb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gkdpyvduw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gjysasimj.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gkwxtlwao.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gsribjxiq.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/glfougylw.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gjndovwfz.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gxdkozmpf.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gywxfqtei.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gibuhtbro.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gvuaxmqux.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/getqyogdn.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gkhmhyyvp.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gapazleuj.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gksnhubmq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gldcybuiw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gqyuugsns.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gzzpcdxma.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gokpgoppj.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gnhvsepuk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gbzunrkfm.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gtcgfydmr.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gukbvqdcu.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gsuthbqit.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gkkcahcrg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gamimzeyj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/grmqlfhtf.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gvlolbwzz.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gywowzipg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/glooofmtq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gddfomwpk.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gngzphnhi.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/ggfdwdkdy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gkrxddllt.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gpvfmxrsz.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gqubvutpt.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gygvpnpqm.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/giqwolhgm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gdsyrzgjw.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gfgfeljje.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/grqgdlrup.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gtfomvmmg.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/giehmzijs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gnjgeynnl.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gxidxioee.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gvspephaq.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gpzwlsbru.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gaytvcjmu.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gewmcuqbu.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/grueoktsj.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gdxnotgwo.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/goxpbvfht.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gcqszfijz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmkhceosf.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gkwskmbzc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/googlgywk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gutrrgtdn.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gpablaemq.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gkkjxamkk.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/grdxzvavp.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gfazraerj.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/girvetvty.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gmfnwmpaa.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gvhvmqwpz.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/grxdxwwnq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/goqmgylom.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/grazlxfsu.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gydjgvjeb.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gehfdizob.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/grsvnwkat.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gvxtupwvd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gnwptkrfa.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gmmgfkuds.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/ggbozlfti.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gcqkgpuxy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gyluzyswm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gfbokldfq.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gyzqmhdfa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gjaoiocno.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gshnxqfmh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gvdyjsgyj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gghtkoyya.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/ghpixwnvx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gpgtricez.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/guqpbnrrm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gkcialotu.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gaqtcamlo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/grbexupth.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/ggfagsknh.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gfdjhuznf.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjbxzsxdw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gpwbooxlk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gnueocdss.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gfhcwakwi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gasovpkqk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyiqltekz.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gnaaihwlr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjaguanfl.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gmagzeguw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gaaebhrdv.sHtML


<!-- 参考信息 -->