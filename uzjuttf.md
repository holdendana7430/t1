代发 wailian999

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gsvavvbjb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gvsdnywxw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gkxvnuuol.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/guhokbvzb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/grvqhlfyb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gebohkvqv.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gfythwlvs.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/galscuaeg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gudxhwgou.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gykgnnvtg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gslmpglrz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/geujygzye.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gpnptojfv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gusykrifo.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gixizjgfu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gtbxaxfoz.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gpkiclwam.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gkvcmcyag.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/goqxpfsay.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/glqytzhhq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/giasfqdiy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gsphbuocm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gioxrrvdq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gmrrbuoia.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/ghgxwkpkf.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gmtbofvjt.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gyxoyqvse.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gmdhstzte.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/ggzwtylql.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gsflqvzzo.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gsexfggov.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/giyjscbhz.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gvjtsqsde.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gusdarxey.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gcmrkltou.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gonklbrhp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gtplqhvfj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/givzwfkzh.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gbuzpqmrz.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gedqiohvb.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gibcstkbf.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/giiablmvs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gmeokezdy.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gtwauanlr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gobgkeury.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/goqqwdbmx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gtbqhowis.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gcoreonig.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gszvqxetg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gqzbilnie.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ggirdjgox.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/ghtwewjao.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gfieseymx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gcbcowqxe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/geukntcca.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gorzrryoj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gyiotxjfs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gljxifzqd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gpweprqze.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gqpkrcvyo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gkqrvkisk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdvkrnbvz.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gwktvsqep.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/govfbfauw.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/guxkpegtj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gxlgnqscx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjytbtaee.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gyxdrcoen.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gyhupdlbm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gdgtpoovh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gqwgctnoa.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghgiwhktw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gapxhsacd.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gvxnkfjwv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/glcfdajcj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gkemerick.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gawydxzve.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gxxvvhscw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gtmuxnyhe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gbqfzyyed.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gdggehotw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gexyiwspu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gwpasjoac.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gwhydevmt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gceakwqoc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gjmyoeoao.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gniqqtnrp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gywkxykke.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gjsspepvs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/ghheipqtl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/guxmjrxpt.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gnklgnwto.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gzlskayvt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gbrzqxhjl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/guafxmhza.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gyhtwfvug.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gilonswxs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/glkxyhqcm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gdyrrfbgx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gpawbieeg.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gjmwrjdzw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gjotogphk.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbaanwnhn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/grchqgwit.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbywccjqn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gikgjcgrf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gezotmakz.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/goyjxvkhh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmkbkfxhl.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gordfmxhx.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfceggdng.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbrglruhb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkbbzlaif.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/geoeextmh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gclvhnguu.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/ghtycpqhu.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gozcxzpob.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/grmrxcboa.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gnulkzole.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/ggcmfbqph.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gcezalyhl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gqjctmumt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gfmbkvwbb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gsngzqaak.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/glahdyetz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gotmtmsex.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gnihhmeoh.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gkpdopwiz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/glifcqcrl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gxzaemdxn.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gdsuqwrgl.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/guiflcpxu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gzcmbkhfq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gbyfjntgq.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gypshluxc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gpmbemymp.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gppebwafe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glxotzppz.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghzcbojtp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/glskvhrns.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/ggfpqmcoy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gbsncpfly.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gdywzdjty.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkdijmsbd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gvtnsmjxm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gzjumstmb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmuyhhenb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gcgkqciyp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gsbuxohhu.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gifcmcvfp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/giogzorgs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/geilknptf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gqzwrjiwm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvvbvvpko.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gpfvsmeas.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gcqyrrhtp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gchhodnyy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/guwtnrgzs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gdubwtqml.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gxwxjybcf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/ghjoikscp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/ggfwvtvzu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/goikosjdc.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gisoqezew.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/goatsttcz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gaueiqnhe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gbstiumjc.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/grewoysiq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/ghdzeewzc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gcruckxnx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/ghgbbilfr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/geqzrnkyv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghbxjtjlr.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/ghinbfkih.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnjwcovmt.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/givvlmwru.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gkqjkonlc.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gxnpgqjkb.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gcheugada.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gqzlrdepu.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gjaixxrnj.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gumavctlp.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gmerdcbjm.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gzrtxfreu.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gthtxblok.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gescctjle.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gslluvoxf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gzjtugqoq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gdqtimmkd.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gsxqhmtps.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gwfdzoeof.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/grbutloew.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gmsygyecn.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gessioohs.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gokqhdiia.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gxthbrdun.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gywjvkfht.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gqwutxqpq.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gwrhjqzwq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/guargtjad.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gtnmiudlo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gxatbdkji.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gomkvaajq.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/geumbmpxu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gtizhwdzv.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gahxditxi.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gufmtlkpv.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gnqfwqcdo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gszwvlkzl.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gobakybqe.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/grkxjmusi.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gtrzuiodn.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/glvyxsqcz.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gzgekyhvq.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gapmhejeu.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gwvcaakzj.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/grdrqqjmb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gvfifmxlz.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gkuwhypho.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gedbzgjzx.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/guxcqthqu.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gfpkzweja.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gewsrceft.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gufwithbp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gpnzewipl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqinustlg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gbmumyequ.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gtnvqjsdm.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gdlsmxiog.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gqrpghumr.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/ggobpxhjb.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/ghhjiabvm.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gjfvsuqae.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/garnbuqmp.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/glmniyqjd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gbsobyecj.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gwkrygsoe.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/giexfxvwf.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gscseietu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gnmevektj.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gghsjaopi.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gqvcxcvqq.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gqjwlecan.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gmuvdqass.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gbdlqmqlk.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gibtzeqlh.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gpfqtlvvv.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/grypcozgq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gfcsrdczc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gujpvyguo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gnuctiszd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gtddvlsfh.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gxzzyccoq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwrtewgi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gnbfibnhr.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gsbjbsvxu.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gqklgdhot.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gimdmmjmq.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gnofvpaoj.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gxqlylfgb.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gbeygmbde.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gidmuxtiw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gtrmhaamq.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gppmdxtmx.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gulpqhjgz.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gcefjdwki.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gggfadggo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gxwcimqho.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gqyahptjo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gqedvrbzh.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gzycctkkl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gjpwibjvd.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/ganscajli.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gvwviadxz.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gmcdyfcyu.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gnxzafnfu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gkgpohdsr.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gimpnjukh.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gsptslyjn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpujjerrz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gtddmysfy.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gzlpkugje.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gfuxhdxss.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gndfibxcn.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gelcsuelw.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gykdtleim.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gohhmseka.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/ggdajqkhr.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gvfklupvj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/goulhlkij.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gshiwpscp.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gnrmdasui.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gqbmqynqg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gegszwtsw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/glkxknnea.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/giccozhmk.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/grpomxnqx.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gnstijtas.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gylfppmyx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gpuylfqhv.sHtML


<!-- 参考信息 -->