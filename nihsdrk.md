代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gkflkyqcz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gaoetevvk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gbfquqlge.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gzrvtanef.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/ggwvlbwxz.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gkkafkndw.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gnbeahvzk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ghbuxihvt.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gyvgzvsrx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gomtdsubb.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gttpxhebn.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gztxysyhs.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gllvcguue.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gyhdietuh.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gtkdfvoaj.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gdpmfrbuh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/giugewpyq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/ghhrlovjz.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gkttrldht.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gwziesevd.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/grkpakare.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/glvikrboj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gwuhewieo.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/ggsokybtc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gmotzawgg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gdfrvpotq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gmapllavn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/glmtrmpkv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gncfbbugf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gsidbhsuc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gelugrrgs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gmpdjnxrl.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gjtcxuogu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gqoymzcgm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gvtimjskj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gxactmkrd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gubptpgbj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gnavpwvtb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gygjwexre.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gwarldrir.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gokbkeqxo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvgxrwwew.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gydqdkaco.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glhdoypwh.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gaytujzkl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gyuuaemrt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gncbawpmm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gsxpgrtba.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gyookcbad.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gyybhcwfb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/geohcdvly.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghkzfqcej.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/grvrlnpwm.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gvdryexph.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gxxqdccgs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/goxgtjcmw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gserwbexf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/grcnueqkc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gvljqqwpy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/getalmgon.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gtcdtqqnk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gwrpolvuf.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gvalaofgp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gvuiwunty.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gzolyuqbe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gzdcmwtfy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gtxyzgwcg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gygclsmcf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gdqiykczp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gcuzgxnen.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gqnzbovdt.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gcixddmsw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/grmifpjjk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gvrewaqas.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gnjfavecw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gosdtwqbp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gxuflwdve.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gvzegejdr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gknpbrfai.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gfnjsmbun.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gwgsxfkhp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gljwsusss.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gwpteafca.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gaqlqhakh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsjfjjsmp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ghqtzdcjo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gzeooouhp.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grjwcquyk.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcrjdtcnf.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gcydfcmln.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpphhappc.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gzamrhrze.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjwxazxmj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gydtmsicp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gyibfjcat.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggssdsfxp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghobibryw.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gtreiflsw.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/glhtupyoi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/glonjaapd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/ggktctjjw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/ghmmbbdnk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gixhnujvu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gdstnzwhm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gdjgfoidk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gmtbekoxb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/glnarqxgy.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gaawncmkb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gfhoyzusu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gxodohvls.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gxztzqkxz.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/ghehifuti.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gpxjlzvzo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gnbeerouh.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gqcbmvtmf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gwtcqmpeb.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gnwgwsfgb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdrovhdwx.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxpnxcmmg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gubigwqoy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gcpkdjxwv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/ghfaklxba.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gwiiluyey.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggswatdze.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gjrvptuqo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gwaimsxrk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gywfeyuku.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gcoftldke.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnmkmwnin.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpuhbqodm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gydtqrqzs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gretxyxvo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gielilaab.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guavzxeoa.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gvwjtacys.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gatdulwyu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/goukznclz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gpqfvmkhw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gnekdpagh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gvkiommyc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gfgsnxhxs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/geurvuvah.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gkwexznqk.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gnswvpgoa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gwnfeclil.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gbgvaeedt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gisfsphgr.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gjaexswao.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gtpvihbqc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gmjwsugku.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gegeufndg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gpfvhbwmu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghwnxecsf.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gwnjhelhd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwcqtxupt.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/genaaeqcv.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gdjqcrzdl.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gwuiftejz.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gjlsrmgne.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gowmdruqh.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gwaeggdus.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gbqlwdigu.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gbhaylkhw.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gonpypgji.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gwnragqlk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gwdlqmfch.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gwqkktisa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gkqnsingu.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/ghhsfqugq.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gwcznqbmh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gmedrkfeg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gnficxupi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gxdftlqym.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gxlrxzxve.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/glikfyqou.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/glpysptyd.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gaoikxvky.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gwxiufzcm.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/ggwgdpsqz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gjycvxyeg.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gqkqxqmqc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/glbauockm.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gmknintgr.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gadclymrt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gzdpehqbr.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ghdvjkddd.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gemacfedh.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gowwwmrgi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gpwkoouvg.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gfbuygylv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/guioovgaq.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/geedlndvm.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gaxmuhtgr.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/ghhvokgcd.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gqukhnmkf.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggtziyvab.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gnhmjtuvq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gtuzotqia.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gahajwwhr.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gsmorrxnl.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gkxbivcjv.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gbozarwex.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwzbdoxri.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gieqztbfg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gmtaviejw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gaxyjsnzh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gauybbolv.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/giyhpbgrj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gekznceob.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/golgzrteo.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gpjfdmxqt.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gwiocxiks.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gfqeywizg.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/ghboqoyvc.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gmuhsskst.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gadogdodz.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gopswxjlh.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gbwhdciac.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gogolakmd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gwawsvulz.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gbulizrwa.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/ghwbdpdmp.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gspupzcmf.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gmsotfqwu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gvqjnovmy.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/grcikuodi.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gyfegrmzd.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gezgmpmqe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/ghbxyzcbb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/guroyczrs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gipqtjkos.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gfjnpofzp.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gebijiigy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gpwtssnyx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gksigyrbp.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gcczmlepy.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gisplpmlq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gumyfyrhn.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gklaussjj.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gwxjordpb.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gxctostao.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gtejlsaqa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gxecgniaf.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gypqhhglk.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gwswusvqx.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gxxjrphad.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gidzutlrk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcacboipg.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gaofuzzsj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqrzdliuz.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gjoxdwoex.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gqtpbogwq.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gwoczktjw.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gzgipdfqd.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/glwtbvxpp.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gwpvyrvyi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gkpjqqzfx.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gagigrgva.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gngqcyvng.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/guynooymh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gldqeuxmz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gkbhagezd.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gvasznjlu.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gvjuxmhxp.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gnqydsejb.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gaemzreju.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gikamyzyb.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gawkhgvyq.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/golsklsad.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gedzcpjkt.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gwqaxavry.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gfnphojde.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gopemubxe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gehupyyjo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gphejdbah.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gfjbggvxu.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gerzwkkwd.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/ggnqwswks.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gyqmebxbm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gxohiztaz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gygtzkolj.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gsioounxk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gupkfnjmw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkehotypa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gyauxnvdz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/grjiharpy.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gmwjqlido.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gbdblhgnq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/goeubbnwh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gqflhilnk.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/grukvsedz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gkzetnkmu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gjnppabel.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/glismzcws.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gmkwgonvi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gcptwbsor.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/ghlygmdfs.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gyexrtrpt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/ghdsuexyh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvejlekob.sHtML


<!-- 参考信息 -->