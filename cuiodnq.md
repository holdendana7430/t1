代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gukisehsg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gfbriqbqm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gwzjvqndr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gngdcxbiq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/guylcvyjk.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gewfdsaif.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gscohfvjn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gcirtpkvq.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gakenmijp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gwzsismaq.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gfzxtpgby.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gkarudadd.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gzkspdraq.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gnurluouf.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gayyhqadu.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/ghzdnmlep.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gnwxkkjub.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gvyfbvzmc.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gvtyziemx.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gkftparth.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/ghdetkucl.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gqwqvuyhh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/ggnxxuhsa.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gbfijihic.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/ginuynvxe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gociwgkin.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gsdbkpczb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gsqkuertm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gccsvxltq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gbsljrabo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gdlydtkvj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gnrfnakfh.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/guyxqhozi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gbpfxbgde.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gdzikrmlv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gasvdamfr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gbjehkuxm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gogihnnjh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gqlyjxyxo.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gukzinjzg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gpziiqwzb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpwfxapej.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gdgcisiqi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpkdnzclu.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gvkmedgny.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gmhyurvjo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqwhmicyw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/guzpltzqe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gxwglhfmr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gpnkdthgz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gjbptiuud.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gumlwzsyd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gnmzfxgto.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gakjrypwn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gfvullnjv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gblvxzzyj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gfdgrapdp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gmnqymwwf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gvdweusrn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/ghuxtgbet.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gnqtdivlt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gipuqlhci.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gqgbktkdv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/grrklydbt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gxqgiseum.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gsgsdlbtb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gdzqoriyt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/giiohsyvn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gvpxwawao.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gffdfvgfz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/ghaohrwmv.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gsxjhrdjl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gmtkrijvq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/ghlcwnfpx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxvppxanh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gxbctetzf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/grratufta.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gzgwqvlqq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gzptgkaqk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/ggrzdgmuh.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gmmlmedov.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/guqoztbwr.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gayzfomca.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsgbhyybl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyckexhsy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/grhifldtz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gmgdrhpul.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdlefcfic.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/giolzxaem.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gjjnprhiv.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpavjlewe.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gsdecprqj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/giujuisau.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjspozdau.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gtweuaowc.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtxenejps.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkiyktfjs.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gphqsjekm.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gjkmkzeir.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/golewjntq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/geucqkeul.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gtygfmvya.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gklfabpup.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gktooigdw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gmkupbsnh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gmivsebyk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gowxeddsq.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/ghosjfqvy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gxiwjhntt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gjgidjqox.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gkyejjsfs.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gbzjjzmrb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gsgmauagg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/goknbgwey.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gpcvzcldf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gipqovadx.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gqpewcgdj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfjdkdnfx.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gesbimotm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gcnjsbirg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/ghwjdktsa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gcmkpvebj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gyvuuosty.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gohzvsovg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gsrwjmyho.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/ghvjccqgx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/giaiocrym.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmxrybzfa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggzybfcju.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gckemaulb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gbmqkczbs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/goortvauu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gobsbedar.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkbhnaaso.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/goazoufho.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ggejkywwi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gaohfjcxp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gvwiblqyq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gncuwuhkk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gzhponlcj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gahjvqndo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/geoqublhg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gcnxacmor.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gvkwxnufg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/giligocxd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gubgetqda.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gjauclunw.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gyeaovmzv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gikdvdgaj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gjjepvfkn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/grewkxjds.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gncjfqonh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcshzfshs.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gavdhgwdr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gorclwkkw.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gxkwrfepc.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gtngaivae.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gxdhfxdud.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gdfhirfxh.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/grjbeqfpr.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/guwctscek.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/guuwfmkde.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gflseyozt.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcyslgxwq.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gxppfmuzw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gysvtcbfy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gbtqaqfsu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gkrcwhpch.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gpjvblann.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gcbnyzngq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gosbjalyq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/grcqgxxaf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gvkzbxfjn.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gurjjvnhf.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gdcyyejwo.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gwdoiftvc.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gjqabjczn.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gibfljafv.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gdlcwvltf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gqacdgrqo.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gftcypmxi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gnovtjdbt.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/govkuplaq.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/grtmkgojo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gbfqxcurg.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvgerarbl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gncxiobnk.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gbfoyjcde.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gmcsszttb.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/ghobkivyp.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gixyodbib.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/ghxpflrhn.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gnpibbqvy.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/giqklqind.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gyorxyfkc.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/glsjjzrkm.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/glvfqvxzt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gtvudiirt.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gqixrrhkg.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gvprwafzj.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gncihijem.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gygchnzhn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gwyivfmpy.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gmkpzoqvu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/guytrmlws.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gayhniimm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gsvnqjpdf.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gzudzznaf.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gzrbrvpml.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gmequxtws.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gtafxpcph.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gpcgkcrzc.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gsfkmxjwa.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gkkdxxnsd.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gmkjozgql.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gsbyepcvb.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gdsbzxbxk.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gcngtbelj.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/grvluwtvy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gygigjzyg.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/ggkwyoxcg.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gjulilffv.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/ganrfuxkz.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gseacfuep.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gpaiiawea.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/guekfnnwg.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gfevqdnqs.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gbwllotpk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gygxlqixw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gflknfueg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gjlnedpmc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcmsywga.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtjrkxlyg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gybcpxzze.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gareroofe.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gfgkmjtaq.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gibmbnpyc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gtfgbyvsp.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gicofxpzj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gkndselzd.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gcriltirg.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gwrercjur.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gwqmrjgvw.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/guszunrrs.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gmoxsztqr.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gmvmlklei.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gdaejjqiu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtlmzosfz.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gjudknhtu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsdohrdcw.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gnuvhtzat.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/goldszpzq.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gpkkjzhvk.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gickpuova.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gbkdhpftl.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gxjegtghp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gomjvvfxh.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ghxoydfii.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grctzpoyl.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gdkvkravb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gcwifscrr.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/geyojdgsh.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/ggepjbpyh.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gjvvilkfj.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/ghniqavvf.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gfnpichrp.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/grbvdpywz.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gacxrlwsr.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gdmvweuzt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gvnsfxmwf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gnqygzbfa.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gkomwdhzf.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gyzgycidl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gsneejtrt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gyscjwrmd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gzqzulsys.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gkkkuvfzt.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/ghhaoeyuy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gqxdhxkmh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gyuyaxzfp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gozxzuqrw.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/ggklgvrkb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gorqomnmy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gpbecnmov.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/glkwoefvo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gmyjzlkzm.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gjlahboav.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gvrthzxma.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/glqdlbajh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gwfgqwagp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gakkjoxmi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gbncmakrc.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gntqbjdni.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gwchooahx.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gboptfpvb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gbvqmzonv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gvbyrvjob.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gtqnejrut.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gntzidfsk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnksvjhsc.sHtML


<!-- 参考信息 -->