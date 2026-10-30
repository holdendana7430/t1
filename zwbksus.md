代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxobgowm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukxpadrl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahvfkqwi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjtbcahxu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glxnizziz.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuoinomp.sHtML

Py:   s.splitlines()
来源：http://baike.fanxiaobao.xyz/Article/details/ghxicnzgw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbopedcpo.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/gcvwrlpjq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxnzrkwr.sHtML

Java: s.lines().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gnotrywjh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoroumbu.sHtML

Ruby: s.lines
来源：http://www.share.fanxiaobao.xyz/Article/details/gaferthnt.sHtML

C#:   s.Split('\n')
来源：http://3g.fanxiaobao.xyz/Article/details/glmmwagfi.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fanxiaobao.xyz/Article/details/givbrthcm.sHtML

Py:   if not s:
来源：http://m.share.fanxiaobao.xyz/Article/details/goodvcgdd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fanxiaobao.xyz/Article/details/gglwqebzw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gpndbianl.sHtML

TS:   if (s === "") {}
来源：http://wap.fanxiaobao.xyz/Article/details/gqzvpjtsk.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fanxiaobao.xyz/Article/details/grkzuyxqy.sHtML

Go:   if s == "" {}
来源：http://3g.fanxiaobao.xyz/Article/details/grdrwujps.sHtML

Ruby: if s.empty?
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqxoxtjh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gljqavcpr.sHtML

[E21] 超长截断加省略号
来源：http://baike.fanxiaobao.xyz/Article/details/givxaqcnb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fanxiaobao.xyz/Article/details/gbrycmjhg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpifpenw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gepczpvca.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwccvgcvw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/glholyplr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdmawygd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxyipocq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbsnbdmi.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fanxiaobao.xyz/Article/details/gllzncqct.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gurmulzgb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyykahhe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gpiffbhov.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjaoacrc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/gebenotej.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqziaxakh.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjhzvycb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmuqwuey.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkonuiig.sHtML

F. 文件与目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpkdrmln.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbxxswgze.sHtML

[F01] 读取整个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkxsjulz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmwdtqks.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gcaetumig.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghnvyeoxv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gtmytyqca.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gghnpkkue.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbfecsbc.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gzhybgoyu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gspuftgzp.sHtML

[F02] 逐行读取文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqwiiivpu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fanxiaobao.xyz/Article/details/ggstrmpkq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyovndlgr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/guzawliqt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gamtnhhrd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/glstnghnr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fanxiaobao.xyz/Article/details/gkarcowhk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjymrvgbt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fanxiaobao.xyz/Article/details/gnytpqlwd.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fanxiaobao.xyz/Article/details/gvcoytkis.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsnfdfcg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gqtsrorbc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gsvcohgtb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gznvtnrty.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmjngwce.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgudijvr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/grjnbehyr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gxzhfzvlt.sHtML

[F04] 追加写入文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjxnjqzi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/grszniydw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fanxiaobao.xyz/Article/details/gphijxamd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpivhprav.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/guwlbdcnx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fanxiaobao.xyz/Article/details/gsazfcken.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gullhywtg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuzctrqd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuvsuvgs.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkkmskfb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fanxiaobao.xyz/Article/details/gecuklckp.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gcmzmmjub.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/goqvnruub.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgkqrmkh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gqwtgcavb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fanxiaobao.xyz/Article/details/gymiktwcl.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gilhujiie.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqqkthhk.sHtML

[F06] 删除文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxmgcqoo.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gpegwoifj.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gsghpudub.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzkfgnnx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoxzdsos.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gfjguxzyp.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyghajsg.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gaozcavkx.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxpveqfj.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjcolglj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/gokheiwji.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gxuvdacbw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gmrwlsmae.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpdfgqxu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glskytfhb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjlzmcwb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjjftukb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fanxiaobao.xyz/Article/details/gaokjxwdk.sHtML

