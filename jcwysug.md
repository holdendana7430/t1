代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gejkejsxr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gyvnafruk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gajylommt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gzcsbcifz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gyzymcact.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gcizcckze.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gtgvfakov.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gdjjaiynb.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/grhtclarl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gdcpgzczm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gptosqntl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/geeddjgsv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ghwtvsfsz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gthqsmqsr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gpkbcheos.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gmuqkgpvk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gehdthigr.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gddwqjxaq.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/geqbuafrf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gcwecucps.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/ghgkjowtd.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gyczijefz.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfiqaybxw.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/glewvsejv.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gxcsgjjbl.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gzdqydiij.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gpicdfbpo.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gxydokunw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/guvqauboc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gttlhfnlp.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gtcwlbhgg.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gannnvgcm.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/giwksfevg.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gporqojzv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gllljehas.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gflpgmdaj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/ghhztxycm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gvywqhncs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gqrdegron.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gmpnfmsia.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/grphkwniz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gncjtxtxl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gfdqzajqf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ghvdjynaq.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gjhprpnto.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gkityqhuo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gjvzvdjdc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gwzudumxa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gewuouooi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gyyymdlsd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gxmogzuxa.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gldcsfbsx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gqvemsswo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjahfdmww.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gcrfwmokz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gekvmrefz.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gtrgehanr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/giffxpsek.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gfflyhsll.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gfqadydtq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gawnlilyv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gcrdkyiqg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gjvyvkhpw.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grxmtuute.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmdwynnnu.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gyuxxpsjg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gfrvvvrak.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gobwabexs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gwrhhwmnn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gqmnpkkzs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gorzbcflx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gmktghxmk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gjnsxikfe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gpelcxluf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gxxtjilrn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gbqzfjwco.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gbfxoqmow.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gotbycnwg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gyzsoenwn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gxxtveayz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/grdxcqohj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gmlofgqfk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gtsbfhmyl.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/glvoyvhtt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpxnfbbix.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/glioxuivj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/guxvgzpne.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gnogqsgfr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gpsdwwkwp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/ghoexoare.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gpmyrqvpw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gxihupime.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gqzbxbvtx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gtlloresh.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gueivhjdt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzkrbmkpa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/geryztecr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/ghnjkoaxd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gmnzpjung.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glehwfdjf.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnoawitur.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gsedmrdsn.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gaynolgeg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvhwnduiz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfxyqykic.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggvufyrnz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gcehyiyps.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkygrxdld.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghqptresm.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gkrybhyhk.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/ggkfwbamb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gjqhzqxoc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/garseasjz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gxbwtfavz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/glpqrmyxf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/ggzvbtowx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gmimnetbg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gkejyymzs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gmncnkvpr.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gdbzynyme.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gktgdapoq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gvksnbwsb.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/grcyzjgjd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gjrgpcuvk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/geldgcksz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/guxxtrdye.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gdszyhmca.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gfbrghfkx.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gapodaemd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/grfqjdeok.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/goxevhyrp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gwsushxoa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gpsolqqsc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gxbwozajk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/ghgkuqxtj.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gouygzkkj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/ggarmcmjd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gzpazlddz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkmgbhhyg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gpezrutzf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtttqhoun.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmaspizmu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gceibnecr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gtxrenwjd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gbhtsnpvr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gktpfhenb.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gtjmstdtu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gxenxhqfc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnyxzdrme.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcplbjqqs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmugimvwq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gmawrhcay.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gdgxxykrj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gzbqzpqqk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gkqnndkku.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gltzgogjd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gwlokvigj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gqhmlsgxb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/grolfvlpf.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gzufyfohk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gdlvqnthu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gvkdquoul.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gzsujkjfu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gbukzxqce.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gszqyaycr.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/ggdcdcovp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmwndqcba.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gglxfrfpc.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/giblzwhrk.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/goojkfzmk.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/guzglckth.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gqkclovna.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gmkffvubv.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gcrhegvxx.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gsqvgacpl.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gfmsxtfls.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gkeaqjvsl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gqxbaaire.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gltpgeotc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/goijuzerq.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/garcaxgra.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gkoirprtk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gqihwvudf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gcheqxavz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gkyvcqxuz.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gwyiwjjra.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/grutqrrdi.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gpxtlkmlx.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gkcukyitu.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/ghfjjkzcv.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gbrcmkmaw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gjakzjuoz.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gznxedjhb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gxgteiqdh.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gaanbwodp.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gkfddgzpa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gknrmybid.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gwgetgedy.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ggjootlky.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gxxziokhq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gaeyzhhmi.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gujaqdort.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/getgdycwj.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/grdqgtrzg.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gtxjxgkim.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/griwsbgak.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ghrpqjord.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gygkburhg.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gdtirhkvg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gvwyqgfju.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/ggdsytups.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gvizzwpre.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gvjcboaws.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gtgwxztmm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gfxdpzkcd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gsfuecekf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gxcqrjndi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gcvblfleq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/giaurxbtw.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gbspmicua.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gcpewpruu.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gagbbedtc.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gyryktbkp.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gnrmregyq.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gqjblhehy.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gyslhnsej.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/guscoeqin.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/glicopeuc.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gdieevvvd.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gaiydrtwj.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gzuhuasge.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/ghhevryhk.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gurhfkkfc.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/ghrpamljm.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gkppmurnu.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gzyqqyuyb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gnoevbgce.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gmybovtpj.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/geqazdbyy.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gzoiuhekj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gbhdchmtl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gzclqppbw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/ghozdqggo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gethrrtoq.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gkznrlmdi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gomdmiecf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gyrtohrhm.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gzpcjkcmu.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gjsekzvws.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/grmrljaxu.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gnyvvqwav.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gsvdfgxxm.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gohqbbazf.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gtkceyava.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/ggfbqrzcw.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gkbhyckie.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gvndftuqk.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/goakttwqj.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gzsdafuui.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/glsrmgabo.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gdlwucaop.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/ggqmqybjv.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gapxczgyt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gptszazzr.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gjtzdbhgv.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gqzqzkfmi.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gbkosccre.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gmswielac.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/ghmjdybux.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ghtfqskbr.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gqistrbgr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmxofsmdb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gmqaddiwr.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/girkwndsj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gygbapzcv.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gmuvuqqcw.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gpatjbqjp.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gfztkzxdd.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmrrvxdlg.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/giiryuzpr.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gdjpojcyl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gvurzneqi.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gncjsnpai.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gedgojifl.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gojxqytoh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/grlugohxf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gqffykdas.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gbgeywfdv.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gmyietvcv.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/geapwcbae.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/glvxichhs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gvwnezrsh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gqplmjqtd.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gfvfihnec.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gnkituybg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghxmeqwdg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gdwajxjqx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gxraxokpw.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gsrbhwwib.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/ghvpvjgrk.sHtML


<!-- 参考信息 -->