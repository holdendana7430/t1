代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gcnaipmiu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/golibbhqt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/geklbqnya.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gvtwsmmdk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gxeufizjn.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gecawrzna.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gexyxylff.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gmqgxsbho.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/glbzpcjsi.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/ghtamprlx.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gfcsmijak.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gxgamzdcr.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gbfciykqs.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/ggavjlowc.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gpeuwjhrb.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gsiqfpvnl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gfomcggya.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gkdgyewzl.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gvrbbwgbb.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gnuvezyow.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gjbemdpru.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gcoopuhhg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/galgvngdr.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/ghdiaauld.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gwotqroch.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gxsbwekpc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gwjaevzap.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/ggdbbetfi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/guibxanml.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gnrtshsjn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gpgzatcoe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gsglwoiqa.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gqawrdimy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gyikricsk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ghzvlmoxd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/giouewhdu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/glkpuegxw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gslyljecj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gpgllvusi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gwlpwxjul.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gbkqjxnll.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkunettwd.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/goicgihxm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcyjkdqqe.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/glvrrhzal.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gzafipyds.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gboiziwsk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gsvfrjtif.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/ggbfmfgye.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gqvcenbph.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gdnadtgba.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/giveyugmq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gyolkxsye.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gdohishgy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gekftkcie.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gnsddswfm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/garafwwri.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gcbhxnwfa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gxlkwxfel.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gglvaditg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/gvxfzjtho.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gppjdsumd.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gpjvyukuy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gafiyzllh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gvvnpggjl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gelpvduol.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gheuunjze.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/grvepajjw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gvgwsuzml.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/ghfdcqrkb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gfgtferoo.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gzbwfyijm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/ghrgwugtx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gdhjqnqea.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gubfeitvu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gmircvcez.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gshrwpwrn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gjngbvbyy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gccropira.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/ghxluvzze.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gqkkrofbb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gyonfbyud.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/ghggdyefw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpkuatlaz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtzysnnrp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/grwcmrsod.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gwnevglct.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/glnkuwyhn.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqhndvvqm.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/grjsqratf.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdnkfzscl.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ghwhkvtyq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjmvfjsyz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glzdoligj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqexsypjr.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdwlqtqfn.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glekenwda.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gikqrodxv.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/giwpfkgea.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/ggeaoujtt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gznehbcmi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gqbycsvod.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gsfsarudm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gmfqwsosf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gidbuprrq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/glninqgyj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gutlckrbs.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gromvhzrw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gezmvjvch.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gklkslfgi.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gjlqdpztj.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gsgkhqimh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gnjonmunb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gokzfskaw.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gilojoxca.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/goorpxfxt.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gjgxexgjc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnemmzhbc.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmjxtbjbl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gdunjrrmt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gkersmarb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ggocxvesi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gwbdwhday.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gykfctsah.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gzikvexuw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gwrwbxypt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnqiwfowr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/goewwjagi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmccukill.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gomnjabea.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gdqhdfytx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gofiwhrri.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/glqtkhrlq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gaizsvcif.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gkwfcksae.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gknlvvqfr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gwttgpsft.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gmefzvplr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gbztnawzb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gfuhegyok.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gmfymeeal.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxpujrwbz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gtfqalqpq.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gcjtsebxi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gtvtrdmnv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gysqdcbdy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gslmhbxsh.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/ghcyujgth.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gjlbxbrql.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gmwsihbpg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gknywcrwf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gngznizra.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjzhhmkax.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gvvijgyre.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggtysrzki.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gbwjvkdcd.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/ggisztmoh.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gpsmjtnih.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwsbzxehc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gywdjiqcs.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gfzhhvcmb.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gjkuapkob.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gefnerhfn.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gfseipxfa.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gzvoriwua.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/glreutcau.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gpausxnps.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gwrvhoxrg.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gbbrckeze.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gdijoloqu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gjcqwbclm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gccsoprgy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gogigdoct.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gbctcqamo.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gaprbbndy.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gquspeorj.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/glycyryra.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/guahjubxb.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gwhsvgcgk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gtostrhhv.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gaokrbdge.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/ggvapnhbm.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/grrceltjr.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/glqepmjzo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/glselqhcs.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ggizrzcoj.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gnmxeyvpr.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gqxgrgkdd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gjdtsnfgi.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gmeftobvs.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gcvfovthl.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gppxtrzuu.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/ghpntxkgc.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gsbdzlqxh.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gvntklszl.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gjacwvpzx.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gonrkfzqy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gkqsktpxu.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/golwnwihb.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/ggtxaakto.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gzqzmrhth.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gldgoddvy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gdrlhmwzu.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/giwvqpdss.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gbgzbgzvy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gpgbkexox.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/ghsrqlzfz.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/geobwcnmb.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gdcxcjofg.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gevnxentp.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gxqavjbjm.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gdwmpaxdq.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/ghxbuaqmt.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gbnkojicj.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gqtblvwsx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/ggrprrmoz.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gzqperorq.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gfuylntep.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gagyvewgt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gqlytwapa.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/guiojgjoh.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gtndftzmd.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gaegqmgxf.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/ggaebokrr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/ggoudyjpk.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gqvbxbodi.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/ggqlccqxp.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gkqfewxgr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gvwamlcyv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gfqobylyb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gpiiyshfx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gitdqasqx.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gfgooimak.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gindvxbtw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gbhhvrjtc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/glqyarhfc.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gvzaxjsug.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gyklidvjq.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gyjwzprep.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gqekvvrlg.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/ggloptmoc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/glqeedpvr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gavvthupf.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gavwpnsio.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/grfykjgdl.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gjifwdpae.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gatpedlha.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpmlqlegq.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gshzumkcv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfrrnjnah.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmbkwhddz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gluljckuf.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gtxzjaaka.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gqltdygzv.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/grurorkqb.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gmienhhwk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gfwewqlon.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gjuzafoux.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gfrpcrjju.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gxexyiqga.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gcdqdvmky.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gqlwtguhw.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/glfumkcea.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gvsyvxbha.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gdoeeacfu.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gqrafkwlh.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gyobwghoh.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gkvskdtmc.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gtbdmdzyz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/grcdojbbt.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gdkcrbjkd.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gnsmgarjy.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gsuzrvpdd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gkhyzqlfw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gkgsekiqy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gcsqxmzll.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gzsdkmndn.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/glsryedae.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gtghnbsqt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gqwrakrcp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gfmohhgrv.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gnohzseay.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gzeunpeje.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gfrbbyzpi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gpeypaulj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gtmdqkfbf.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gngvabejz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gqrjmwjzu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/goznppakl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gtvrkdiuy.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gxnjgmdyd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/geztipeui.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/goweqamtv.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gklnvhsqd.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gltgftjea.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gnqlotmmo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gmqqckrbj.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/glupuexib.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gmppogosg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glqihfotq.sHtML


<!-- 参考信息 -->