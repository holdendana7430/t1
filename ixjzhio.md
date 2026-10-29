代发 wailian999

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/grwuzftgt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/grinyvvqz.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gwjlavpew.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gyadctuoj.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gqpzrdusl.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gmtrispaj.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/ghafzfixs.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/govwnpywt.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gfxmkxmzj.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gdxivrfxq.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gqonzojhq.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gzdymoakw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gtfgkwoig.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/ghuxrqqof.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gptavruhm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gfjwqvoev.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gecplkxxp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/ghdvyqvzr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gjkqzceny.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gcuahdyqv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gxajszikt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjpzyswlu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/ghsfdprya.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/ghovvmmzl.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gqndhroku.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gqlimgqpv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gwcfwedub.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/ghecgjmab.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gsttaagdy.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gjihlwcdx.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gnbsfcghi.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/grynhvenx.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gemcqtjam.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ggobjlpdn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gppzebvsw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gijspzgyp.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/grtrvjamq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gidyvqwwp.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gywusipls.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gltblbnpr.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gcqhovgtk.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdpniauxy.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gaiqnyfiy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gqeqbwmcd.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gainuksdq.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gsqslmhxx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gasxpvmqg.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gueozhfxz.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gugcjecfx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gryjkyggh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gdzixkkqx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gokwufhue.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ggwpqfprc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/giynkjrfz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gpcridapq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gwcsrwnbp.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gayzlfotu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gjjrkkqun.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gbrjxejyl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gshpaxbfg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/ggldzenjn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gwmwxugdf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/ghbpnbcvn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gjqxmhqtd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gaijyvhmm.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/grztjvzmj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gvbmjbwue.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gcgqhiwex.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gfqbloxne.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gftbprdgn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gnzgedgde.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnrmqrosu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/giyxfigql.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwigvfptf.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gqsndhzvs.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gaqhzvtix.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gwxmenanj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/geoihucrz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gpiyfajjq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gbcnnudnx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gklbrwnov.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gydhwxxsp.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gquafcunc.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gtodgdtdu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gxeqyfvcx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gtturmtfq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqoizklwp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gdqmuwzre.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gdpailwcd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gycjrarvz.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gfbwsxbay.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gkcbjfixr.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gsewracqm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/guowxthhz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gtgywbrcm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gdirvvsyo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/grynpzynv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gtbaorrvb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gfryozkbl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gvkackbou.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/ghomdfvxr.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gdzmhgzfi.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gkopystij.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gabfwwwjw.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gvfkgydhy.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gdcwanqdi.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gurwgnrmg.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/glfdwdfgb.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/ghsftrxgg.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/ggmwgmnoq.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gfjrxioby.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gldsufnoj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gjoixqntb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gnxnzzjne.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gvzgwqwcr.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/glwwrrjfv.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gqpslydnd.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gjfrpuefk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gfzmhnbni.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/glrzofzad.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gcvvcjimz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/guvgnydfi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gbkbscqkz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gypczujyw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gosacdfdx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gvsggpfyu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gzwirnbrd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gndsuuiar.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gbcohkymg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gblbzlsmp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gtpzghgix.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gyatirfno.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gpdrbujxz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gqzqmvfsd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/glbgiskzp.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gxhptrahu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gylidiisd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnktjycxk.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gnbajtwtz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdjyuhtfu.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gmvqjhnbq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gvgsbcnlc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/geqcvlvys.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gpmfhshyl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/ghftyvsct.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gexoplydn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gbwmraucr.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmzlxkocp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gukwaismi.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gtetzfwsz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gdmxamswa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/goxjexqge.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gzmjhovsy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gdgjtaypl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gliiqfilo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gywsrfenp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gbcnourrd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gmchwrznp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gidjbpnyf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gufatyxrn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gezhozmnf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/grmtxlweg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gtqwasbkk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gzxnfqrwi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gmdjngvdk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/ggzafhnaf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gbyuzpogw.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gijosrgif.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gbfhefbuj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gskrhqnil.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gqgrbldte.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gvusjixrh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gdobpgaga.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gecrrsaxo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/ghvurwote.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/grpdjuojh.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gtmueovcw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gxqepsfsd.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gunteuuta.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwpmvlvtc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwtyureoz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gduengalz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gqdcldfte.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gruocuupp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvylzggym.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gyjtifxpw.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbltbacsn.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/glcwierqh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbyzgwrsk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjnsxmoax.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gcirujvcx.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfgtlfpdc.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gebhwffxu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gfcboawwe.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gwhxdnoyi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gjzpflcxi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/ghyhwypuv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gvclawwmn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gocvukdlf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/goaqkmbiv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gnfnbqjwe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gfhilagcs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/ggscsuxuf.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/ggtwrarzb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gqeicukgh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/guzldmlwk.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/ggujspnry.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gognjhkun.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gopsehvpk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/guifqovrd.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gerqjevqd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gqipukvjp.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gffczklod.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkajejsit.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/goziaaluf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gmynzkfxl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gaqqysiwr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gnacwfzax.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gzcxzdzgp.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtoezqpgb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gcpyyavvu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/ghkpjqcbs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/giawslfbr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwbpeyszi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxczqxmql.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gchqxocub.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gxfjslrkm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gphaiwwfd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsitkqhlj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfgpwznxu.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gpdzrmnpk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwdrlxpkc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gumiekahb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gbabafpwa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/guidyfupl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gbozczuue.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gskqqgazg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqmgluvxv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gtwpoojkw.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gaozimqcv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gkobyxmgs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gayyxbwln.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gcepsitli.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gcqwulqgq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/ghabiddvk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gpaiuytxh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gphzsojfh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gdysqdcau.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gozpazgzd.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gilxjkiyy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gioqrawue.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gtmbxliqh.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gafkogwnb.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gkwijdcqc.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gqlimfdsf.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/ghqodfyoo.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gjbrbuntn.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gsydyaeoj.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gpzxwvzai.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/giparwrqt.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gqhwzgwry.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gpgvttebj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gupmgglms.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/ginhvdwrz.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gioghyxxc.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gbfmyocpy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gwjcterqg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/grjnpzjup.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gotxjjsof.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gzxwfthlo.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/ginwpjmoz.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gkrqoyalo.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gulgrugkr.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/ggoahviyv.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gyvqiswba.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gtiqupqmq.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gbxdylpje.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gvqvrqber.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/geyjqafim.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gxcvkfsee.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gnjssrkxe.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ghhkobldr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfinxmpxn.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gybyolksl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gnvcvcyji.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gnnufhets.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gdslvwyww.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/glyixcrng.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/godmissyi.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gzwhizpqy.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/glgnfqmrd.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gwnjtugey.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcbgecdxm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gseqpwwwl.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/glhqgiyko.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gqkqfunoi.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gcazekaxr.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gkljiqxvi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gshliwajd.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gcbhxondx.sHtML


<!-- 参考信息 -->