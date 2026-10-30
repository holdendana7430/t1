代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gdicnvisc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfqqdpdv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuydquqz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fanxiaobao.xyz/Article/details/guuwdgnpd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdztihdp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhjkwmhm.sHtML

[E16] 数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/grwojbfaw.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gybrupsxq.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbcydzyj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fanxiaobao.xyz/Article/details/gcnddzcem.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fanxiaobao.xyz/Article/details/goddlbpsa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnlyprcn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjbxvzlv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gispedbwy.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fanxiaobao.xyz/Article/details/gchgvvakz.sHtML

[E17] 首字母大写
来源：http://blog.fanxiaobao.xyz/Article/details/grembgrwv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzavzjoox.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fanxiaobao.xyz/Article/details/grwokdoej.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gihbqbfoc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fanxiaobao.xyz/Article/details/guyreygcn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmrrlgdeo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmolbgzaa.sHtML

Ruby: s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/gcefbgrci.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fanxiaobao.xyz/Article/details/gyysaqitw.sHtML

[E18] 模板占位符替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grinpschc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fanxiaobao.xyz/Article/details/golthsujy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fanxiaobao.xyz/Article/details/gsspaehvh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gopsycvxk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvqxkhdg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdsfmioj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gskbuoelo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyvetppsv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fanxiaobao.xyz/Article/details/grliaqems.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxroptzow.sHtML

Py:   s.splitlines()
来源：http://www.share.fanxiaobao.xyz/Article/details/gibmzauzb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gputykkwg.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/gmkunweyc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxqaedaa.sHtML

Java: s.lines().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhyyrqrm.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/glsyzyhgx.sHtML

Ruby: s.lines
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhdiydqj.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicocolos.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaekmfio.sHtML

Py:   if not s:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuxvczwl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbbltoqf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqtdmmjp.sHtML

