代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gqawpqghc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gduycluro.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gkivafopt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gsokphjlw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gtvrnmxtn.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gksqtzqto.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gzuhubepn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gqtdjirnf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtaglwsls.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gneplnclp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gknbaeijg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gpqednkrl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gvvuuxzjz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gfkrdtbit.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gesrckhat.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gnxsvqrye.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gpunimyft.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gmbyiprnq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gbcqymjun.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gwjstkats.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gnhnopxjv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gueebjpre.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/glkwddmqz.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gyxrikwic.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gsensqsjv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gpcvjnkly.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfyeguqiv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gmysfrehj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gscnnhoea.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gmbhxesat.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/guiuteadk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gbtkzuisg.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gxlfhtoxj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gtckaakgi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gxygmovec.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gjxmfhvhu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gwndjqzxy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gbvqnqsqp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnnyxtrb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/grebjfceu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gmrdjbgjd.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gtqrzbfll.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gepgustxh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gfymhqnix.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gtdontzwf.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gaduhqust.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gzmfjgkgk.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gfeesffwq.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/geaebaeii.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gkrgunohh.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/ganqwzcat.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gttuzmktc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/geewxiigf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzvplfbvh.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gixivemgd.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/grwbkjkht.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gircupeye.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gpattjyyd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gguouvgmp.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gctlasvua.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gyscbfzfq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gmfitsxqg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gjuizygxp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gvotaowun.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gakudilxe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gldlgfiii.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gamarxzis.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ggbeqyqwz.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gyjkiscwi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gninrcwrc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gefqrmajz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gqwkncyfo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gmskyjozj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gselzdebj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gxgyssvyc.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gommydiks.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gzopxzypv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjziehiue.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gwzwidzws.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcuwqssno.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gzoiyukpa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/govedikkj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gggzqpfbj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gnptkdnqg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gfcpglpvh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gxvlufgdc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gkujqjdqf.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/goaeulnti.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gvgsapblu.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gkxletggf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gaxbjicfs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gfffrkffn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gnlxmvhwy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gqdmtrzny.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/grlkobtkv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gfmucdizu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gyuobdlom.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gyfgerbkl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gtckvptzn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/garhsgxga.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gnqkrmbde.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gpobfqcvg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gkrjgugmh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gxngmonzj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gngljxmmc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gqbpamzrd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gdzlsndht.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gtnsdidju.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gfwspgyhu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gpxfunnwy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gehqyagcg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gvtwouhfg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gtvtxtwar.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gddoxiilt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gbrwauysj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/giukxcden.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gslsjteao.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gkjmamoxv.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gysvgyvqy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gopelkhgt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqiaeabbx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gavfjpaws.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gkrhfkuhe.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfhfnlrcu.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqnzbmval.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gjutulcqu.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grebcvykn.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghjymfqve.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghlquzzuo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzentsona.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gzkvdkjeo.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcjrxerxq.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjoxcdgdh.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvrxdlyce.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/guutqkgsi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gfkqcbmmd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gvdjdwkxh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/glngysweu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gotfvuhjm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gnnugxtiy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/ginawctjj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gideaghtp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gprjjaawa.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gkgvtxzqv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/ggfbnviqw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gjexlmpgw.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gqvvuowyb.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gjvhnhnij.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gdrcrdmwk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gcwazcudj.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gghintmih.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ggskigmvc.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gjvxdyovw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/grpumdzox.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gpsfdkxws.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gpxzxgqri.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gkydhwcee.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/ghjuknskg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gprsoihkp.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gukqmxius.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gzmfemfjf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gswgcuazt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmggngemk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gjldjmdjr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gxuqryqrw.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwrglpejd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gfpibxgwb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghucgmxdn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gutundoik.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gljecymff.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gekhuryoc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gaxxpwdbk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/glkhufbay.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtjedwxfg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gufdhfhwy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gjnvqhlpt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gehfkjqwn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/goyvxuecx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gikfkimoj.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gaqhynuci.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/ginfjojmv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gbqaymkqk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/ghemkozao.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gmhxujnms.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/geszgsvun.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gthmxtjbn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gnpevfgon.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/ggtfhmlha.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvjdchrje.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gupgswnjb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxfmwdvgl.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gggktffxe.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gisygyfcz.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gkfbeogry.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjecispol.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gmwvflvwn.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gcixqfypd.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/ggwiqusjg.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/guywxeiuz.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/guxuwsvgm.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/giwpfonki.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/ggzdpzbzd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gepymxyqv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvojzgalz.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gtknpfpjk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkcazuwog.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gqzuuzrel.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gknfblpuk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gcglwsyrn.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gdkjoeyuy.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/grongsnff.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/guljhgrtz.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gzxrgvdbl.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gelkpehku.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gfttvhzie.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gljtyqhez.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gznznvshm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gtdprlxfv.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gsgcqrras.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gthubchxs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ghrrsepnc.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/geibxxhch.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gtitutqse.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gmymnwahm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gyjqvnchq.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gmbjlgrjj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/glvjzabjr.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/grltgsnjs.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gcomakxjq.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gnenpfihv.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gxxmjfmkr.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/giunzbtoe.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gtnguviqx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gukdjamfw.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gczalewjm.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gyllkmqun.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gezpyaxtg.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gqwviiyrz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcqavvtrc.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gfnbkmqbx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gmzupbkwh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gxtbkylmo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gzlydbwja.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gincbpced.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gplndungt.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gxkwmsgzx.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gfrcquuxi.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gsttanlrl.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gaegdwiia.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gdleyxoym.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/ggmukqyih.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gjxzrcwsf.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gmnwajfsk.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gtjxphlab.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gmxemorwo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gzhjblrrn.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gcpqpcoxs.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gdegkdxwh.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gzvdrvubq.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/ggxpcxuvr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gqldyggrv.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/ghqvrnrge.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gmyymmtwz.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gwbmnfmry.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gpegtaaud.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gvjohiees.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/girdwmpue.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gnmmwndnu.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gpddhhxhw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gtzdsdeaz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gkrxlznbx.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gpzkfmtmb.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gsecracxc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gakyfzmwu.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/genjimkdz.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/goqaiyewr.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gsnlcaqia.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/grvqmacmy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/ggrhafamq.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gbdoxmrcv.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gncqloxuh.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gvlthuvuk.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gdvgliaid.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gdsnnxohb.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/glhwllnsk.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gsjrvfpnz.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gnwufrusj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gpoqvklrw.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gjtdeplco.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gklnqbtvw.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gpzgztxuv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/ggukiqpvu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/ggepvrdfz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gokqmsurh.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ghpubyzmr.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gdihtkiam.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzwdgdmho.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/giwnswjjo.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gflbqeujb.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gjtaufdzu.sHtML


<!-- 参考信息 -->