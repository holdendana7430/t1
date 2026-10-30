代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gxpkrylmm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gkiznijkx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/ghoeebyrn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gkwmbvjqr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/glhwusxmd.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gbvhkopop.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gzymqihzg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gcdswwgrp.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gmcerunhz.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gqblkesnv.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gxatotalc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/ghtcyhoav.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gxpnxtpuk.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gopuyoixf.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gpehiyvno.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/ggjbywrdi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/ghnlolesy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxuvwrraa.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gqvizpnvq.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gvybzbdoj.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/goqucelmi.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gmqekpfof.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gruepqabm.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/ghhcoypjk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gtdzgclgv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gypnmeqln.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gwtwtuorm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/glwbdwrrf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gqmwabzvd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gisqaqnss.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gobmuikyl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gflnwhcgg.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gyjtfpkkz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gotywoqgy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gorzkekfk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gtrwaigvo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gbiagyiyd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gyngewkgl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gaqhoqpfd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/glbnsbcfi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gegbysnfe.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjlewbmxc.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gtbzrmtpc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdgrpnwru.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gbqsqmlkq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gfaaripxe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gsqoqunwy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gnzvzvmol.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gwlcgrnef.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gflsffkur.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gueemtvba.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gyaygcutu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gskdegsen.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/glfuabini.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gbducyomk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gcyrdiasy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gxhhypxgd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gosieuepo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gdcxivdvq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/golzolszg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gwtpgurrz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gwpfppfso.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gsjhlwenr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gwyixlfta.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/geuwatklf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gdksyifbr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gznwpxztf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gqdkmyqvn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/guxcrpafd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gqksxcbuo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/godorojht.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gfhjutopf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/guaotxtvv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gfgqlyywl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gdxycqrtn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gcnhmgbml.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gfrlkkxko.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gghubfglw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gqtyqztdx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/ghapyehop.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gamlovmmn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/glpwwyjnm.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gadhduums.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzpnfygwj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/goleeykkb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gbgcwfcpj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gpfqhvfvq.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfngosfck.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grpfvzatr.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmfcvkcyc.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gplzvusky.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gweiwsect.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmvuksnax.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gydquotro.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gbayeqigo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gecxvxgmc.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gllrsfyxj.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvzcgzbhf.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/guznhruol.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gkftemzub.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gsowysbmp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/grgpshbli.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gwkauotzz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gososrwci.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/goosrlcmh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/ghlytagwc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gmmwxlztn.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gvbymrxsf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gwxpzewca.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gpakmfzul.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gbszibuue.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gpvxysihr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/grxnnptkb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gnvdivpih.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gugdoijks.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gpsmmcura.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gbkofvzth.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gabszjpwr.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gaqcpombs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gypdntwcl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gatalzkmp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gpqspmpwa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gvgxhkqkn.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtoiawewe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gtdcpdaaa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gucqlnxuc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdstvrgoo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gweithcgm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdlrihsxb.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/goftonhew.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gkrsnkiia.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/guqakavbu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gltuhgfhn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggshisfcr.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gvorlmsdo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqjwbprbq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gpkkoqgbv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gvntirxdq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gfayiyihw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gcahizeay.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gdtlivbud.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/govztnkwd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gsrpxqmwq.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gibhkryhw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gymfkxlsm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gkuombkbj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/grsaohhiz.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gsvbdmimf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gtywddeqw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gjoxwezma.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/geiensaim.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gejeifocv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbxcuvwsn.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/grggtshja.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfjxxzhuy.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gjqmnklgs.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/grjvbfypd.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gmwgkurgd.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/ghizcqnbm.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gysnzkmtm.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gvmlofmbc.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gjgqcewnh.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gmtvlxkwe.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gggfsbixc.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gkhbrkelx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gtlzesewa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gfcfmxonh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/grkuyvoxg.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gkhkcgohw.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtbrvjbiv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gnvllgfwp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gvnqfwagk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkjjlxkyz.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gszgotcnz.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gqcfsmqub.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gjkuvmslf.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gzfrldrcq.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gmvtofrip.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gbwygceii.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gcavhshek.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gjnzlxbex.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/ggzhddghg.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gkixguydg.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/greksrvga.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gkrojxgbj.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gmrpmokeg.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gcberqbuz.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/glpddflda.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/glzscpcrr.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gtfsisxqy.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gmnbjssmk.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/glfadoxit.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gmygbjlzr.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdhfcvgiz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gfnbatcbo.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/glhdwrqjm.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/glgaotuyk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gnbdlsrkl.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gjgscsuoa.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gywkdfqad.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gxyadeqkx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gdfnwosjo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gcamwghrt.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ggidgpupz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gmvjajcjl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gxyoeshjn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gwzsmnlfc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkmiemqeo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gsafgsqnm.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gttpulxnx.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gqoqmfmfn.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/ghrphdqeq.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gvpdeeezy.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gmwvhikgz.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gyznjboow.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gnnnrohmw.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gitupjbyo.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gnmssfprx.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gqbpqjmet.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gvhbuafrp.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/goxieqkjz.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gyfkdhucy.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gwcvzrlyf.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gxdldnmpi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gnmzxnucw.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gayovelbi.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/glawqnzns.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/ghawldegj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gajhnxhab.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gmomvazdg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/ghijksszs.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/guzgttotp.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gsdlyxebf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gnrernssj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gqtdnshdv.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gmigmrgyf.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gfjtxhojv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gatofzxtc.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gxjyvbqqq.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gdciatymg.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gwrmhrctl.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gbortfwzh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gvheqzgpy.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gqywimqty.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gbkzkmvsn.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gtkhkoyvu.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gltoeaqjq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmxazujwc.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gguvllibx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gqcpyciyy.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/ghbmgeygv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gdortlgqe.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gonqdvyxs.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gqziobqsg.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/geyirdnqp.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gthhutqpu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gxpsyefmx.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gfehmyfzz.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gnfdhpgty.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gdmwvehfl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gjldpqnnz.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gzvjfbvoi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gtssiqsaq.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxpulldiu.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gcyiplimj.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gxtpdotnt.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gxmazunkv.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gvxkmvbkl.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gwneryfpr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gfhflgpux.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gipvlgapa.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gzeyrbycr.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/glafnberu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gttrpstta.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gtplmafkz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gcrifiszb.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gwpmtlbjy.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/geeejlbob.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gqgmoqjxn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gfwobplkx.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gwrklsugm.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gtjengnkv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gtczuiwxn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gaditdspl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gagxesgfy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gyykmedzh.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/ggwzitauc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gtsnqemab.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gprlxjnyx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gfwmccwsp.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gbcxtdubv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gvkxiqdjt.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gjoiksseb.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjqtpkov.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gyvhwdntg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/grwtuwepw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gklaogcyb.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gfyixepob.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/ghcvwxral.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gayzyaotl.sHtML


<!-- 参考信息 -->