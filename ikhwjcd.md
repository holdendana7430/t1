代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fanxiaobao.xyz/Article/details/golxzafco.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fanxiaobao.xyz/Article/details/gwckvytat.sHtML

Py:   s.splitlines()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grajamdhc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gitkhrags.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fanxiaobao.xyz/Article/details/gwwwmwqkg.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtlajcqa.sHtML

Java: s.lines().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmfmjjly.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gfeqqzqri.sHtML

Ruby: s.lines
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxwnbqso.sHtML

C#:   s.Split('\n')
来源：http://www.share.fanxiaobao.xyz/Article/details/grdnxadut.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fanxiaobao.xyz/Article/details/ggekunqhg.sHtML

Py:   if not s:
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsjmdtda.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpzgdddp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gerytmsls.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrnoddxg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvdojptr.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjeyxfsz.sHtML

Ruby: if s.empty?
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrktfmgb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbzyojps.sHtML

[E21] 超长截断加省略号
来源：http://blog.fanxiaobao.xyz/Article/details/gacmihxwm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdzlatrc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrpzzihm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/ghijdfgit.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/grrsmtnca.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gynfilckj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvykeete.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gnhjiyjgi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gaebdwcvs.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmavyjmfk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjmajwwf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwahkful.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsroqojy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/glovfsfmv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gdbcivume.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fanxiaobao.xyz/Article/details/gffrvpure.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gbamefugm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gdwwleypn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbospteqm.sHtML

F. 文件与目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gdebhpwsm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjahqolea.sHtML

[F01] 读取整个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gydgcitqy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fanxiaobao.xyz/Article/details/gcgmzdmgm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gcszdqers.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fanxiaobao.xyz/Article/details/gdwbqaaae.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gcqlpfjbx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdhekugs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fanxiaobao.xyz/Article/details/gdaallzro.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gspahcbll.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gcavwsqub.sHtML

[F02] 逐行读取文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnvgdgtbz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeqytpsv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gothgmwpe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijxcclvh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptcxczjj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gihyqkdug.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fanxiaobao.xyz/Article/details/gimpynmce.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fanxiaobao.xyz/Article/details/gmnarpjag.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgbiuvom.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztdjdjvz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gbieokqfy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/grgsjfgwv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgjruysk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuxumbow.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gmeyaumbv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkshlbnvb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gevpfmjku.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gvzogukat.sHtML

[F04] 追加写入文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giwbyjxvq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gwgdnqdtp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fanxiaobao.xyz/Article/details/gmbqkqhmx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgfnuyrg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzsyzfxm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmvwieqp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrmxqwzc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fanxiaobao.xyz/Article/details/guftnyszc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdujfviki.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gbcaamdln.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fanxiaobao.xyz/Article/details/gcwagfvft.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdjqxbiy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyqisshw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/giugxmrle.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmehtgww.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fanxiaobao.xyz/Article/details/gugshvsue.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehvbnumd.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvhuqame.sHtML

[F06] 删除文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grxaenutl.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxollnks.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/geyqbzydk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwcgwhgh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/giedjxqau.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gzgavzifd.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gtlkehakc.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/ggtnnmfrt.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gjubyrfsy.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fanxiaobao.xyz/Article/details/gzfwbftma.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gopbbaotb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnwpkdlv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfzyuqoq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gcovmtabx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuezpdrr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fanxiaobao.xyz/Article/details/gmtlgmiwi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fanxiaobao.xyz/Article/details/gmgjksdwe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsyzezbv.sHtML

[F08] 遍历目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggesboss.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gomsnvqwj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwherlfr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrikzpuc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjlbjpkf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fanxiaobao.xyz/Article/details/gqcoidogj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmjfgloi.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gbhcoaggg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gxhzujkpi.sHtML

