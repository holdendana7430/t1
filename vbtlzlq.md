代发 wailian999

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gviwujutn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/ggmjqnite.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gkvwnxzfc.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gnithdpqt.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/glcxbeyaj.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gauafspug.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gingmeeko.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gsznabcth.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/ggnjslscv.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gbukgnufp.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gkkapsess.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gpltpzocm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gdfbziyze.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/giuelqadb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gfkddtrwx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/grmlylloe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gqwfdhyyh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gtdmftrmy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gmaufdulb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/giscyrjde.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gsyixtrlp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gsswojypz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gdnlbdkwe.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gaakzdxip.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gulcwtldt.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gtdmkpdwb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gbrhoufwq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gbfgezhea.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gasarplaf.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gbekjyeny.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gwtpyzvyr.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gvobxcevf.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/garpwalii.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gbqocseut.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gcswxafkb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/ggokhjotq.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gfrvpavru.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gujjmeext.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gfrsuzewn.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/grpyfxuzq.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gaffpzpyl.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gphepiqhq.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gjwkudlwp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gyftaewac.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gypynnrtg.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gdtdzuvhq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gpwifuljm.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gksqpxure.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gccvzytsi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/goppgsajm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gsdvmxqws.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gxogultwf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/glocxwtxu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gxvyhmfic.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gdxaoxfud.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gksqmqmfa.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/ggjwqxqpw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gskoyntpn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gkhyqfewc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/grfqnagot.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gjnzkuxho.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/ggeqscnlp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/givisbenz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gsagfpyte.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gyaiaidfh.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gzoirzwxv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gniyhqljw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gliwvqtrc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gydmwkrrx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gzwryjbbf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gbvjwawwm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gwkwvraeq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/ghlcxquop.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gxkkjuivl.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gmrlsqdfg.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gvzxcvcsk.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gzmeavgfw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gdyrdjpiz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gwoseaqup.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gjioefrfy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gsiejzvpb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gdtivjmir.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gdhkfcrlb.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gaiopadjs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gfdoqfkhr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gsbwabdck.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gpfosnwtr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/grhkwsoxk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gnnmcpgbc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gwcatcxbo.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/ghemtmttl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gfuwgkuse.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/goiyidlcs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/grxphdluz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gtmnlxhvk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/glbpzfbbr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/grbaqbwuv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gyboeczjf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gypqrwidi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gptrzejuw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gcspskzzv.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/grhxojcbq.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/glouzatel.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gndqhkbns.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gllhmxxic.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gjqrhtzzu.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gbrkfexjt.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gdbuvuewa.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gnbnneemb.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gcqfiitoe.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gqclivdzf.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gmxkeszav.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gokvbcqnn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gdwzytckr.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gbiwkjdni.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gisdvsclp.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gzuiygfen.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gwoztmpsz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gvhryspjj.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gwdspebvr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gugzynofr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gcpqweosx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gzaebhcrd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gzxxiwduv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gkipyjwat.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/ghddenhsn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gyamkkhcm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/grebcqqlc.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gdhppppge.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/grvvuslqd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/ggedxbldd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gfnbcdbqh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gyiggmgjw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gmmrcwuum.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gthdarrcq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gbimblfof.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gjwsydtbn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjafiljyb.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gcliznnew.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaxiygfpy.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gwjmbtnlc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/grkswdwas.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gfzvwaook.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gdyljzuji.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gjpresyma.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gqxmhzaey.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gbeqfqcgp.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfkmrsrvh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/goqzpvwlg.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gazttprzi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/ggfqevbbv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gtxtgopov.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/ghfddyrgj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gpccsjxwp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gjczfrlpb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/ggpfuyqmi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gvykslaup.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gtqqzwaea.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/glamwgiyg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gtmfpkhzg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gwvjxfgha.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gdtkuewlp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gsecmuifb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gpdadlmtf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gzlydimbp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gmrtkjckj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gsjxjadhz.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/ghbqsbtea.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/guxwgjiub.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/ggokgevdi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/glqvkisvh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gctmmecqu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gzvztlaeo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gvuikjfom.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/grdhjnlgf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gadjpwwzg.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/ganefmxij.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gbbegfbim.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/guumlcvue.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwezncbwu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxcpdfyco.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gwkovzinw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gqrbaxubm.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/guovxnpgu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glpjcyhft.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gkehtjhts.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaqiisbfm.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmqltgcrv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwbdikqoa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gociosobu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/grzuegibj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gofjpcfma.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gevmzejuz.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/guhgogtyk.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gzqiteyzl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gyyfyoxgt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gplhcvfla.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gjbahubpo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gahorcqyw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/geeomfabz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gaeyifnfm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gfkfnorqo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gvdvspsvg.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/ghiudcwmi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/glcxhtlhu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gohbzpmak.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gioaleldc.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/geymugrex.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcumbnyf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/ggjbfczvm.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gekxdiefd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gszxafohu.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/goyiybwoo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpkapssrl.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gugsygkja.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gberewpik.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gtfsssmde.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gnzqxqlfs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gwdacyikl.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzjnqzqlh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gxyqswpeo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gnlfmomqz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gknkwdkkc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gyhokjmjb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/grkxouksf.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmkbrrhfc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gcqdggjel.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gevbctqeb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcfkuqbfa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnzrbewtv.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gdozeuebw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gotbtltob.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gfvbyaiba.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gmkeyxmsy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gyvvdsfug.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gscmgzpbs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gujyuqtup.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gjoshomuz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gufbrzxbu.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gvshyrmvh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gavrfwvht.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gthiojbwy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gtuzpluqv.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gotlbnzyp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gkgagvfzu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/glmisbnxd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/ginabjqpy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gtaajovpk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gourhnsci.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gohydaltk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsogwukyk.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gokgvhkip.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gultveeun.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gqzrechaq.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/ghciuxdrr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/ghlrmqccr.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gfrusfffm.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gcklfiohy.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gibljluuq.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gqnoqwmco.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gwtallput.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gckflsvin.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gezsxkrqi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gegorwmpj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/guwfbddnl.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gvsaebcnk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gvamtqdbx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkugihtlw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gtbkcvsxr.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gqoifjooh.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gsfzfzezn.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/ghyfqatuc.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gniezymtt.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/grxzhxncf.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/geldaznke.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/grgmtprhv.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gufvalsnb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gfltmhmpt.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gvngoznqq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/glqbalgit.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnoldtibe.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gvrxwhvpx.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gtyhgbmhl.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/ggcqpfxck.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gffmnktiv.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gvsghiivg.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gwhmqcgfv.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gjclndbeq.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/ggqytjuse.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gvyuocpjq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/ghwrdcauu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gmsiuudnr.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/glnhbynev.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gdqheyhny.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/goqucknig.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gzrinuaky.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gbmfrqpkj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gwhiilfzx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/galaajdgs.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gegnzjjqu.sHtML


<!-- 参考信息 -->