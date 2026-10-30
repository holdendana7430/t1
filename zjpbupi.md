代发 wailian999

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/giwzosdca.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gbnoyioaf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gkbetaxaq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gvaqindaq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gxzgeplol.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gsjjplgta.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gokpinkus.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gtcowgwko.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/glubwwstm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gmpzdcvqf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gyjvfamlz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gjyniotod.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gcowwvpof.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gurcugkgq.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/ggvnaraud.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gdhixoddj.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/guowxoswc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/glpeiizfo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/glarlowro.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gzbftivml.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gpszjzpjy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gjkbgdbip.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gwflnnlwo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gwtsozjtk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gbngunhed.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gjywtokxy.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gypwqqsfd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gaibadccq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/ggurceyjp.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/glrtowodr.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gcqokpjdw.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/giztlxcfz.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/goeinsxam.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gckapatzz.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/ghcxcsiqy.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gjcnhaago.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gyciufxlz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/grerlufgi.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/grgdvcvqk.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/geaapbsdx.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gwpqjgyqy.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gifkkglte.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/grsspazvh.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gcuqskfgu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gldabbkvw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/ghnyhyrle.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gacxtyitc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/grtfppfcc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkpoysskm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/grdzvexpf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gzxcgrydw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gtayfwuzd.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gxzsfacss.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gbcvephnh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/girxkyldx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gyxffnwom.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gavtbugma.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gaqjkfmeq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gkassuycb.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gxghorfnb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gwicdhrvq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gslijohnj.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gtfpagyhc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnouenqme.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmffdhiye.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gfrltaotm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gyylhpttt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gpzgxukoy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gvttrmltx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gbeggyjmi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gpozwirzx.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvrudrdwu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gngisyety.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/geussqiam.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gwovlpymh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gwabajler.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtwfgumlf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gdetbenxg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gujkopbow.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gteloculo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/ghhgjqsqo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gbwdkpftd.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gmusnorrs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gnpuqwiio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gbbvomaxl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/grtfrqmly.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gjzkauqve.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gxkfobruy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gmhoyfvqn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gwalvdxum.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gazveckaq.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/geobqrxnr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gccnynaty.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gypspizwr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gkzmpltmc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gnuqamnaj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gluioehvk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gzzkwptrt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gbvanxjyd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gtapzbziw.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/ghpldvila.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/geqahfshm.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gpjshfgsk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcnudwamu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxcjpfrfu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gvmfedgpr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/goklquksp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gklilmzau.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpqgxrqra.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gksgqvbcl.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwnxvpjkc.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/giktkpxft.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdtteiaig.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grsjrlkcv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmbemfyae.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjdovnipf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggvdalrdf.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/glmukntql.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gzzuerfcp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gwyldrgim.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gbgzpvzvk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gonpekrxh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/ghvscwebb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gyctqwwfu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gwtseevsa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/ggcqchqva.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gppmsrtpx.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/grfjolbwo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gvoizbtyx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gyznuqaqd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gcizjtcbq.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/glopmaqgv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gvwekncqk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gcospktfm.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gsckawpux.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gchjkhqqc.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gilrcxdok.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcltnucol.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/guriznmlx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gebelsnjy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gosvdagnq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gmeuezbhg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gffuxmtjl.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gafyczfox.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/ghiufzsnd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/govulvqop.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggpoulezz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/goexloudc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyjjizdik.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsrbhympq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gzyifgqqy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyqbrcrhe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gkoztxhec.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gnrzvrjbw.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gphuzzefd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gqbrtiftx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gsjrsvmcu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gsjpdfeqy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvninjbin.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gvbyriagr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gzeptsukn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/grmuvkbva.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gdagzxflj.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gghfccrco.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gtgexkktj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gymquzpne.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gqhtfudwh.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gbiwtkcmv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gurzsxmga.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gqvgqxhjo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gflkxeswk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gwxzebrml.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gztgsjlxm.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gznmkwfyj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbskkbfcx.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gtyfewnqg.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gxpjhqvhb.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gtfzmoxpc.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gfbrkvnut.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/getwfxzzd.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gruefyycd.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gxdyqdigp.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gmliiarhp.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gutfpmadt.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/giwvsmdhx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gekwxedmo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcxtsdscs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtmdeatnl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gsdmouoia.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbkyzjciw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gwvnhbqtx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gnfpfttyd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gyizcwyoa.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gnisopkwe.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/glzshlrck.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/ghbzsnwxw.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gfstbvefp.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gwpagvlxu.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/ggjvsbfwm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gpbnrbdfe.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gehigzzvw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gyfgxawqf.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gbskzxgbe.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gdyhitdtf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gdaqtmigm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gqbadyumj.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gqacwahvu.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/ggmmuptoa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gjylfmeuz.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gzdoqrwxw.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gxvcbrdbw.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gkwzxhufr.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gnevkumyd.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ganwewhlm.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gjhnobsxr.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gdbtitpqc.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gvjrwfccn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/grcduxndr.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gcuhicrwz.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gkvzphnre.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gegaynhyo.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gbkmgkxec.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/ghwaorrnq.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gzxszptzm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gydovlzbx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtrowpdiu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gnkrdekuu.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gimuukweo.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/grxfexofn.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gjsprpwkf.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gugucqbjs.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gltedovwm.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/glbnmcqiq.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gdnnczsrr.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/glzifshoi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/glwdrveuy.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gqsyaubch.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gsnythrpq.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gfjrdelrc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/glfispcuw.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gcbvsoyet.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gfrvbwyhc.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gvpimliux.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gmspchwjs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gfxpllrps.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gbtdlytay.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gxydpqisf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gpalwawut.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gmyhvzosh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gmvtwmuot.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gyqdfwpsu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gyiamqecu.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gcegxogfk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gqetpdavc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gcupjwwzc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/ggbmuqemt.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/glkwhmokq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gbnvkmdfe.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gqzsweskv.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gftdouavf.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gcipepvyi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gnhfnoahz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gdyczghhe.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/ggsybikuf.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gevwuihng.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gzhweantt.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gcjnrlslr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/geeztrpea.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/grvxemqxh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/grphthghd.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gebdmntoe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/grcojndmr.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/ghoemsgcu.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gewypvptc.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gzouhjcjm.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gcajliyfz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gynrfuhgc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaysfubfb.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gqskwxcom.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gogmdkzyi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/grdvftrrl.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/ghgxphmet.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gpzbwddnt.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gfalfuwze.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/geqfcdnty.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gbysjghix.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gscmtjqed.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gaaxkacun.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/guglknpwk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gllslwbjq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzobxsxi.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gdghfmmll.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/ggktjoblq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/ggryziyvq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/ggyrbyzkx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gsywusnhn.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gbnkenagz.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gwziuzzel.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/ghkcbcjup.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gvwabfykj.sHtML


<!-- 参考信息 -->