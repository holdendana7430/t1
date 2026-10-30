代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfhovsgm.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gzsxjfdlf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfhpdsev.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gmylxiqlx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gkbbzcmld.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gvtngyfdy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/galszsnzy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjxxzvhws.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gdcjlfrgy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gcvsmnfly.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/ggidhhgnq.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gaegdytbp.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gajjacfct.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/ghtcpfool.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gtktddzaf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gishesard.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gjlljyref.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gcufsnthl.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/ghkaekowm.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gdvztgmmk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gpuunycfx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbajtiaqd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/ggrdczfqa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gumcahqoc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnkayviud.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gdzrjlrvj.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gaestlkou.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gcuisxauy.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gpiszqpjn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gmmxzsnah.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/ghtnrumgq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gsojynlxf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gifottpxu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gugxvgybc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/ggmyekjoi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gfnavlbaa.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gglnnzmwv.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gkdbwgqrz.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gvjqdefvi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gtjxpzjmf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gkasturam.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gegimwnyx.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gnipfawzz.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gqwrlqfbo.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/ggxvysbby.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gwahoimyg.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gbdfvovkg.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gzhneoavf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gavvukppw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkpaneyhj.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gihxbutzq.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gftppffkl.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gbnfjoxoz.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gdxpoqyal.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gyjzlpasf.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gluiuzpcw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gjopzqmzw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/grurcdjoa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gvuzsqnvu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gxxdnqksc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gcoymmkrk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/ggnhopbrh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gxqncdtte.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwbxsydvd.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gjsqdtmne.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gwmohttha.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gxionczxk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gvteakofj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/glfttzfzi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gbpdxbanv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gxmrmprvk.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gojcyatyd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gmmyoxomi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghvmvmkkb.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gmqmehptz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpmaeqbnh.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gkeszalfe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gqppeygzo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/geopthxyj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gbcekedcn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/ggymfteet.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gojtcbmtj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/ghfjbelxc.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guglubiut.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gkqzznfjz.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/ggnvgnwro.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gvxmvsytr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gtnpdetjg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/ggwhjroux.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gunoozkna.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gmrlpfaxj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/grgshawkc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gjtgoldru.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gkapprscq.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gdgsaxxij.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gtwfisugg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gvtouohov.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gunukgktn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/geeqjaqio.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gxubbxwfm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gzowkomyl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gmlaceynr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gullchtxz.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gdhresepz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gpacrpyre.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gaaoqkvue.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gplaxupda.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gqlqbcygy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gexhhpoxi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gmhifbbfo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/glibcoktj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gksruzgnw.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gcezetuwn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gouqtsplo.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gikumqmxa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gllgszcfj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxhdgftmg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gvjkkjvdg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/ghrnvlfkv.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gicqammha.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gttlibxnw.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/guhxkqskj.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/grzwfqeec.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdofqvdbe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gblldggex.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfwzmltdd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gvwjnjwyd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbnlusvmm.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnlquzupg.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/grfywvnbr.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gmxivxadu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gvcnzwthu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/giqvodflp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gsjgqcgmy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gfhmudavy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/geskrxdcm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gqbniberr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gekyvonjr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/guhkixubc.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/glpvhxynn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gmecksbnv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gksovayqt.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gmgdpqihc.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/glmgeazod.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/geeionyhn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gnapgfvxb.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gxvvvtidq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ggscwosbf.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/goyreppey.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcgsuumto.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gdqdfxywi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gqlpgexxn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gyuhmsmlz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gskfsrzba.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gallrtule.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxjppdkcm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gjxxjmysd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gvggosixd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gepptduhw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gbkcxcfwk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gyyhonvgi.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwfvfsshd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gigxboadm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxgvvkjhz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/geextzgxv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcrakbnxg.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gpisnqkqo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvpmqtjlv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gwzggwnni.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/goxqbtvdv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gdlnzvxln.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gjpisclwq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gyeteqmhx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/giwemqent.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gtlnhfveh.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gpcgycnme.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gzgoblvof.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gmcycqjqn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gmrevnkxm.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gwbauwjbt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gxrueryet.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gbxehswnv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/ggkkcshyl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gynogwbmm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpzwnmbkh.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/glzndotak.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxblotrly.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/geygktpwm.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gzeodzlqu.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gglztdeev.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gfzxwgjnj.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gkmhejeby.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gvwtbksed.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gqruchxyf.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gwyewmzmb.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gfyefcmkw.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/ghdgqvrds.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gdtjcmprk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gajhemktq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gobwtretm.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/goydxtyze.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/glvkgnwzn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gevlhpbiu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gipafvfml.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gsfmmlqpz.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gqldpvcvb.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gqmwsfsdr.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gskdqumuv.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gyymtthrj.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gfyuqjykl.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gduvtmpai.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/ggwunkyhi.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gjbiotmiq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gnfjcoxbt.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gtcqeuwjp.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/ghlsjoltn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gpiiyfhim.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/geolvveax.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gusthmswb.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gseckzyau.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/grrtsguht.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gccceoewg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gczqhpulz.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gazehsyrk.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gmfndzula.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gjbibehpq.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gwxoaudgy.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gmvmshfab.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyrlhrrly.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gkmsajhbx.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gmjfohmyw.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/ghnpsotkm.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/ghcbtnanq.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gkjrnhgio.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gxuqsocnv.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/glmyxgetb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/guqsynkmc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggdhnhisd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gctntctup.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gpgkkjzgg.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gsupsvypc.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gsouohuxo.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gwsaccmdl.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gbnhjvjzb.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gjdneeaum.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gyjokhtnn.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/ggkfbsjqt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gjhrborow.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gznuwqhid.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gswthesop.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gokohldox.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gurhozwzj.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gajxarnfw.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gmnujxwyx.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gldzhgveu.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gdhspmhso.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/ggookyiul.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/ghovlevpy.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gbxkekhgi.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/grexttjho.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gqelkedju.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gujlgtxkk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gmlrlsgub.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/guqzvemem.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gtgegcnxt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/ghbftedkc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gmhfsstuu.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gbfkoirhn.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gkmyyhmei.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gmqgiylyo.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gfeoiwese.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gplgvxpzl.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gwxnedndy.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gwfnfuqtl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/grfmjuajj.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/guvtfhuqz.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gnprmfglp.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/guugyzify.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/grlgpokfm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtuwrmtfn.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gozcnxyex.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/ghjqdsxrw.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/glvysdnat.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gukptjqzj.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gnisgeely.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gjdevhlhq.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gsxumvfvo.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gpmtcdiak.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gvnlnnxso.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/ggalokhau.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gyeutqasw.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gpztivwgb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/grbuoqegt.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gbinfmjih.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gmhjxdfns.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gcdejspce.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gapzlffjf.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gntjwwnjg.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/goylxhrdi.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gwkmlfwjp.sHtML


<!-- 参考信息 -->