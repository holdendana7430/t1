代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gteflcpfg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gnoxkmznx.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/ghfomyiji.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/guzreiauw.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gxhrlxndk.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gqwyxhiit.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gsktezyua.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gdewzuyde.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/ghlfttcwb.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/ggwpheqsx.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gqsgunxqb.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gzdbrbedp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gwcadmzew.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gbxbarbin.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gbafgdxig.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gmhaimrmw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gzarmjvlu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gvbkynvfp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gotwcmesb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gnoxskris.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/grjabgoom.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gofcewrev.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gextjpeul.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gywlnpnmb.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gyiigskfe.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gfcpqmbqw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gpjotflnh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gudlqkueg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/giiklufxe.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gblzvpgmz.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gbteivehr.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gjrdjxcpe.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/ggeyxvqyw.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gvncdjyfi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/ghhkuqvnm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gsmfnamdp.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gvbzjdwtw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gaigwxmmf.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/grsmbwugm.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gyleeymno.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gcttvebkn.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gxawcdfnl.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gqeolvonk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gvggudgxo.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gdqyuqsaf.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gjmszjnsn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/ggijncbek.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gomtjaaqf.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gmvcjlmej.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/grtlozohy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gcqzyqycy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gagegyemh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/ggbwiavat.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbcslkh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gfmafwjrh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gijabajpv.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gueuccnks.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gpjaktxob.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gmidqhwwu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gzondolog.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gxnfxmoqz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/ggclnalhq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gzmvgaggp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gdtswwoly.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/ginyhzvvk.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gdqvsfqjn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gsjopbahi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gaocoxocz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goqnovqvy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gvillqgti.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gbhuezqbe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gzsxwawqp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gkydsydhg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/giaphzvph.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/geqmnwzhs.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gwdorzuhw.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gribucrjv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gwwkupogp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gdsrltwot.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/grjigjfrk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gwtcwclee.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gagylpbau.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/ggspzofnj.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gqcwdesmh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gaxbnllou.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/grhonwiha.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvtxqvwdr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gpvhqcrch.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbfrrbocm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/ggefocumz.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gnamdmllf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gaocrrppc.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/ggkxhngsg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/giiejkchw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gfvdtgeap.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/glqsauvbi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gxwyqdtwx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/ggwjmuoit.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gbbtpgioe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/grokwklvx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gapjxwgmv.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gbjrizdbw.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gravxmhdl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/ghmhkkaur.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gbyeygtej.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gkodccnxy.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gwexfzoph.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/geexexaqd.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gaydkymlh.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gamnadcsx.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/ggymyisug.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gtfqhhoge.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gyxjsokcn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gszvffeor.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gtjepoajs.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gmdckjrsg.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gwinqkqfq.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gllleoqdm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gnwvsymwq.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gisvjvkgn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gciuxpktb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gdqmemsln.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gvrrigrrw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gxtdoqojo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gmjzsolqs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gxkkfozwr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/guxvdrebm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gwbvsdlyc.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gsyzfxmus.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gpspavxlg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gvvikpkuk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gkhaebmik.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gdznqrskq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gwzitxxjb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/guojbioct.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gdqsbcbwx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gkogfrdac.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grmodouxb.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gszdurlwd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gstfdyaio.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/giqjaupdr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/geqocptzp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/glivpkelr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/glatzfkhp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gkibbprlf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/grwayhsis.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gtjjyqqak.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/geudgwxag.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gswsykhfv.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gvpxwskgx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gvygfnggx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gaphzqwef.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/giiibuynv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/ghlxuzdit.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gulobwavt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gagfpgtta.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gseppilku.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gmarvtnhr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gdgcpsnfl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gxnlnyjos.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gevxxncxl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gakzhqpcf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gxkqvhnsp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gmozlhild.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gzuupjuct.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gfljjaigu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gdyixnpxf.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gcvashfol.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxtjdntcg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gtfieqaai.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gctljxpmn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gcxpzemwv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gsuynbtdf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gkrdyhwyd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gmolhbniv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gfvmqxszi.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/ghycfupbr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gawviunbp.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gybowlhhg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmvtrjfvb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gddgqyfha.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gaqsjynld.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gxlivjzjz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvmocljrx.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guwicdrbp.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gkeltzolb.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjodtrulq.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzpdenhjk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/giyobmayj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gccjdtdpv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gzinfpwqw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjhntymhq.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmmqiidmp.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gzsnlrbtw.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gadfkmmal.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gcccyqubh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gmdtfqvzd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gjyhffcxg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gguibwiwl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gjgfeqdnt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gtsmtsqln.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gmkdhmwju.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gxgdpvwij.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gzdhgmobh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gwgvgxjdq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gwaqfhzjh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gnswpxuew.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gckvtsivd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gfzguzwnn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gdwdocbtn.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gexrqzcys.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gzpffjoft.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/guqrbgrlj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmvbirqek.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzhtsnurf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gotlpgesf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gsgcjmcuk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gxfijoygo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gepgvxuqn.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbycjjubz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gkhyxkotu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gzlcabzrq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gakvjyssv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpjnfykfi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gciperyhm.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwzmjdqin.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gnpvyqtnr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsrutpvlq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gujrakepm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmrfhcdzm.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gibsprrjt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gdhgegfti.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grdigqaix.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gczbkynbz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gjbnskdxl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gugwurhak.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gisethiie.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gyfjblhng.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gnlyblbmb.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/guikarnbd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gttehhess.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/glklgoidm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gkhjgbcuj.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gvsqdpvqd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gnqrizwgv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/giulmckvv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gemwzwmtj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gpocueitv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvewuyeiu.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gkqfshaor.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkpybpxmz.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gpyzypwnc.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gkfvdswer.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gclplzcrn.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/govoxdxtl.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gtlpifoaj.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwgqrraxv.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gohnuryak.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gzzitryua.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gpivjupde.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gsuipkkkd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gqjibbgyj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gthujljxz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/ggaogeepe.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gykafczov.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gukudajmw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gduclfmjl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gnhqbrnsp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/ghtqpdeej.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gittwpqsk.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gbzxfdlma.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gidykmeah.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gnrkdqjla.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gacdxnctd.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gfxpcyagh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gsgzgzeat.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gytiylgvn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gcxrvlesk.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gioyyznwp.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gvjsfmqms.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/ggbldnirc.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gbbhgowey.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/grbnvboap.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdbhjkvnd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/glegvntis.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gzsfocaow.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gnqeoeejn.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/grhksuiiy.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gzzcpbfzq.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/ggcvplamt.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gzaahobsq.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gwghlcgpe.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gyrtpbkwf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gstazvhox.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gxfefmzlv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gktvickje.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gtvoigmft.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gzqczuomg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/ggnazlkwm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gwddyjrge.sHtML


<!-- 参考信息 -->