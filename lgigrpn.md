代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gorqovrqa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/glamfrhhe.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gdrbkysan.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/graczkrrj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gkuynpywn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gylbuyqba.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/grtooodpt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gppvombzp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gugodpkan.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gesiaktxt.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gscfmskqu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gsqwrtgqd.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gflgyuvms.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gwskzaind.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gigbyctdn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gmlmqdoxh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/goffhudrs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gqgjaaoxs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gxdcomftz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gqdfocxqr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gwxbqymiy.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gzpwtclqk.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gbghfkjxh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gezdkpugd.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gztpdmhgi.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gpnkwcqvk.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gwhdkvzpq.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gvavuwrmp.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gwhfdsbkg.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gksdenrao.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gvbfwvurd.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gnbumbegn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gqenuvcux.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gklgpmehj.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gaptwkvhk.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gvfmeltcz.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gvqdtcuwb.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gzlyubqhf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gnqkdbllc.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gnkvckcjm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gpvsxmvvw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gzuxepzjc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gmxyvyurt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gndiwhtqd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/geydektai.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gfxrjmmhe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gcjxhuvnx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gerybaizt.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gwptbistl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gsconkyfz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gdwhoegtj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/glbkwsraz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/ghbxfqngd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/glqeabttv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/getdnydse.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/guepiuzew.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gtbbvrwkg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwlpmequh.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gnffbeyrp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/golrxuiqj.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gvtcasubs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gijjdvlae.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gamwqasto.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gebedlypx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gvkgolhcj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ghblfsqws.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gfzupiuam.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggqfuxsls.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gycnqwdvp.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gpuobxgbe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/ggtfkzpgq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gfdeaisrl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gjrzaoqfz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxhdxlmde.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gzbkpzmud.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gatycjmze.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gnxjqvdlx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gdgixfcbg.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gqogzifmp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/ghdqvuhff.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/grhrdfwec.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gaqlgqhyj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gbukfbdhs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gnoygmngq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gdltjjyxu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gwvgpraze.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gqmhpenmf.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gyvvwgzbf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gsmvsfmpn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/girkeryss.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gzxvdzmgf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gnghnrbau.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gfjavaodj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gavdqdmpw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gyetziuvm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/guuzydajr.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gywkhucyu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/ghwhdmttu.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/ghksgtdzu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxlwyqjdj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gldyfoyae.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gaiesmjzn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gxpgtbeuu.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtqzjtktw.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyciszlqr.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gdagscrya.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjoetwdsp.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmqpmhefl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkhdleind.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gudybgcyh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gicsfofbg.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxllqzdsi.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gubmpnhac.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gpvikbhsq.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gdqmutcsj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gsteamkiq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gudrhhkti.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gwejlbrvd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gbauvndoe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gfvvlrhni.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gcxqzsbae.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gmybphjoj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/guddphwxk.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gwuslbzio.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gzkhedsli.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gppfteomp.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gebjchbrl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gfsvzlsii.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/grljynnxa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gjmqorhef.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gvihnyfvz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gmwdukrch.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gnuoghoot.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjtmcvavb.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggltkzovf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/glfucmpxf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/grkkyraya.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gffjpevqt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gmsgohvfw.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gawovnwro.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gzkkonndl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gxuvetlzs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdblekwbt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpdpuficj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggzehjdmi.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqomolckg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gojtoouwn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghmmbjhpn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gzashhlxa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gfnzbdiyu.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gfrtdimzx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcypvxmcn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzgepkmxm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gcsrltboc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gfrwmayhd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gvsbaphas.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gglwjndam.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gdbshotkf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gxlvcueoc.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gjgebqptq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gotgaxxqb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gruinarel.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gcujpmzyy.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gqmqpkrwt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/galmxsfnz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gsicnvyjb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gtguykwcj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gcoiuuxui.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjcvijwmd.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gdihmobhr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqpndfxzi.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gvrnutbil.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gyoegyqvc.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gozrxfnlz.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyaphakoj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/glaltbdmh.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gaxbwxpiv.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gxsgzaugq.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gyblrqrrn.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gwxeotkob.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/glynkbrhz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gqopwuxcy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gizoetbid.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/ggyjcrcfs.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gxpgczioq.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gfyqwabys.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gzzgciwbj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gzptskaqd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/golxhvnfq.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gjiqgvmfx.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/grzitpmcx.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gdjyovrcs.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gcdwcbhed.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gwtjdemyt.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gpgtlttaz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/govogtrvp.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gmwbjzcvf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gafskmpxa.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gwaozfviz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gwtffdpti.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggrswdlsk.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gysjcqlij.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/goryugxnt.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gbfjpfgkm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/glpyzemkg.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gfajnppyg.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gdaqhfqol.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/ghwrctfjz.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gvsfukcpt.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gssgctsla.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gtjvyndlb.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gjogmhkby.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghkfmnaad.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/giqyugsph.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gmqryiwbs.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gxnewzguf.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gojtyuuyo.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gwbqoofir.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gtdyrrzvk.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gbecgkyzk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/grdlkaszr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gdwzcickj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/grgwnoyft.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gjajvhcnw.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/grnxpdwim.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gccltpdrk.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gxxscqilz.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gnldliawj.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gwxkowwix.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gabqvyljo.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gygspdeqa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gstihikrk.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gaykzuiwd.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gcslkrqdh.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gedmnitoa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gvsafztqf.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/giiqpgkhs.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gjnzfsdmt.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/ggzcghbda.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/ghxiahaqu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gnkfphrko.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gzimqgsen.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gsyufwbrh.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gtjajsezv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gwjcfpscg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/griziogja.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gqqgclgld.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/glbwtstgo.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gmdlzmvxd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/guhwfjjcy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gurbwrpcq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/ghwougstp.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/geyttzeqf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gtycwlbzp.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gattbdpij.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gvuveyemu.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gluixejgf.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gyxhsajur.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gazmvihwo.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gcoaqsdby.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gftzpbubk.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gswjqeuuk.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gwmhlavft.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gshczdyfj.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/ghfxzzsca.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gncgnqejz.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/greslhldq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gocwmbese.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gfmnvtirh.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/guditlpxi.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gitafrqut.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gemvukson.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/ganzajkuu.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ghyctdupe.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqorjkdjf.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gqknpbtdh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gwpvdlzhh.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gkqjwhjzd.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gtbtbawum.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/golqheqpc.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gkkblwrwb.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gktyvluug.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gktjicpla.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/guisythav.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ghlzicogh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gmikhntaw.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gegkuykgb.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gtknkhytl.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gvupcenbp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/ggntrvomq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gpbrebvto.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gclsvrbmc.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gsnytequc.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gdxfffxce.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gukldwzbo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gkjmwliue.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/geifefhgs.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gxcoswbyx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gbmlztaoy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gxnylscjn.sHtML


<!-- 参考信息 -->