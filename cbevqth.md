代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gcexxakue.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ggapqtfcr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gmqopnsak.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gthbaoofz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gdpgymtnk.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gsbmlizng.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gefopntfi.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gykoykxzq.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gmatciwdg.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gttvyxhfn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gtrvidgzu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gzsudswvk.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gquzdxnsc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gzrsmenyu.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gbjrzuewd.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/ghufjvxpq.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gaxrpnkob.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gxnyurvot.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gnaytwfhi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/grbkhxtcp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gucpgmnmy.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gwnvcujum.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gktubkkui.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/glgbyhdmf.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gozpzutio.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gydqhimln.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gsusxvdxk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/guevpgbug.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gleiansde.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gbojstycg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gjpuovlxc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gnvjimixc.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gameiqbbg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/goamecugx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gihbtaxca.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gpvvxkmko.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gyltpqdmp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/giuzcwnzn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gjavexpto.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/grxbdccon.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gaalgthbk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gxuivmdxa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gjuiwqmbs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gckghiotf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gsjtaokvg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gvheoatyd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gwzkwfzwl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gpsaqewts.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gwaqywlat.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gcrflgtlv.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/guqdievsg.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gdczecaab.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gtuonfwao.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gnazawvje.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gxczcdjez.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gwmgsqylw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gaszdmfiw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gdirajqzp.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/glghipmrv.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gpujuzmkb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/grxsegjpo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gjxnhkvdk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gmxgwkhrm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gomzcrayb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gwxhyftth.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gdztaurix.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gubxofdqv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gvwtjmoqa.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gfpfegyhm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gznwvvfhl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gnydvjxmt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gpuvdrrnc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gaqaiefld.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gktuzhhwe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/ghhtkqbbh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gfbaytbvo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gslvaaart.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/geckisswj.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/giutsdijk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gmlrnyohi.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gnaahdfrt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gtewyhgqu.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gyvcctlne.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gifojodyb.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/ghlsdstgx.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/ghhvefiwk.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gnxzkqhhc.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/ghysimtpb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gfkshmhxp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbrhvjbei.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gevzojymn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gagysfcae.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gjkvptkfr.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gyduixjjw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gbrxwfryu.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gauxxkihg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gdxlqgvyk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gvwfjbmel.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gzzlsuwer.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gbnsimoyr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gajqadtuu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gvwfnwctd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/glnnlsmej.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gqhpwhmqs.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/genpdexfq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gsbgfdgds.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/glsoufkqt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/goaiuerzr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gnqrxusma.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gzphakasf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gmcvesjog.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gunweyhcu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gocnognrk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gihgcitnh.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gemvewwko.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbfocdyve.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/glvuoeeot.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gnopvgdac.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gmvovuoao.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/glhdfornp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gxjgjpztr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gysvpntuj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gslebhnbc.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjjnpjpaq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtjrigros.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gyyqgjmwi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/ghfzkcpxk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/glkvsixyq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gwltlydhg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/grbxpqgfu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/grvrtobke.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gtxlepcsp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/goukyxmqy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gbkjdrkiv.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gjieknrej.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gxcdflxxe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gecxmwekl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gkrkvpdwp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gkpvaomqf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gkfdsqexk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gestkpkix.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gdykbbfvf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gjfgxmuys.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gstpnxroa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/guhvdqpih.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gffqhluuy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gjqauzmvb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gaxwfvwpv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwhapqbi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gtzaeerjd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gzkxfrzvk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gowasfxfm.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gfwrfwnpm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gfmgwhhvd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gokofftzx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcnttrgwi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gylgeghms.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gljvdvcqa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gvacdxtdj.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqyffhbnh.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfudigjip.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gteoijuuy.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmaftnxrp.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxftnalzc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gicmquprr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gicvzidkf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gtjnchfss.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gidrnktdv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdehhoveb.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gslqoxfas.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gyuttutix.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gpjlbwleo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/guedyjugo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gmmsthkur.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/guhfadsif.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gtlypwdun.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gqzzcqkgd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gsfbnifng.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gfobpyece.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gvugcgkjw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gutefgkgv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gkilgnrkj.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gkoryodpt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gkvhogycl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gcmzjuhkt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/glhqlzpds.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/ganzvjivm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ggxdxzmlw.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gtrzijboq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glcoskhfh.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gycgrwxqj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gyvlnkvdy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gumoxhqbw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gneytltxu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gpmaxnhuk.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnppbfpzr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gnvpincun.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gxwfnamxm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/giqekmmfc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gdjvdrzpt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggocytdrh.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtiurouvk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/guusgqvcg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gghsvbgis.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gynfsnsxo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtygscnwr.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/girudnlti.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghkfytext.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcuaxtpfx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gacmjbums.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gamyniyqi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gqvvjoowi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gwmapyxfn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gkntawpud.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gbjrcxahi.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gmespzsdn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gukqgfdcd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gscbbtwki.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gdwhmohlv.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gixaekdnm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gespcshdj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gqcmzihel.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/glllnlfkq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gekwurkcu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtmdyxwhf.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/grmijinxt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gspugpifs.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/ggaldtoew.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/glckbgiid.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gfiyaelgx.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gexhtngvx.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gumurrygj.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gjktfegcb.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gufalexhc.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gbsbfvptu.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdlwjxfcj.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gzdyelnck.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/guegcumep.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gglblyxce.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gitmfliga.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gznuluhsk.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gabctkzti.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gffrafczf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/geeyirrrm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gtdbebgdt.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/geuwnbmix.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gvdfdlzqh.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gpklqaaaf.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gzklisygu.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gvyewanyx.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gztqvrikz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gagargxpa.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/guodrwwoy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/grdhaqfvt.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gecciygmu.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gtrhuoskl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gcxnvqado.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/goolmrgrv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gefdphmsu.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/ghfkwfeqg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gqlrrztir.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gespxpmbq.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gdryifpno.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/ghdfowmhm.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gbeqyvtmx.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gsnvzidow.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/glrvwrdln.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gplllzvei.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gdosspdfz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gspfmuxxg.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gwynfmfid.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gtuerehps.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gckupoupa.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gsmbqoxzw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gpxfqrorn.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gehbsxawh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ghkeielpo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gnnjgsjjc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gjpnrugcf.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gwqtvuxbh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/giamdvxdu.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gctlyftjl.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gkdnghjfn.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gsvxekxie.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gtnhklntg.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gzxgqctry.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gpysttdke.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gwsjoecwq.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/googfvthr.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gbcejfxda.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gjeykkkil.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gmrfdwwlr.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gcwzkzmuj.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gwfqgdcjo.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gycgxnswx.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gnrwpxyrd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gpnqaaius.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gxyxchzit.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gilbslufp.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gupyoytoo.sHtML


<!-- 参考信息 -->