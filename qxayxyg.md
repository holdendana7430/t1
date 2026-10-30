代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaszhkcmb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/grkozadxa.sHtML

[E16] 数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gpxkauryq.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfezkmkjm.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguuiayal.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fanxiaobao.xyz/Article/details/genlduluw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopaowknt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/giyjqkoov.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxfflmyk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gdpfyqdpq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbyrrnnn.sHtML

[E17] 首字母大写
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkvqwxxb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtqkoemr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoktnghu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gllueimuf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcedfdlcq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fanxiaobao.xyz/Article/details/grlbzxwsh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gpmdhgidb.sHtML

Ruby: s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/gfjjmffma.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fanxiaobao.xyz/Article/details/ggodirltl.sHtML

[E18] 模板占位符替换
来源：http://blog.fanxiaobao.xyz/Article/details/gvqgnmdyb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fanxiaobao.xyz/Article/details/gehpesqjr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fanxiaobao.xyz/Article/details/godtlscns.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/ghztgbxkx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gqftragfm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/glqhezbjb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/ghmxxobqx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkavmokq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbhvmkyt.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gbhtizpdp.sHtML

Py:   s.splitlines()
来源：http://mobile.fanxiaobao.xyz/Article/details/gavngcnjy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gdlxpckni.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxclwwxoo.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gorwezcqa.sHtML

Java: s.lines().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbizwtup.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/guadnmlie.sHtML

Ruby: s.lines
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbadwlrw.sHtML

C#:   s.Split('\n')
来源：http://blog.fanxiaobao.xyz/Article/details/gvyksulqx.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fanxiaobao.xyz/Article/details/gwyrjpbvl.sHtML

Py:   if not s:
来源：http://read.share.fanxiaobao.xyz/Article/details/gadcjinsy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fanxiaobao.xyz/Article/details/gftmepzrs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpskjokhp.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqtehjjh.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxqdunorf.sHtML

Go:   if s == "" {}
来源：http://3g.fanxiaobao.xyz/Article/details/gptkketkm.sHtML

Ruby: if s.empty?
来源：http://read.share.fanxiaobao.xyz/Article/details/gdejjnfpc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjycdgcue.sHtML

[E21] 超长截断加省略号
来源：http://baike.fanxiaobao.xyz/Article/details/gptugtzip.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fanxiaobao.xyz/Article/details/guujbcijw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gbqxriglf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvvjxysg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstojktlz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/genfsgnel.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fanxiaobao.xyz/Article/details/gannuizbk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gggxddarb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvdzqnzw.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fanxiaobao.xyz/Article/details/gtmxrfckt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpnsvgkz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gdcoiiuqc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjioyllcj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gruakcpns.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/goocadojk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfmnuovb.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gbvpdnoem.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhowqdwa.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjbiugosu.sHtML

F. 文件与目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwfivpwv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ggewduxbl.sHtML

[F01] 读取整个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwzyoeonn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fanxiaobao.xyz/Article/details/gfydmdnnw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gsrtvknkg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurmisefy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvfkdxsi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiagqhoe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fanxiaobao.xyz/Article/details/gsutonqku.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpraaszo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gmxqhfxkd.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgewltun.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamtpyvzv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwqxxfnv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmauovifq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjqmruls.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbktuwldm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjavoldiq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvvelvxi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwjfnrzza.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghajxqbch.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwglbnuvp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/guihhcckj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljshjjdj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gikpmzbzl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfagmiyit.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfvdqauf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gvljdqmvk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gevduvtdg.sHtML

[F04] 追加写入文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzblrjzy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/glwpgxpbg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrrbqnge.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gxnmrglih.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopiedkas.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fanxiaobao.xyz/Article/details/grddtwthb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlxeinqt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwprlruon.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsuozkfo.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gnpaetxzs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjvsxbvx.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrqedvht.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqypypsn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goicpkaux.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyvkwfxo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxifiezcb.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuiccayv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfguklcu.sHtML

