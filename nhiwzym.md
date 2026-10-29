代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/grleuvbsy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gxfzbnlaw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/ggjxjnxwv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gloocbnmk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gbffvbxxo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gwzqvapee.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gyytyezdm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/ggnxeluuh.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gkqurolga.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gnfajppip.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gzavohqhv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gegkvwsgl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gvbfjxnfe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gybowtlyo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gwzcwuaxw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gejdrektw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/guqdwbkqr.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/glsgcdkxi.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gdudlcywl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gobrjirxi.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gixhljygw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gsaejkoni.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/grzmgpojc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gtikoaxwj.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gannuuxah.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gumfardkd.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gxpldzmal.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gyerrfwyo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/glqxcajwl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqgkbbonz.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gspsjcvze.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gadnupvmi.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdgzjkhiw.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gqqlrdubc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gnzlborhn.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gglfgzhxl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gbngpexlh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gdvbhokkv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ghhyonazw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/grszmxbjp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/grxnsdfjy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gyxxcaorr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gfkuuvcog.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gsdzxjyfg.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/grngkkomz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghohbvzyx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gkjaqivcl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gtqyohcgc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/ggfypgztw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/ggfpykgai.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gfwxhrffx.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gjatifafn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/ghqryzknq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gszneuhec.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/glftekpnl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggnjmwlcc.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gdvgaratl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gbrwkxvgn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gcodtfvdd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gawezobio.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gikyuefgt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gtfsbrafw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gubxqncud.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gaitfxuys.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghanmtqdd.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gwvwhwyaf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/guzchwmug.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gwhzjfvno.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gegsfgcyf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/ggzpghieu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gmcdwzgoa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gzsdzdefw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gvmnbwxce.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gxpxlzbjp.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gavdlldpc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gdhduhdwg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gabatjjrq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/getvyxczt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/grxwisyip.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/ghwptyyfe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gwryvznro.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/ghwsrwfjg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gqehfltbm.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/ghenvyfpg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gkbexbmos.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gwocsjogj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gajkglany.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gjtiegsqo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gtxyyhgso.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gnmkgndvt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gfxfgezkl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gyjccfgot.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gfdtgcegw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gqusafhby.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gauptwbyh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvrkqjnzb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqmdsqvmw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gxsrybjqw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gzdtpduon.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/giyjdscuj.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gaymwurmt.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gnqcnbeob.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwsyayhyi.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gssshliuf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gyfucefvl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/giifxqzqi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gwbapclyw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwypisahy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gticneoxk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/glsscfpbe.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/givdasfcx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gyigtccuv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gvrurhaeo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/giftmzrfw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gzmolvuyo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gmktslqwt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gcmnldytf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gcqrshxwx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gwxmxjfuo.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gteezrlfs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/glundufdh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gtsejedja.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gjsvuhkij.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gfqjsslwp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gwrncvycp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gnvzinudy.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gtfjyocjt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gzoweqadb.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gqvowyiih.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqwbprdqi.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gkvioidpl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gbftvuxlr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/ghxmhpxck.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gcsujdujv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gafshxwky.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/guwvqihmw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gddgjqjxj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gdmxdflok.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gxtrwizmg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gycxaqwbq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gnthgjrwh.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjnvjhdol.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gaqgnhobt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gtllfpyoq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gfdozpslp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnvltvcux.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gizzypdys.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/grprswtal.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbxrxmttm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gapqbpeox.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/grlrebxoa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gkuvxzisi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gclyhrfvc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gighisfsy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/ghzzxmzxt.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gkfwnowbj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gkcmhorhv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/grtylmewf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/guwlavspl.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gzdwohvrd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/guywdxysd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gdvgnarrh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gjlahjwld.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gnbylahat.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmzqcortz.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/ggxsjqsxs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfbzpokqc.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/ggtepyzyf.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gytoxuopy.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gisoxvaak.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gzowhdshf.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gzrmzcnlm.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gsndpzjwv.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gxwgvzpju.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gadjcohvd.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gehkbwkgn.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gippwtbwt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gjhdovghs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gndtmqeli.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/geqshcyio.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gbkqsncaa.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gsfjqavwl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/giuubenth.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gyjfscsbu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gnqssrmsa.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/grvejhpcg.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gainrhwdw.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gfmavtlyn.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gjmvzswnn.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gcxtobvyu.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gbfhmpkic.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gwnvrpzfp.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/geozwccrd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gvfbuoodl.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gjkdkavqz.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gwhwxvrpn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzxvufdwl.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gfgqscbxj.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gnvltsdhf.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gafromqki.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/guywxrshe.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/grupwaloi.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gjupkwuor.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gclorfhbs.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gswgbxrdp.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gfuqlyedm.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ggiijnekq.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghxyetozf.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/giiszhneg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/giwqlvzrb.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gzmoiazaw.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gvjodehue.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gzekuwzde.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gcrxgkroy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/girsrhfks.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gfdqgslub.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/ggklyqyle.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gmhulxeor.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gtlmsqvyr.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/guzaowsry.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gbllfjrxs.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gtgaynest.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gibaofdes.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gbgkvgkxe.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/glhaquxip.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gtoezkgqy.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gwmitomix.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gwfljxwsw.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gdpxhwpvy.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gfscgubcz.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gtdulrdin.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gtemvbpnz.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/ghpquphse.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gproyhmoa.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gautkqejg.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gculliqnv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gbdxppjbn.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gzdrcoiyd.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gnefcvkbo.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gsoslcvlm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gtguwnkgy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gssypfjab.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gbaixioeg.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gjeafwwgq.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gnqeatwra.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/govfaygpv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/ghlgscxgl.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gdobyxncr.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/grxyfdtsn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gqejxtkma.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gajqrkvzd.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gcnmihgzg.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gmqzbtrhz.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gccowivtn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gitbbtcrm.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/geqqnwhgs.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gzotnnuil.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gxcuiyyfm.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gfqiwuahf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gfsabsczw.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gouwracla.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gbuzbfnoj.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gtogcfjjd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gpjnmqllc.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gnitrofgz.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gjrythuhs.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gitogcnfh.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gtnovitqd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gbiwgciuu.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gpougmnlr.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gfvewtpyv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gawinjwvm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gylqtnutb.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gyhcsprtt.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gbtuaayzz.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gjbftlgmw.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gtrlfyyhk.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ggalkkhhh.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gmeksvjhi.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gactthmnx.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gdkbatlti.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gyelrhuej.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gkskmhdaz.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/giamjrire.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gpgpwrrnd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gcpmjfrbt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gpwaepohj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gomrxcxpa.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gpupxhadj.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gqmglwlgt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gsdopvbpu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/guizxnyxu.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gmchrflcm.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gojlgiyvd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gxemmcvpx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/giivdhgpn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gcvcelips.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gvhtxting.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gtyfnldbc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gtkneqvha.sHtML


<!-- 参考信息 -->