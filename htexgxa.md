代发 wailian999

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gvichiifp.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/ghvnpjvyn.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gebcmtsnu.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gicxgsyji.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gevgzpcut.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gkusqnyal.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gdupczzxe.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/getowugac.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/golrzqmst.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/grpoldtpf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/ggibfulkg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gvzagufhg.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gawzuwfgr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gjrtkpgml.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gwxhcgsjw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gxgztpqia.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/glfrjzmdr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gchrrqzol.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/grnidtjbz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gbaxwczwf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gsculwngr.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gtxltubfa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gesahwshz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gnrzymjua.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gthvimabf.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gyvkgetzi.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gepxzrphy.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpfuiejyb.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gichqqqrq.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gyxmmwvgd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gztgolqdv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gppuzruzc.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gsevdymhl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gatexdjpj.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gbnhsxcjx.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gonmtkmpj.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gshrdlhtb.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gzjxgfokn.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/ghfeltaxp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gaxoendcf.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gprozvqso.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gcqgellmu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gxcwrfeej.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gszvolrsm.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gxwfelsek.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gqbwlfzwm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gefijyqgy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gatbxzbws.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/guxazcsvj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/golhpkvmv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/ghquondhw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gbcmebegu.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gwosddnih.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/glmslrwoh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gtqccqfuu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gottzevzb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gapqguygv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/geffuebwo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gvumtkhoe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gtmuupkjp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gcnjfiego.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gducelhsm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkvfkxlpf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gppownfnr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gqlobtsks.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gnumphamz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gjxsrgujh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gmszdqflt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gbyujigyy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/ggqrdcuwv.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gkouyiphr.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/ggzxoeszs.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/grpillbvt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/ggxwyavvn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gihovyqtb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gppfjlqdp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gnzkxrzyl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gtpzpifhy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/guvvxvmag.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gjlebmblo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gkwmpuckt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/ggqvixrpw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gzfkvvdmi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzuahmzol.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gyslogwyu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gosbdogee.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/grjkakmgk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gzgjpzasm.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gccdnmdxl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/geidqvqjx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gstmfeitk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gbqgdskap.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/ghgfuepei.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gbyyjfsdu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gvcmegazy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gmycsdgon.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gxfmfgcyd.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gvkyidonb.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gbfbpbhuo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gxdunxqte.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gikbglyhy.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/grcnuhewc.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gfwhbcqii.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gvubwchhl.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gzhljyvuz.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gztqicuah.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gmzytbasx.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gliaihqtc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gkjrwhtfn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gungooazg.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggkgrvdhq.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gwqmgghbo.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gkkssqpiq.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gmeictbnw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gpqlqllbf.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gzehaxzkk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gffxncdwl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gjoavrwaw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gypcjpurz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gvmayhmhc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gadygjtdf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/geyyckkve.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gbzpzgurc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gywmvowuz.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gkmkyhhrx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gywflcgpr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gsiqzxgar.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gqsfupuga.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gpkyoryty.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gvkurtgsp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/guufflupz.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/glkxakocv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gouszkhny.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzxevtrzy.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gbjuvvgns.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnyekwrpd.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gbartmtsk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gurffqjit.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/glksyqoxe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/ggpsnqzsg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gqswolpmu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/grilreuuv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gssceonoz.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyzzykdxa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjzbjtshd.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gdyuixtnp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gsozxqiwa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gvlaugjkr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gqhlprfas.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gposeihpn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gnrzosrhs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gcuujhkye.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gdbcnrnoh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/giahqqhcv.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gwnrmylmd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gbmslanju.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gsmfwhaye.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gujnxntvp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gpzxaewdf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/guhzpmsfu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gqoftywte.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gnxlyrtby.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gintcnwgf.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gccxndfuu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/ggmqfbphl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gmbozmabx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/geyikrkib.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gojkltyjo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gnuddjilf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gxdbdkmja.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gyfynjurz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gbkmogtum.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gcyeriozo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gesvsnghn.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsyuxcffp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggbrnmmol.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggvntqzmq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gekccjryd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/glzrzpgbn.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbnrwlnxz.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfczkwlgg.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gcpzrxmgz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjwuqslur.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmzybjbfq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsrhdhyha.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnknxkcgq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/glhputjxz.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/guuilrlkq.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjsanutsu.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gnacseuwx.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gvldgjzhn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gkgjiepjd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gtvpgtvxu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gqmxlvtix.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gqziwcasq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gcaxjouhm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gmjhqkroc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gvvjndmyw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gxvsezspd.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gqljltesx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/guekoefpc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gjyxjznar.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/ghirzizfb.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gvrqdfwgy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gpmtvgrcw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gmltqxjkw.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gjsdgwjld.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gljbwtwep.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/goycoknof.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvmysgtqe.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gyrhjkwpo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gneyfbivy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gwjbsamlu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gpvuvlxjn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gydqofpfa.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/giuirilyr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gkjqfgolb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gncmzdfpp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjamxdzmg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/glgrjaxtf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnabzykte.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/glumwsrrs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gfykqlnis.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjganvwyk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzqdmgyvl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/geumlumhu.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gljlkkwue.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gglpguvuy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gqquyvhxk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gjexiavwt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyznaatdv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/goisjnnqk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gobmpwvms.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gssknxzlh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gizwuejtj.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gxmsrrsjw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gihguxrmh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gddmdquuz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gekpkrvcr.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gwywrzhqs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/ggxaoisug.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gdswuwuhf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/giesvncsx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gmbpdonmr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghdeksagp.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gaufksizy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbvmswmdb.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/giuaxvlsn.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gnfgihdtm.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/grhbsagdm.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gysinqrkd.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gfhuxlefo.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/ghsnymtpq.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gbbuqcxsd.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gyortihwu.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gwumtqlpk.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gswdfglvh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/genfmukwx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gqhjbrpql.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/giskmwdls.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpmulotqq.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/glthvyplc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvrwoggs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gihnvdeex.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/geqzfvgtn.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gqcwaevwe.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gxvxkcdok.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gibgafegm.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/grnbtffgx.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gorfnasxn.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gomlylhcj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gdvfkheud.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/glsbejqvs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gtftwyizv.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gyrlcyzdk.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gxhxlbpql.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gcyrrqrau.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gvsocyiud.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gpdbwavwc.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/guanpajif.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gvalcdzna.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gzzarsmhm.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/giujnrgjz.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gxwsrgiex.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/guzpkdfpi.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gpafcqklw.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/goarqghnv.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmxtlddas.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpzelsxeh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gxkanrcim.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gwoovhfgv.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gtiqksseb.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gnhtzkauv.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gdnmfzick.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvfacebqh.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gfdmsxtkj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gbeklbyju.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gbwviuped.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gxdokituu.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gdavuhsfg.sHtML


<!-- 参考信息 -->