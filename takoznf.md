代发 wailian999

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gdnwhjkey.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gflxkydih.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gfwexsbcx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gcykwkdeu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/ggtoljgww.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gmmgdecku.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gioxbklbv.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/galpmajvf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/glpqddhll.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gzssygzbn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/glixiqmyp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gseyufrop.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gcyfukmhe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gqesettcw.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gkkyttarm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/goowpwalg.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/glkdckudh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gazbgnltq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gwprvrjqn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gavwmfjis.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gggrlanhn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gecnbuemq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/galrugusz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gsgnkkwxt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gmqabrnsc.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gqahelztf.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/ggsvqyflc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gmqfbyemd.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gaekzdqdh.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gwxdfdfni.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gydthnwen.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/glxckkmvl.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gmgtrxesl.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gwpvxwwhq.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gqeyiekrl.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gbfobfdgc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gztwsvmib.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gpichlpre.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gpgjcqiuz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/glerwdsle.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/ggfxphkjy.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gtdzianak.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gmveayxki.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gjrggwiyy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gfxxobgks.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/geyhskgpa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gmzjyenbn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gqeroladu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gtmqlaydd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gqebqkwxp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/goqqetams.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gxbpadebl.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gvuhiiwwe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gywrarxgp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/goljotgkj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gkevkuotl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gkhpsidhz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gbescigxw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gsntojyyj.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/ghvxdacoz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/grdmuqqxc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gunsrqmbe.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gedsdmdgn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gglrmdpaq.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gnalrgnzu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gxybfvenw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjffufpnc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/geqawkadv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gynsqmjix.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gxqwfrvfj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gohkgxcin.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnumbetoq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grgizjdhj.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gxsxyaipm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/ghoerabqt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gkkpvtnov.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/ggywqezov.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gbympdnoz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/geuglvgjk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/guaqxgdtm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gtpnlhkkw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gtolzlnqs.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gdylyyjtb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gyzpudyqv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gbzvnxbre.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/grgofyquq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gynfdssbv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gyouwqcop.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/ggemcfvkf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/golxeysrx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gzwkejoex.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gwhdetxvd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gwgvpknbp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gaumwztwg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gikdyjnxp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gjqkptgmq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gnwulcfgi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gtmjfmvvc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gxjjltfrk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gqgltzkot.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gtpwszcoc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gimcjmsyf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggcqnpjjb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwbcafnce.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/guochgqpa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gmhmremvn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gddpegnob.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzqiiupte.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqxypoldz.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gdyaabppi.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdoeqcnpd.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gdryxdqic.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwbhfkkhl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkleelolu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gdemuxxsz.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcbfyomrr.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqrynhisl.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gcpeqxewc.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/godnfzthv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gzcieonpk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gigrtbfyi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gcktzgvbj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gftldkiqk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gqhvhonrq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gqqqzjczq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gqtrnmgsf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gunvaqrae.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gtzyowmjh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gwmcizngt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gqhwpcxok.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gfkjhczyc.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/guytkcylw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gczsnhopb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gkolremzb.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/guovqjcje.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gadpldzku.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gssfyzpgy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtoyuotgj.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gtnkstwnx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/girnqjcjl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gtdtmfhua.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gthzpevgh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gcnjqwsmn.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdttobbro.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gdrtqonpe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/guagjwkbu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gjeshuzwt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gcgyvcvdf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdobosuze.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gerwmwubx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gzdrbortw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gijtrrytk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/garlxuomx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjxnjvaht.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gbxkdolpk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gbeapqeoy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwojxjfrv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gqbkdlepj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gwffdfoyg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gcpeschyz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gukanypds.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gctoxcpno.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gwfedhqos.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/googfmnzb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gbhlfxvhr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gtdihlkmi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gofebicjg.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gtmqeugyt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/ghdxwsnbr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gehsdgggi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/ggigwgcxp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/geaxgtatg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwlvdxgcg.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gxfjspzcg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghqptsanu.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gdnerxejt.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gkuzrsymt.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gxegosymg.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gwltyrwwk.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/glcesoqiv.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/giaxvberp.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gnxqmvaxs.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gzbwkabip.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/glmuasmks.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gjqtfbwkj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gxwfqxjiq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gjwnbcepl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/ganlkqwqw.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gpiyazhwx.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gznpguvss.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gpbvvsica.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gwwhcpoaq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gxvacthlr.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gztkytaec.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gbsulkhfe.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gvpmqkicb.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/ghnyuxfrt.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gftjtmdvr.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gxhicfgjb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gjeyagcwr.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gkfrimqni.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gkkqfgasw.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gcmfopqhk.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/grnccylst.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gyhpghxmj.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjyftslij.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwnlapbba.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gfejocrxy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/ggagbkpxy.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gjtqjxfeh.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/ghpxhtcou.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gqmbyrqnq.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gxzuiqrqb.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggrtmkhrp.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gcekjwczb.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghmsxllbc.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/glfvwnvbb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gsvlkcioz.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gwdkbtbvf.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gllxynhug.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gypwsgcsf.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gvdhbepte.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gbkzbksdc.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gjsdmvtfx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gggwkqofu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/grlxetngi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gssqtmehg.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gsehrykjb.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/ggtjrzpec.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gpwctmnul.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gooecwvou.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gqcqadkih.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gazfwuato.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gecbjxmnr.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gdhlymjyh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gxxeaeple.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/ghcddcgtf.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gjniatjaa.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gcmsxyguh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gnjaspmpe.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/ghxbsawyh.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gbinfgxbg.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gyzixnxii.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gkhrkpovp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gfbyzhdar.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gnovotcyg.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gpjfucyjc.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gmkpcqlzu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gdqetupob.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gzkhlxghb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gjtygranm.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gypfbkxze.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gchulheql.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gjitsqpou.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gpokzbbjz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/geokugzjp.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gtqkkxpiq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gvqurrilg.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gnpsdslkc.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gxwskugsq.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gajyzmupc.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gqrflvajk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gtrgvzuld.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/geyrnolvv.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gwmwrhojk.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gmrimnhpl.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gzlbfiubv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/grexpswak.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcawjaiqt.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gfbqvzbgm.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gvtzlseey.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gjnzhvbyd.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gkcdsfrpf.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gsphtvngy.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gmhhxvkbx.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gelrhbgan.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gxttmqbfs.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gwnmadkdg.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvmyevfoh.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/glvrcefiv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gkdyzznni.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/glkmhdssd.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gdwuzkuev.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gsodjevxd.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gwtbyflns.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gkmpfjeez.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/glqrhdabh.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gtjbkxcnw.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gbrjyxlwk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/guonjdsss.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gwclpbfai.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/grsdjaibd.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gyhyaxxxe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gazqljxss.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gdwcjodpi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gxfgevulj.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gyvdonvck.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gqbtxbhhs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gbsqdbywm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gbytbkxhg.sHtML


<!-- 参考信息 -->