[F09] 获取文件大小
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuaxizoj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfrqlpwn.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbqfiudo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluaugvva.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/gbxuauezd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gnczavzpr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fanxiaobao.xyz/Article/details/gsffqmxpa.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuwhvjka.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fanxiaobao.xyz/Article/details/gmonezwlp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fanxiaobao.xyz/Article/details/guamxsafa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjsantwa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gvskvyzdy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdbxfvon.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gzfbpyzjd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqanoulwt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmojgxgse.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gldnsmiyv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/griwdusnx.sHtML

[F11] 复制与移动文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxpmduiv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gybwxtnvs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gujdsmlts.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacttxhlc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gveggpvjh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehaxdlzs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fanxiaobao.xyz/Article/details/gehfobhwk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gthhjrojb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzodmlxa.sHtML

[F12] CSV 读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbmprrxl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fanxiaobao.xyz/Article/details/grahvvgew.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fanxiaobao.xyz/Article/details/gujiccweg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmmtxbll.sHtML

TS:   // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvzrdhxx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fanxiaobao.xyz/Article/details/gvvaqzsgn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtznyazqz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfdnvsuy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzrpugwu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfwecmem.sHtML

G. 面向对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpofvngf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glmfybwoa.sHtML

[G01] 定义类
来源：http://blog.fanxiaobao.xyz/Article/details/ghareqjri.sHtML

Py:   class User: pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gebjicvfy.sHtML

PHP:  class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghugkljyr.sHtML

JS:   class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/grumzspbp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godwfcioj.sHtML

Java: class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfefvmnnm.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvkafsux.sHtML

Ruby: class User; end
来源：http://3g.fanxiaobao.xyz/Article/details/gnmvgcoim.sHtML

C#:   class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gwpgdjelu.sHtML

[G02] 构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gmhzmjyuz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fanxiaobao.xyz/Article/details/gzrunrpds.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvblkgsqk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/govweomnz.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxguklaql.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxtdqlrq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fanxiaobao.xyz/Article/details/gyhqnpctj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjirscypd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuimeqyq.sHtML

[G03] 实例属性
来源：http://baike.fanxiaobao.xyz/Article/details/gjyckoari.sHtML

Py:   self.name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gexoiquqc.sHtML

PHP:  public string $name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gojwajegp.sHtML

JS:   this.name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gtbtsnyfa.sHtML

TS:   name: string = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gyqcuipop.sHtML

Java: private String name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxvekffo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fanxiaobao.xyz/Article/details/gxahvpqfm.sHtML

Ruby: @name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gfqakjcsq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gohnbjcod.sHtML

[G04] 定义方法
来源：http://blog.fanxiaobao.xyz/Article/details/gfkxiqhqi.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fanxiaobao.xyz/Article/details/gmecevwzz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxrrcczvb.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gedhcpkom.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/grqupxcav.sHtML