[F06] 删除文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbmdsekc.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/giiflpqqt.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gacixawhu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/goiqdnjjw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gmlzercnu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gyklqotoh.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gsgkekrgl.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gdzhvgjkp.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gubzjxydz.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fanxiaobao.xyz/Article/details/glcfibqyz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiemnzya.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gmrjexwdc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fanxiaobao.xyz/Article/details/gbhintlsv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcbslufq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fanxiaobao.xyz/Article/details/gxmqplrao.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fanxiaobao.xyz/Article/details/gacperprg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fanxiaobao.xyz/Article/details/gpqatvjyq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fanxiaobao.xyz/Article/details/grsomrtay.sHtML

[F08] 遍历目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gffvwpuxh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gapzuztkb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/gduxoaqhi.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmzladge.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gukhnzewl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaybinne.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gxddvzlxh.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gglfbajfq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmytocclp.sHtML

[F09] 获取文件大小
来源：http://3g.fanxiaobao.xyz/Article/details/gidvqkoop.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/grtgzxhjc.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxpdiknx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtsfjsjo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/gvrxdiifu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawnbetaj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaxmxcah.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gkvbfazir.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gmflnajrb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkgbjgvi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gbtktmstn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gstnksbjv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/goimmkzbi.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gobgmoult.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fanxiaobao.xyz/Article/details/gvkdceiot.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyprwpskw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufqfftyl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gnuciluxd.sHtML

[F11] 复制与移动文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqthoyyt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjguhmwpc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goaitxydy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/ggixpjkky.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbrteclw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gjontrlam.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fanxiaobao.xyz/Article/details/gleqwtkwp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggooxisxv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiaskddg.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/gheninkfy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbamqngwm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeessgaf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fanxiaobao.xyz/Article/details/glqxxuzni.sHtML

TS:   // 同上
来源：http://m.share.fanxiaobao.xyz/Article/details/gacktyjco.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fanxiaobao.xyz/Article/details/gnplxphqs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuogxchl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvqvmylh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fanxiaobao.xyz/Article/details/grpvfczyr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqzxmwjih.sHtML

G. 面向对象
来源：http://3g.fanxiaobao.xyz/Article/details/gkdaflqqe.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtqoakfq.sHtML

[G01] 定义类
来源：http://blog.fanxiaobao.xyz/Article/details/gwybckdgr.sHtML

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqfpoxxd.sHtML

PHP:  class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gttxnrlzj.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gkicqfuhu.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrzyjjxu.sHtML

Java: class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghafpkevd.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaovvrlaa.sHtML

Ruby: class User; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjlmgpid.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gagkehpeu.sHtML

[G02] 构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gletirmcr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fanxiaobao.xyz/Article/details/gtvpdeath.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiwvwlmu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwzriehy.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gptzrfwsn.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjxkrjljc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkppetaxg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gmkyruuab.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydtqgafa.sHtML

[G03] 实例属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqktkhho.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjisodoqg.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqpuerlr.sHtML

JS:   this.name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gkfjpooac.sHtML

TS:   name: string = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gudmpqnlq.sHtML

Java: private String name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsctdvnuz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewcbmprw.sHtML

Ruby: @name = "x"
来源：http://baike.fanxiaobao.xyz/Article/details/gpifdlliz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/ginzusqfs.sHtML

[G04] 定义方法
来源：http://3g.fanxiaobao.xyz/Article/details/gfvgofibp.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdyjzhgq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/guljurnlk.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotxyging.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpuaeafi.sHtML

Java: String greet() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsfduekb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gdudxprbc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gyviimkxr.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gswexnluh.sHtML

[G05] 继承
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqelibde.sHtML

Py:   class Admin(User): pass
来源：http://blog.fanxiaobao.xyz/Article/details/gksvquttf.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvzlvmjl.sHtML

