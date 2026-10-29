代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gjrmcomol.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gymqxzkjv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gchitdkpk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/grquzymmz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gmrqnvmpw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gxvwjmbqg.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gaxtwygqz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gsckekdrf.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gdplpftqz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gsjwolyxg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gcddotzcz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gtshlbnjd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gjsvpxmci.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/glflldcvp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gdcafttvf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gnpodzfkf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gbbqeefsb.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gaaajpddc.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/ghqetnwgw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gsttjciya.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gbuclcgsf.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gcmkuarci.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gjtfhyamh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/glafqjzjs.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gqybcxnwd.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gcgrmurws.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gcnnjtmox.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gfoexijku.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gnhtgoshx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gmicplkyb.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gmlvjcxvk.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gsvycoine.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/grwlstuju.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gcsjizuau.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gilyvnanh.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gjbsrbxpj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/ggmhxugec.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gbyrbktzi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gxjgxkjji.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gvuwagjrl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gwzevzgkg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gctrdhmzy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gwjmemrhf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gogjlwoaf.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gbunzffhy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gcemohqfc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/glmgfpzjf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gzpsbqjlj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/ghbmodxgc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gxmewjtjo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gwzyeezhu.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gwxlsfqyy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/guyrjjmwx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxhjfwifg.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gfwsjwfhz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giqtxktzf.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gjjdahgsk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/glugajlsr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gnivgckmo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gkjzikefd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gahfrophm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gmpypuepw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gynfjgdqs.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvapoccqp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjkkmoxdd.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gdxcfbbkn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/ghjvlxioq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gzcvzsjuu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gdbehcdyb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gxlptnwds.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gmhmaufzw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gxlyzjdzg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gvmnplivv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gpyamghlb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gufdudxin.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gowjtuxlv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gtoflvsmm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gvfpspjar.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gxpqmnwia.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gszbcqshu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gbcmrspxy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gvqrdnrzx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/glithngkz.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gzefmvmvi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gefysehgk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gnyzxggrh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/ggzbmtcvp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gtfvsqltr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gokvjuufj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gfeqeakek.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/glskdofjq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gvpqnjhqg.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gmdsifcmx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gzsjdexlk.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwewdkhha.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyannbgpv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gigdzkvbt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gjenwvafd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gefyjepcg.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvmcuatdc.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcjrxpavl.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gitdzwhzy.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjmmczsud.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gowlycttg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbulmxtdx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdgtptnoo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gichjyzyy.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gddlohwqp.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzvgsysbi.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxysegfon.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gvhxhdtne.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gkxxeunft.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gqpujqcwo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/guhzdixma.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/geriyfyru.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gagfjtuke.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gzlihlnnd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gjppkfemt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gpakljyat.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/ggnimysvp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/geqfzmsar.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gtywuggpa.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gdbffbohw.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gqhxihcdq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gkuzyodwr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gtrnwxtif.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gcoiinelq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gvwzjltux.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gifrgwmll.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbpmexpxo.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/grsjndthp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gerwcnuup.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/grhhljsyd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gbltbktfd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gfbamwpqy.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxrruzccu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gjkykvsrr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gascpinia.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmcbwyqes.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gonvbpiqq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmsvezdzt.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxiieeckq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gfqqbgyvh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsmmbtndv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gngpipbza.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/giopsjldo.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gjnkmrufb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnwxvkehi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gwblfipfo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ghltqeybu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/grgwilvbl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/ggrwsomvw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gcyriihwr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gvmshtxsd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gddopvook.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gfupquntc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gedbmorfj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gtluirhns.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gglxlajui.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gniwlqhay.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gcmgmuaug.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gwmdpwroj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gzpbgtmnp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gjkmzaykg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmwwypyaq.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gbazdmwlz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvbehubtw.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gdqqrmtwr.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gwopwnclb.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gwzpertrh.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gujslaynj.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gilmtvsle.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gncxumkbc.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/glurkkrkm.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/grwiwkqdz.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gekcsoptz.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/ghinwtbby.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/glsnvgrrm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gdmgoqrsv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggjtkvnxw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gznpaehrc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gqhjhufmz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gejpgmukb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/grzlvnndi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gbqxybuzm.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gpzinosjg.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gfnvxatfe.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gsxavntwo.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/glvylphdq.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gjtxljqvo.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gpqitells.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gdrvcekwr.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gjgzuowov.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gkrnhfner.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gqcjmoqst.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gmksfndpf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gjykwlzjd.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gpvttwmjz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gibwnzvcl.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/giswggvoh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gtzmbvgiw.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gobhbcuhi.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/grtbwrqcy.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gfgcqqxbs.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/ggjcttxlp.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gpsdqpclb.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gaxmbrpbo.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsqqughle.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gjgmduuaq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/glvdbiwct.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gqlisxtgm.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gtnwtmqsn.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gmfzwvodt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gkjcbiawl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkbfkdkjg.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gihwfphee.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/ggrgrtsoc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gikudymko.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gtluswahi.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gcvmedmvu.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gzkqicqav.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gnpjhkrmi.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gphczjjdi.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gvjmfmyck.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/ghyugwbye.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gryiktcbd.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/glybakvoh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gjgofdxur.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gtwgwkgyj.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gbaalnkce.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/grfhrpnqf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gdgurikjc.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/giogwbffr.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gpnlnjssf.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gypglhqnh.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gaojnucan.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gpaxxgkbl.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gnoxhpojw.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gjjqugdqj.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/giwmwecxf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gsepghhxs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gmkmrrbyo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gowdahkzp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gfnqepshj.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzkfgytpl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gaaompbgd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxtlhxhrh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gjsweseah.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/grehwddri.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gddzmzerk.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gzezvrwdv.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gmurxrejx.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gdzbbmqen.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gohjmjcob.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gllwwjkyr.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gwjmfzfcp.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gwyckukwt.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gkxrgemcr.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gzfmmrkyz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gsbggjptu.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gkcthcrtv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwrdchbzc.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gqntjudgm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gjkehuxay.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gjjnxxtaw.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gjcjzefwq.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gmeyniiiz.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gkojialsw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gzlhusirn.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyfmxqcbu.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/goiacwpnb.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gehaggqbz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/garlavhua.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gzmzegrqo.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gmpywyrxv.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gvuzqlbmx.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gefnpylbv.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/golsleaht.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gthpeixra.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gsssotxej.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/ghnabnzcr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gujkxidcq.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gwqhlnioa.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gjemspjlv.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gvciqovwg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gzbxiglzj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gjfvoctdn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gnmuzunwk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gkwxjczvh.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gchivtbwi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/glhftbrjp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gnxeuzltg.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gjglmhtec.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gqcnttssh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gqxexzsje.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gvdldingp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gazurzqnx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gtdsusien.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gaafuxcsu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gfucmtdeg.sHtML


<!-- 参考信息 -->