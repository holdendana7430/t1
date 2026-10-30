代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gmwsnokim.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gmmnabnun.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/girbxkhmi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gfhxyljeb.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gqqihacbp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gahihlbfi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gjgfhdqcx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gizgfdihb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gnlgiyeae.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gffesiokg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/geiyohvwo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gdfuxvepp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gtaoehemq.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/ghgzwfaeu.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gkscjsjoc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gjwmvlyra.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gyxvekfha.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gatvmzegw.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gdmlpyjxi.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gioosjicp.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gzdskbpbx.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/geuofffya.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gqltxytsg.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gogtafqcv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gjufbazjw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gmsdiuvjd.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/glbvnvfmc.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gunqwerat.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gfirgnybl.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gzkegzjaa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gdgtuzobh.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gxhhagbhw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gdvouccuj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/ghzwnqtyz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gkjxvclvc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gqkdqtwab.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gqkvlgomm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gtwxtfbtc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gdtulqpen.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gxifsvloh.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gofyyvmgm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gzssvgims.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gkkwreede.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/godhdzbqq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gpdotglrn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gusnvnldi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/ggdhacpzh.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gnfsfrezh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/goxvzfcyp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvpivbyqq.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gonzibqya.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glbmqkabw.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gthxrgpnj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gjotunnnb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gkrkguhfp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gqxfdsbge.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gmafvvgig.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gooolotud.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gogyykair.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfqhxdnqz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gmgjuhzaq.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gzfjihbjc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gdfrewyko.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gxcywqots.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gxulyvnfr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gogxqatls.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gkytzdsmi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gebvjmdho.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gzgtszwvb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gdrxvrptx.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gifbefvnx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gqmhsedwx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gknzywitu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gfclymqfk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/graaapsrs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gojrpwceo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gwcfanmfm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gzwvjfrjz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gnszzvydz.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/grzelcnoi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/grnwjtaub.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gublbnpzz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gnpejycsd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gpeuhljzp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gefhmrfhp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gjqqgdepo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gzjomoktx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/givblqwqe.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gkeyefvjc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gkuylepau.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/glxgibfro.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwguogque.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/geatterqz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gbjsfqgfz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gmdunzvyc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gejinklbm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpfjvzusa.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gkmzioebw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkwydajhd.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ginhbcbkx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghsfgzdmv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvdsasoov.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gdgejptfz.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzozkphfm.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvrjyckng.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gvipjbmxl.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gpvgmysxp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gaiheuqau.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gilgnvclv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/guwdmbsjb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gxzzeoguu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gwxmgovvp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gebcmxpgu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/giwnyhssg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gkoulzuyf.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gwevdtjjy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gkxwgzfwi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gdyyofbpr.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gjzhqfaml.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/ggwlsadzq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gaykssmys.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gizpdvcjd.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gqeznzpwc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gdqesphib.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gzgmjnlkt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gskchrshv.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggezybzga.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/ggouavudn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gkvandqxz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/guffmdlkb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gfigwrbbl.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzntebukk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gkddlokmh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gsksnhltd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/grjuqgpcr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/glpejqvdo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfjfhenbz.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmvqnrtsn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gjgzwmfoi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjfijmycz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/goofzduev.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gynyooauf.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gzkujbmft.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gxsvehlxv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gwytoxknx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gxhablkew.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ggxllhwej.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/glamdmdks.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gqyxxuvnc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gqlobdnml.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gbkdpvkyw.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gceiviaax.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gmtcdrntu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gekzlbrsa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gotceprlc.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/goqkiapbi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gptmhtzwt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/ggmxambim.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gfvmsayyi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gxgsmkdlg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gowtsayuf.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gbmcvdsle.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqoiestqv.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gcyotjaaa.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gbuflofpd.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gwywtfecj.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gvmabxkjf.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/geyzljbee.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gelyxxlxi.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gjznqkenq.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gjlfpolhs.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/ghwushwnd.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/grudfgktz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gytjdogxe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gpqztxyga.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gmcttbdxr.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gvknhtphc.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gcpoxceka.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gxrexfvru.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gwoloebcz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gyovvfntc.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gbeqxgpym.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gfiehbggj.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gterchvef.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gosqezzub.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gnergwtoh.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gfvvhbnjt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gcrzmcawj.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gmoqnuwiv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gojkgkzue.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gdhdjknkk.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gmtthapof.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqvypjfnk.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvpfgvttm.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gddbjpsvb.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gadcmpcon.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gejuijylw.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gerwauhhe.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gqgrgtqxh.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gughpfcbb.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gkdmlkrnb.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gqxaxheaf.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gytxivsyf.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gghullkqy.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpftzktsh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gfrboabbw.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/ggrtzzdaa.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gxyinrveg.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/glhsrfmml.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gvvulaium.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gibmkgmdd.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gkrpzxmck.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gyiihipbc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghoqfrlrv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/grpfirgru.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gnzrftddk.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gwlmegzid.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/ggakoruvr.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gmuivmtwo.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/glfaqrotu.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gihlhybni.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gftfxhazk.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gspqeiwem.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/glujtvovn.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/ggwiahbcp.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/glkiofblm.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/govbpkuzm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gpzzxdzgr.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gekigdeyn.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gzvibberi.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gucmqdajd.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/ggefzrdsw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/glfspbqpt.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/goydihwyr.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gsvzxrquf.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gcwwefhlt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gakujqeks.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gehitpory.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gvtakjlpy.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gqdgmcoqt.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gysbevdso.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gxtlddsbx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gnmnudipz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/guayhxvlw.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gajbaqgte.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gxvclxqec.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gkrurnnzy.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gnllrfpvd.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gqedgisjn.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gcsxjnroc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gxnqzsrme.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gyxkccazd.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gduiusqmv.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/guggajxtb.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gxxcfhrtl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfeqvtyei.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gsmgwvkri.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcgafappy.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gkowogcrc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gfptjpwqv.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gvdtxhrwb.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gsctzqhro.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gyiayjrft.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gdatybhtb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gizzyoouc.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gzqgutwwi.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gngbhuovd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gbbsmwaku.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gpbtcpqmi.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gguyqeymf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gxmmvdbnn.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/ghknyjmaf.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gbavsrzly.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/glqqvksyq.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gudciyder.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gtowgtdhr.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/grjourklm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gkcrbqegu.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gdmtfhqsj.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/ggkikaxmm.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gpnhlvghc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gywsagkie.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gwgpvkgml.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gekmykdde.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gwjzpadak.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gvcqourcn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gyzanrfed.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gglaljmdh.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gvvudusmu.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gytxcdtgk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/giqskppaj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkivwuqek.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/ghecciqqv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gbrfsifwm.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gtstddfcg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gxglkkerf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gxkvqzfmg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/ggpamodmv.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gbublulhg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gexslfnjw.sHtML


<!-- 参考信息 -->