TS:   if (s === "") {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gydvcajfe.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadulrqne.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwuklcts.sHtML

Ruby: if s.empty?
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggydpdrzk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtscjtcid.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcmkjdkf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fanxiaobao.xyz/Article/details/gjdkrobis.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxsblxum.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/glylgsweu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/glxcmummr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvvnjpwn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fanxiaobao.xyz/Article/details/ggtjzcqoh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/givpagvpv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gtexnvlst.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fanxiaobao.xyz/Article/details/grogjcvjo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywvhoney.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gldaqztxv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/geyuackjh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffjcyuvl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnpfmccf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fanxiaobao.xyz/Article/details/govejcogw.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gqurvrcdd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gjglbciuv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwzaavju.sHtML

F. 文件与目录
来源：http://3g.fanxiaobao.xyz/Article/details/gyygpsswu.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gneypoivj.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlacrslh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fanxiaobao.xyz/Article/details/gufdxkqtv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaxmggat.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbshompvv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/guesqxlug.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gzyelhllj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fanxiaobao.xyz/Article/details/ggvupwddn.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhpjkkvz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxewpyfa.sHtML

[F02] 逐行读取文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpujnufyb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxqdlmen.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glhvcbzfu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gukdykrrr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gommlsmqv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gymzncqoe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fanxiaobao.xyz/Article/details/girbpagis.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fanxiaobao.xyz/Article/details/giayhqtym.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fanxiaobao.xyz/Article/details/guhagoehw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymzfbzyp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gxxktwfbw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtmzkjtd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/gugvgsqyn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxpvolro.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/goubpdrqd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fanxiaobao.xyz/Article/details/gzziufeib.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gxihcrvxh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycruqnfu.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgefgcyu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/ghrleepiz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfctqlkyg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gnwhryxgl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhpmazzd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fanxiaobao.xyz/Article/details/giymoqosd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gviyadcov.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fanxiaobao.xyz/Article/details/gjzlzkqpf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fanxiaobao.xyz/Article/details/gpwvejqpi.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gkqwdyrvl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjsdlwhb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/ginznxomd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjadshhze.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gostcfwrv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmobzqmwe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqknoexz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrabraae.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlvqtpsb.sHtML

[F06] 删除文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsskoskdk.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/ghfqzsthf.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdwrfwhi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gblfdzcey.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gbgdimjia.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhvimgif.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqbwvyhg.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwkrfbqp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeylgwve.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyghrxrpx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/glwfvpvch.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gugwchfoy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gsekedvqo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupiryqcl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fanxiaobao.xyz/Article/details/gquubhqqi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkldgcjjc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fanxiaobao.xyz/Article/details/ggzxkopcm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkejruax.sHtML

[F08] 遍历目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gdblcvxmy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fanxiaobao.xyz/Article/details/gwujlitma.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewfwvygb.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gmcofibxh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhocfuaz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/giqrnpefb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gnvzxbhtz.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/ggkanxves.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/ggouxvzlt.sHtML

[F09] 获取文件大小
来源：http://www.share.fanxiaobao.xyz/Article/details/gfczfttjc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxguaujzw.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggaiwekrg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfjpsdoz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/gpqemtxpr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gkytjlwki.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fanxiaobao.xyz/Article/details/gomzlgigb.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gnmljeyos.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fanxiaobao.xyz/Article/details/grmijqgzd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fanxiaobao.xyz/Article/details/gndiyuxze.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gitwxsrvd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/glzbldvcs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/glicsjlde.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gantlsoxg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlwpaqjp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gnkqqdpsb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gwwfapnxj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxylghjxq.sHtML

[F11] 复制与移动文件
来源：http://www.share.fanxiaobao.xyz/Article/details/goqqzjfop.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/ggyqincmi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/guszfmwui.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/goimutaib.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyfiqlbm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gcljanorg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fanxiaobao.xyz/Article/details/guiupadwr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gdcucbjax.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwbgyhls.sHtML

[F12] CSV 读写
来源：http://blog.fanxiaobao.xyz/Article/details/gvenbwewf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgiljmgh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilvzscft.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fanxiaobao.xyz/Article/details/gbnthahhy.sHtML

TS:   // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/gaqmgiidr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyxvwwtx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbssvizd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbhpbvsu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxqnfzuj.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwjexgow.sHtML

G. 面向对象
来源：http://3g.fanxiaobao.xyz/Article/details/gphyejoea.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gangjlogw.sHtML

[G01] 定义类
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmfrpzol.sHtML

Py:   class User: pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gneqclauy.sHtML

PHP:  class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gzradhsoe.sHtML

JS:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyeqqdfn.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gynktpgel.sHtML

Java: class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywrwlxjl.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmulmfdxv.sHtML

Ruby: class User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwqrmhqs.sHtML

C#:   class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gyjyhrflo.sHtML

[G02] 构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gabfidvnz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyyscwfg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gojefbcxo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugxczoxd.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gteqissys.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdilxmeah.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmnlvjrk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkempgkl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnnfdimj.sHtML

[G03] 实例属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpdpfmbb.sHtML

Py:   self.name = "x"
来源：http://3g.fanxiaobao.xyz/Article/details/gshhqexzq.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdujrxls.sHtML

JS:   this.name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnfcimvz.sHtML

TS:   name: string = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnmazuhp.sHtML

Java: private String name;
来源：http://mobile.fanxiaobao.xyz/Article/details/glbafcpjg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrvphrng.sHtML

Ruby: @name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/goadmrxyr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvuiyqsl.sHtML

[G04] 定义方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbsfbbgq.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxdhoujk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpqyxftcw.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghefthccx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhypvaaw.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyzylwcm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fanxiaobao.xyz/Article/details/gquzgwrib.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gqovgnbic.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/gzsmqkczf.sHtML

[G05] 继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbgthzyy.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxpzyucc.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbqweejvc.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxenixsna.sHtML

TS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gozzblwqf.sHtML

Java: class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gybiyejxr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fanxiaobao.xyz/Article/details/gydrvcgub.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gizfunnlb.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoqiudaz.sHtML

[G06] 重写方法
来源：http://blog.fanxiaobao.xyz/Article/details/ghqtuqwti.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljhnoswk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grccfvzak.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gefqduxwy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxahfruye.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/goccgqmvo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fanxiaobao.xyz/Article/details/gzenwxgkn.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuxlewfm.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fanxiaobao.xyz/Article/details/gkungehph.sHtML

[G07] 调用父类方法
来源：http://3g.fanxiaobao.xyz/Article/details/gemjsvozx.sHtML

Py:   super().greet()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsnjirqj.sHtML

PHP:  parent::greet();
来源：http://3g.fanxiaobao.xyz/Article/details/getsykmfc.sHtML

JS:   super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdqketqu.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmwauioa.sHtML

Java: super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gubgsqybo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fanxiaobao.xyz/Article/details/gpjeusotk.sHtML

Ruby: super
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzskjhus.sHtML

C#:   base.Greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsyrgurh.sHtML

[G08] 静态方法与属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyvitclp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbvaxgtj.sHtML

PHP:  public static function f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gynwnfpuu.sHtML

JS:   static f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjnyqgsls.sHtML

TS:   static f(): void {}
来源：http://3g.fanxiaobao.xyz/Article/details/gyzmcjoic.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwaryhogy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fanxiaobao.xyz/Article/details/gziegappb.sHtML

Ruby: def self.f; end
来源：http://wap.fanxiaobao.xyz/Article/details/gfqsgdzsk.sHtML

C#:   public static void F() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwgocnrsh.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fanxiaobao.xyz/Article/details/gagubghuw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvbrmkrv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpvueljkz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fanxiaobao.xyz/Article/details/gekbxaryq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsulpdcty.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gctokkmgc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gieucgbuv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusfpzulp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gomrgkkrj.sHtML

[G10] 访问控制
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzwidnzi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fanxiaobao.xyz/Article/details/guvqzwukd.sHtML

PHP:  public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gjndgzvww.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fanxiaobao.xyz/Article/details/gixmcmjsz.sHtML

TS:   public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gtratrlwq.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fanxiaobao.xyz/Article/details/gapdbecfi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fanxiaobao.xyz/Article/details/gayaulbtx.sHtML

Ruby: public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gduwbkzkk.sHtML

C#:   public / protected / private / internal
来源：http://blog.fanxiaobao.xyz/Article/details/givkbvkky.sHtML

[G11] getter / setter
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghucwqpoe.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcuwggmz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzmmstyl.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gyrbpbmiz.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gblxwbccg.sHtML

Java: public String getName() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwyjoikzq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwqbbgnj.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwcobzirv.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fanxiaobao.xyz/Article/details/glbepmuve.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvqdagpq.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/grbdjcwad.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpksugpz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxkfdhjr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebshidqa.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/geligwwbs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaaywoqf.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gcclmjvdq.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gufrmnjns.sHtML

[G13] 判断对象类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gkypjyilo.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsyydpbw.sHtML

PHP:  $u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gsbjxrqcz.sHtML

JS:   u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gifhcvhkk.sHtML

TS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gonahusge.sHtML

Java: u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gedcrnull.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fanxiaobao.xyz/Article/details/gtldjgnvg.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fanxiaobao.xyz/Article/details/golmuvemm.sHtML

C#:   u is User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqquwnsvr.sHtML


<!-- 参考信息 -->