[F08] 遍历目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecjocuuf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjvmesaz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyjlawms.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gyzionhgm.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/grgnjeoei.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulclmomy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrtwtzud.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvneweqoe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcnabrne.sHtML

[F09] 获取文件大小
来源：http://m.share.fanxiaobao.xyz/Article/details/giwmcipve.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlxtsett.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhphuhdz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fanxiaobao.xyz/Article/details/gajkekcif.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggytkfrif.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkhvjlot.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fanxiaobao.xyz/Article/details/guwvppavm.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/grjkauhwr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guarcicve.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhgpgyms.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gftcgbmpg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbedgodxu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gortxsffc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeiwrayl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokqcdsyk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqovjvxfh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/guolkvlds.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdtdqmcd.sHtML

[F11] 复制与移动文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggldxjauc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gavkgpsmc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gpoqagesc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gpybnmjwf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/giopjqwog.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyapwyrek.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fanxiaobao.xyz/Article/details/gcaudkxni.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gfhbmrhpu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fanxiaobao.xyz/Article/details/gukqnvvpb.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/grgsbarod.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fanxiaobao.xyz/Article/details/gsqnqsslw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fanxiaobao.xyz/Article/details/gnakjwtcs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fanxiaobao.xyz/Article/details/gfclrjavi.sHtML

TS:   // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gcmibxzet.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fanxiaobao.xyz/Article/details/gfdwmxsau.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gdeimmdmd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fanxiaobao.xyz/Article/details/gihnueisl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnatpqaq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgiweabl.sHtML

G. 面向对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueuhyizq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghaiwxgzd.sHtML

[G01] 定义类
来源：http://3g.fanxiaobao.xyz/Article/details/gtkovyytf.sHtML

Py:   class User: pass
来源：http://baike.fanxiaobao.xyz/Article/details/gelgglhim.sHtML

PHP:  class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gntniwath.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghjavcctd.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzxyhtob.sHtML

Java: class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqatmaeda.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzdkkevl.sHtML

Ruby: class User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gyishnaoe.sHtML

C#:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjeuxwrvr.sHtML

[G02] 构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/glgrfhdwq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxtkgdnq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklwpadci.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxctnqpak.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gepfjixid.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidlgjsna.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fanxiaobao.xyz/Article/details/gfzddyoam.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gpupynaom.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnoguekf.sHtML

[G03] 实例属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrugtqzr.sHtML

Py:   self.name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gnyemlqwu.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/grfthuyzr.sHtML

JS:   this.name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/grgiuytkq.sHtML

TS:   name: string = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtmzmwot.sHtML

Java: private String name;
来源：http://blog.fanxiaobao.xyz/Article/details/gfostdqje.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gadcpveto.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmxpvbsd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gswpkvcpg.sHtML

[G04] 定义方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcgtvnkb.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjwzjeqj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvffvqqm.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghankdrpr.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gntlgbkfo.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjxrjjbr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gksuhcwhl.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqadvfxiz.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gztqhekrd.sHtML

[G05] 继承
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtaonpsb.sHtML

Py:   class Admin(User): pass
来源：http://wap.fanxiaobao.xyz/Article/details/glqktczvs.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guebodwyu.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gectxilgs.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gachkechy.sHtML

Java: class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gcjpcezis.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgraxiln.sHtML

Ruby: class Admin < User; end
来源：http://blog.fanxiaobao.xyz/Article/details/gkkdgqhcu.sHtML

C#:   class Admin : User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtvvynqeh.sHtML

[G06] 重写方法
来源：http://wap.fanxiaobao.xyz/Article/details/gpcnhgvik.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxcazywm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkvdvacnw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrrjutqi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnjwpzcg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfrfstnh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmujnzhl.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fanxiaobao.xyz/Article/details/grzrmkvuf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfainkie.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/guadaqxpp.sHtML

Py:   super().greet()
来源：http://blog.fanxiaobao.xyz/Article/details/gexyfqnzr.sHtML

PHP:  parent::greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gudcukbbw.sHtML

JS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbfsnuis.sHtML

