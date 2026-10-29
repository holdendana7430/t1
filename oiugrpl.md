代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gawjrnxgf.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gfbelxobg.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/guwvnwpgd.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gtaaxpuzw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/geklzrvqc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gagqditiu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gqmpylodw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gnwffocqz.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gohgznooc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/ggmkgthcn.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/giftjcqgv.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gqngcigak.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gtuyzjtwg.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gzavuhguo.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gosdfhgby.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gectfzpuo.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gvwbilrut.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gmqsdvqix.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/ghncmyesf.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gygodvbot.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/ghefaoxih.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gbhckxeks.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/greksrgen.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkhrwwud.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/ggdszpsac.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gogvptvca.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gmptahrpw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gmmqhyide.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gypxghtam.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gsovhpoox.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gjqcorlkf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gzctyitgn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gdqeaiqdm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gpbyrrflu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gxadbkndd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gqscfvdyb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gktcdoecj.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gcssqrdth.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/ggxabarxx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gvmgcvdhi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gdwbbiuuy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/grtqdismn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gigednusm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gmcxlaeok.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/ghfhzrzgh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gwhkkodiu.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gfljsdfqr.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/ghyeozlaz.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gvvonprsv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/glwjylgoc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gnbortmqj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gyeiqsdqg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gagbxofri.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/ggwqbxmqi.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/giwatimtt.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/ghrijjvga.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gkzflsoap.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/ggemrdjxk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gofjgutke.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgybcaik.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gpwistlvy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gbbhcilxu.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gggadxxvx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gynpgmsbu.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gdeaclnjc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gpipmdraq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/ghvgbwslb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gnorpjvds.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gtpxjsdxt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gsqxybihr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/ghgkqpswr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gkkoncfba.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gcovgovrr.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gsecqucwk.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gqmtpxxnr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/ggiweapdv.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gzgbqbbrv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gnhqlokyc.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gcxpjorxp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/giqzjefiz.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gntqiudln.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gxbldewxp.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gontblsqd.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gbrdthfkt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gkbtxhoum.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gayalzqjh.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gzwanngut.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzglrhslc.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gnxujaowp.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gddngnrzy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gcjzovjcw.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/ggpuokebm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gtuvvbcir.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gjswnpfmd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gyfhrtvax.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gteafwjox.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gerfhbfcd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gxiqcmixm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmonhpxwh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gcjjucnxx.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/giniysayg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpqmgykmi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gpiitaucm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gnvjeeeay.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gyycttmaj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gifqusfiu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gttvwyryu.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/graiareff.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gpswbursd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfkwlwdqr.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gudbdizwk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmuftohda.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gqcrqchku.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/ghdecgons.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/glzawmntb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gsrhmyhno.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gigiokdkg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gnhjrkkxs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gcikyhbdk.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gedhdbfdh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gtpregfro.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gfhesijxx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gkryupdtj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/guxqujqao.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvkafqjaw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gbedfwoiq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/ghfskeoye.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/guujqjadl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gdzqiadbn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gridbryev.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gjvttjpcs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gkpatzpoy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/glwnfevew.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gujzqwqus.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gzugdrscg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gnaocaxuy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gkheqsyhw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gztbiguuz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gfborbahn.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gqcrrrxjp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/ghdceygyx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gjgmqzqks.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gwslwdhax.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gnoirjbue.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gkwetelvs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gkqazlqrf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gysrxduzz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/grzohyohn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gnptcdcnv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gkpxnvogk.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gtltepgvv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfnwpnwku.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzhghkmte.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gpdkgpdry.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gmcdpwnpi.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gznxbinsr.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjybouhxq.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gcwoackrx.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwukdmtdg.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbeabusjq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpglwctpi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gclaaknku.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gkxvqymcl.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqktuqnlo.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdrwksbcg.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjbepphbz.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/ginvjymfq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gkfjotzdb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gcjvinfyg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/guxwlnlna.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gownnqtsb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gnpabsitp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gcnzkotei.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gznvuskyt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gpctiriaf.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/guvisfnws.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gylbcunna.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gbxiqiecd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gjbazcher.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gvtpwtoat.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gdjtxgtgp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gbphadbjs.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gpklyktbx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gyocxdhwg.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gpvcudvhr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcsbkzwkb.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/grpszckrd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gddofxsfw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gnylkswfy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gksiazyob.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/ghbnnipum.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmtvsptsc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gogfskhbd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gdavobynz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guamikdkq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/giejyztdo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvydfkdog.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjclabirn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/ggozyjews.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdqslvhoo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsyssvdxg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfbrwmdql.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gvvydxtcx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzmmrysgj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gaqggndvm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/giftkhkzj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gcbqxyeij.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gbafmcucv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/ghfhqwkzv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gswpakcgn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gcdtlxuqz.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gycdxqdjp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gcsavyvfi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gmukmhzee.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/ggqoeisxy.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gfrauylog.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gaufbawwb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gieopkfah.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gzrzrqsxf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gnoyvviio.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpidselpv.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gswbunygw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnkwcbqzf.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gmvlgsrqi.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/grmbinlvf.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/ghoqgblhs.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/grtqqprwa.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gxognwbks.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gehhgqjfk.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gjagbmxsg.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gzzlmhyoz.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/ghfwgpsem.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/grwaulmmg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gbytscgky.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/ggebolpsa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gcbszioow.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gpokdmtwl.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gqsgxkqgk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gegjexhor.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/grcbcadri.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gqtrdfbpm.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/glqbzasux.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gadhnilzr.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gdvrysgke.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gffucachc.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/guuxjmriz.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gszeugdyf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gqlnwlfmd.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/ghicawncx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gdbqcdrmv.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gyczxdzjk.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/geqzgpjlo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gouapismz.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gonaihxnx.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gbsheouni.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtiiahlpn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/garjvarvq.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gedrwkmup.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gibqstaik.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/glpapluux.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/ghgbkposq.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gpvqtlsbk.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gtmfejjxt.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gvgfwhvii.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gzgqntxic.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/ggiertzfb.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/glxhytljb.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gbnegjfoo.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gtzsbmrdr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gyfzgchot.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gdjhbjujm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gfesqpxuw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gdzoawgnu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gftqsvkif.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gekvwsvex.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gmegldvgs.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gzgwzfeyn.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gxkjcoupe.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gucntokfa.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/goiyroaes.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gzjhlxtdp.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gaievhoij.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gnljzuzmq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gbwsqzyer.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gcsnqysog.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gidgljnaz.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gbibwtrym.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gbthfixoj.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gdjvokein.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gbxqhnxlr.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gjqssyjqe.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gpxhlpexo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gzeyztrlr.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gbfbxxfrj.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gpwiesvcg.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/guujayris.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gbrvihfkp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gfikzrxbe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gkrohwvow.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gbfzhbqxs.sHtML


<!-- 参考信息 -->