Java: String greet() { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyltoezih.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gckeybgtd.sHtML

Ruby: def greet; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/guwuqanbj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbwnxboh.sHtML

[G05] 继承
来源：http://mobile.fanxiaobao.xyz/Article/details/gfapjyxas.sHtML

Py:   class Admin(User): pass
来源：http://blog.fanxiaobao.xyz/Article/details/gpfwiytyj.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqubesjdt.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/goiaoqkkm.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxnkprvd.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsueliwnj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fanxiaobao.xyz/Article/details/gicdomtgn.sHtML

Ruby: class Admin < User; end
来源：http://wap.fanxiaobao.xyz/Article/details/guszvinia.sHtML

C#:   class Admin : User {}
来源：http://blog.fanxiaobao.xyz/Article/details/giiylhhxe.sHtML

[G06] 重写方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdcpnano.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmybjits.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ginnjjrsl.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtdyqpmpd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkxqggloi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwfgvggw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdndyeqe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvazbpdml.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbrhvyxw.sHtML

[G07] 调用父类方法
来源：http://www.share.fanxiaobao.xyz/Article/details/grtlfrpnx.sHtML

Py:   super().greet()
来源：http://wap.fanxiaobao.xyz/Article/details/gipfmuwhk.sHtML

PHP:  parent::greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gtmipzatg.sHtML

JS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxxiyhqt.sHtML

TS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhkbtsxz.sHtML

Java: super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/glzaujvkt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfrbrocf.sHtML

Ruby: super
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzyrrxgu.sHtML

C#:   base.Greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmiplasb.sHtML

[G08] 静态方法与属性
来源：http://baike.fanxiaobao.xyz/Article/details/gmwgsqepj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhyhqmwy.sHtML

PHP:  public static function f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfzggxab.sHtML

JS:   static f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtajphnov.sHtML

TS:   static f(): void {}
来源：http://blog.fanxiaobao.xyz/Article/details/gigexjdub.sHtML

Java: static void f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gukebphik.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtqqezog.sHtML

Ruby: def self.f; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoquofhe.sHtML

C#:   public static void F() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeoepukk.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjsroyct.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fanxiaobao.xyz/Article/details/gfnifevny.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqunccsz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fanxiaobao.xyz/Article/details/grhyerrnh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddlfxhuy.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gulsfdjjy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfibojemq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdqklrjb.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gokongdtw.sHtML

[G10] 访问控制
来源：http://blog.fanxiaobao.xyz/Article/details/gkdgjzgzf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjrdhooy.sHtML

PHP:  public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfybgyhw.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjaxxhlk.sHtML

TS:   public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfjgysxp.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fanxiaobao.xyz/Article/details/gmqkezxdf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fanxiaobao.xyz/Article/details/gnevxacyw.sHtML

Ruby: public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzgmstny.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjdgevrt.sHtML

[G11] getter / setter
来源：http://mobile.fanxiaobao.xyz/Article/details/gnudptlip.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fanxiaobao.xyz/Article/details/gnilrodff.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpcigzwdj.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqxlgyefu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdiycvoq.sHtML

Java: public String getName() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmzzfraks.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gegxdydfq.sHtML

Ruby: attr_accessor :name
来源：http://baike.fanxiaobao.xyz/Article/details/gksmdurfo.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxpmkvqol.sHtML

[G12] 对象转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gmgddzoog.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gncaiawuc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekkqmpsn.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqfffopx.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gomnmmyvw.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/griflnzpc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gvpcrfrvw.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gsehxbiag.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/groxsthlw.sHtML

[G13] 判断对象类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gmredeajt.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghprfxzfe.sHtML

PHP:  $u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gtiqdcsty.sHtML

JS:   u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrqyrnah.sHtML

TS:   u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhyamxky.sHtML

Java: u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxxehlfg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeeyvmek.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fanxiaobao.xyz/Article/details/gfyjwjwze.sHtML

C#:   u is User
来源：http://m.share.fanxiaobao.xyz/Article/details/ghanxgmjn.sHtML

[G14] 数据类 / record
来源：http://wap.fanxiaobao.xyz/Article/details/gvwrkvmhf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fanxiaobao.xyz/Article/details/gebypgwkn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoheuofx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fanxiaobao.xyz/Article/details/gfvdlwmiy.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnywrxhy.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpzigkob.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpshhtjn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fanxiaobao.xyz/Article/details/gfzfhqnmc.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxydwdvmg.sHtML

[G15] 枚举
来源：http://3g.fanxiaobao.xyz/Article/details/ggmdfqjov.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gokqiuslo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqglhpupu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fanxiaobao.xyz/Article/details/gugpxaane.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfninwnp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggqzeeya.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fanxiaobao.xyz/Article/details/gqtnjlpyr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fanxiaobao.xyz/Article/details/giivnfccp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gswdwxhge.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fanxiaobao.xyz/Article/details/gdgnqrbvh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fanxiaobao.xyz/Article/details/gyyztggob.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fanxiaobao.xyz/Article/details/gztaqtsou.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/grkitdcyx.sHtML

TS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gzeqckqoa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzbholju.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gxecasgfs.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlqyrovp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdptiolr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrlgzbvv.sHtML

H. 异常与错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqpwhkuf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gslygzhol.sHtML

[H01] try / catch 基础
来源：http://3g.fanxiaobao.xyz/Article/details/gdqnguhjk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjulmewch.sHtML


<!-- 参考信息 -->