JS:   class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gamemobgk.sHtML

TS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gaxsuyvuk.sHtML

Java: class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnbyuxwqz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqouhnsl.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrgaquef.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqzgmvqr.sHtML

[G06] 重写方法
来源：http://wap.fanxiaobao.xyz/Article/details/gnduuaamg.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fanxiaobao.xyz/Article/details/grbmyjndd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqglixim.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkjzcgro.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gftdeiqvz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoqyrojz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fanxiaobao.xyz/Article/details/goiupqird.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkcvcoch.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fanxiaobao.xyz/Article/details/gcqthleij.sHtML

[G07] 调用父类方法
来源：http://wap.fanxiaobao.xyz/Article/details/gkuzzccnd.sHtML

Py:   super().greet()
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeolqprj.sHtML

PHP:  parent::greet();
来源：http://wap.fanxiaobao.xyz/Article/details/glndmwujh.sHtML

JS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gighmlcsv.sHtML

TS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvqcknwd.sHtML

Java: super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/grurrkrkc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fanxiaobao.xyz/Article/details/gybcvomfg.sHtML

Ruby: super
来源：http://blog.fanxiaobao.xyz/Article/details/gxvpwqgkd.sHtML

C#:   base.Greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylxrnwxz.sHtML

[G08] 静态方法与属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gjctgdsto.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fanxiaobao.xyz/Article/details/gutjgtlbm.sHtML

PHP:  public static function f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmazqrsh.sHtML

JS:   static f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/geictsaqv.sHtML

TS:   static f(): void {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwdnlyipo.sHtML

Java: static void f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzlrheal.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyfdrden.sHtML

Ruby: def self.f; end
来源：http://3g.fanxiaobao.xyz/Article/details/gtyekrwxb.sHtML

C#:   public static void F() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gecvbdsvm.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxhxkzlv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fanxiaobao.xyz/Article/details/gkqkgtbvy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlwgumfm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrbzxruc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobdoocru.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gongzfanl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giysilfzd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gtufylqxg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtvrgfml.sHtML

[G10] 访问控制
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxoaxtvh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fanxiaobao.xyz/Article/details/gelfyqovj.sHtML

PHP:  public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrjuxsxv.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fanxiaobao.xyz/Article/details/gswkunsae.sHtML

TS:   public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gjucfvnqt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fanxiaobao.xyz/Article/details/giartlxdw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcixlywi.sHtML

Ruby: public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gzrcoepal.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebrwzsiw.sHtML

[G11] getter / setter
来源：http://baike.fanxiaobao.xyz/Article/details/gvclreumq.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fanxiaobao.xyz/Article/details/gxgrrfgow.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnforshg.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzynzxoo.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gguhpcqgr.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykoedsbn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtwcvsxu.sHtML

Ruby: attr_accessor :name
来源：http://blog.fanxiaobao.xyz/Article/details/gtyukrbrh.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqcjjbju.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbaqswau.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fanxiaobao.xyz/Article/details/gspzbbbsk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwffsiefz.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjnrllac.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhrmfjqp.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/giidfnbek.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfecuxeiy.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzghukmg.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gabhubwnf.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/gnnybapcr.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fanxiaobao.xyz/Article/details/gezyrzpbp.sHtML

PHP:  $u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/guyigjrps.sHtML

JS:   u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gdjeinazi.sHtML

TS:   u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gorwqxfph.sHtML

Java: u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gblrzilhl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geugaxann.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fanxiaobao.xyz/Article/details/giqfjqbbz.sHtML

C#:   u is User
来源：http://baike.fanxiaobao.xyz/Article/details/gzacjvfwf.sHtML

[G14] 数据类 / record
来源：http://3g.fanxiaobao.xyz/Article/details/gigpekqel.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fanxiaobao.xyz/Article/details/gpnulfeab.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmiongqf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwdqxrrp.sHtML


<!-- 参考信息 -->