TS:   super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gluhdwreg.sHtML

Java: super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaavqpvgi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fanxiaobao.xyz/Article/details/gcqsisbrp.sHtML

Ruby: super
来源：http://www.blog.fanxiaobao.xyz/Article/details/gveacbvus.sHtML

C#:   base.Greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gopauuffd.sHtML

[G08] 静态方法与属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhdfqmvt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fanxiaobao.xyz/Article/details/gzpjhwcjo.sHtML

PHP:  public static function f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gsoeliler.sHtML

JS:   static f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsthxars.sHtML

TS:   static f(): void {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvcmugbup.sHtML

Java: static void f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/geyostlpq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoktpamc.sHtML

Ruby: def self.f; end
来源：http://blog.fanxiaobao.xyz/Article/details/ghdjowgsa.sHtML

C#:   public static void F() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gbozpoyli.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fanxiaobao.xyz/Article/details/glcqnevzz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fanxiaobao.xyz/Article/details/gpigkxjma.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gprlbfbuz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fanxiaobao.xyz/Article/details/gwfwobsvp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhicunrq.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsawclha.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/govolatwd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehgbxkbs.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpwtbocg.sHtML

[G10] 访问控制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbarxfegg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwhpxdyk.sHtML

PHP:  public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gzrwbmihn.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvlnxthx.sHtML

TS:   public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzklszmi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptdguiwi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fanxiaobao.xyz/Article/details/gflwuwpym.sHtML

Ruby: public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnxyqjwx.sHtML

C#:   public / protected / private / internal
来源：http://3g.fanxiaobao.xyz/Article/details/gjvnchqly.sHtML

[G11] getter / setter
来源：http://www.share.fanxiaobao.xyz/Article/details/glcboemau.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbkjwghi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbotxalb.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgeokuzj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gohhbqmxk.sHtML

Java: public String getName() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwokzffic.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkxllebg.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgwiwyrf.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxpjjdkqu.sHtML

[G12] 对象转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoijargp.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/gsqynfcze.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgtgqsba.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjitubcje.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqjvahpg.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjeelqxt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gtliemxkj.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtjibvkm.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fanxiaobao.xyz/Article/details/grljmmpfz.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/grszllhbu.sHtML

Py:   isinstance(u, User)
来源：http://baike.fanxiaobao.xyz/Article/details/gfedncdyr.sHtML

PHP:  $u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gqkgdnjgw.sHtML

JS:   u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoczuxea.sHtML

TS:   u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gygffphym.sHtML

Java: u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gzeapztji.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fanxiaobao.xyz/Article/details/givudedia.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fanxiaobao.xyz/Article/details/gsnkjeqlh.sHtML

C#:   u is User
来源：http://mobile.fanxiaobao.xyz/Article/details/glvlrmjbg.sHtML

[G14] 数据类 / record
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfyrnnkz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdpmtdir.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fanxiaobao.xyz/Article/details/gnppwiywp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwrguvpj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fanxiaobao.xyz/Article/details/gspgklkpy.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtiztsnvx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqhehkno.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlsewffp.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fanxiaobao.xyz/Article/details/grhadbxqx.sHtML

[G15] 枚举
来源：http://baike.fanxiaobao.xyz/Article/details/glsiubkts.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fanxiaobao.xyz/Article/details/gmuhcgugl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlafuqlx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fanxiaobao.xyz/Article/details/gabnrfdwc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/grfdccycl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxitomhae.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fanxiaobao.xyz/Article/details/glyetwcay.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhmnfipv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrqamgld.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fanxiaobao.xyz/Article/details/gjvrwegos.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fanxiaobao.xyz/Article/details/gayjiqrkl.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqxufkgx.sHtML

JS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gjjlbqnxc.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjqigpvk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcjxrbww.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjottczb.sHtML

Ruby: obj.instance_variables
来源：http://baike.fanxiaobao.xyz/Article/details/gzbobsrna.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/grulreiwu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ganhlnqee.sHtML


<!-- 参考信息 -->