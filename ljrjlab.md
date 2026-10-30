代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/guzmqgkrc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ghgcevtfo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gqcfoaorz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ghesnoack.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gesutwirg.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gzzzrxhll.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gqxldotkl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gjmtouizl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gurhjgaei.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gjlhrnysq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gjumssdfe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gaxzrbexv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gizpbmwzl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/glvyhknbf.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/ghzuzznxg.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/geycjcaev.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gjweodggd.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gjakhzxef.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gofzhnahi.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gbsmrnnck.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gubqgelxk.sHtML

Ruby: items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gfgpmpdjj.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gjcizphak.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gueyzsmiu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/ggpyhatil.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gbhisepqf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gabntybbu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/glpkakdxe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/glnaetzkc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/guyudrcmc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gbliqxbca.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gdomepktw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gejhnmhnz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gjqpehfvm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gsngzqadg.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/glokvbekm.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gutdzuyvy.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ggjnvdngj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/ggattttju.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgpuhqza.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gjzxdzmsi.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/grfxtrelf.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gimxmsygj.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/golhpeprf.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gphxdnamq.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gazgcxgdx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gsspcsfms.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gtbugvotk.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/ggpzrlbxg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/glfsgiqwc.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/grxfzhnnd.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/godnlbcyx.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gcmixdbap.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gvxpjlvla.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gktlxilsp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gtxsftblr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gsydolxsi.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gmvpqzdiz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gchdoyspu.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/ghvsjtwme.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gkafvruhk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gwyfgqhar.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/goqgagapd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gmsxlrhqq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/grugizmtz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gknsmmjmc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gugqmrwsz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gxaucmilj.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gixjikszj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/goyzgihha.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gtuyuuoaa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gwfrgbwag.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gmobljbsp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gfzqdphsl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gqbmeiawt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gwbifyirn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gweskgjxv.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gehqyhksk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gkrqhsbvr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/glpmmbtna.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gfpgykevw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gpavqafsz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/glzgkojjl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/glqkzuxmc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/ggoxrgtyc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gqpvbroks.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gowfglvgh.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gtwncycfn.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gpacvcpxd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gklfyhasy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/geurvdvhx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/guvuqwjib.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gxojkqahq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gogbapzie.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gerkzugef.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gdigonvov.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gjboycjfr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gypnciuyy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gtkqpcbwi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gdieebgsn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gikucphld.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gbdrgdrgy.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gawuyieuf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gsfxydvky.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gaaivsstm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gxounrgpa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/giwbhaiby.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gvqwnakoy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gyxccnnxo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gyuxeuhck.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gruaxrncy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gkrbyfijv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gblvguppd.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/glhutdllx.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gvpgbyssf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gqmdyuawm.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/ggqoouhwp.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gdrphpkup.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gnvpohevi.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gavbpufbf.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gofyjfejp.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gmbowfjtd.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gongskxsm.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gbdywoscn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gxjyoqzso.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/garscvgyp.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/glbedbwbi.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gtontjnit.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gkwsthldg.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gpxjbwwts.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/goihwykkm.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/ghipxttsh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gctojzvdv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gcjlfzpvh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gxzmeeake.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gtmmsuvyl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gpomvludz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gxdzcynbr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gxrwocqzh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gpxbmkafs.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gzrepieay.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gzqdgvpfo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gqveucnem.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gurrrlqyo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/ggkboycoq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gheclesfy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/guiycudje.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gkqlwmfyw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gsknjfqwp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjcwrulre.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/grlgymqvq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnehombwz.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gvykmejja.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gpmqaqtyx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/goptfqtvo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gdcoqrlyy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gwoyngojv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gcyexarwd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gffhyzkds.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghnyytqir.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjydilkmr.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/goegyjmxo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gbypqnyly.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gdqpwbyhm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gvnoaqupc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gxhwfcyku.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gysynwmyk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gecxiyymr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/ghxtflagf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gxoskbono.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gbcfbkcmn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/guyfoyvgs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/ghashsmfu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/ggeflcsce.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gxamxtkoh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/ggulzconk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gmutelvfx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gguccywsd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/ghspwyfib.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/guygcikfn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gjfbwjnrh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gdiakzuhc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gmcvdzdtf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gkoadftjs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gbucgnhdw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gfbfmklwf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gxxblhzia.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gfdyhzcnj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gccthkjus.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/ggugcweji.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/goyoelipd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/grlwffiji.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdjxdenir.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/goxgjcael.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gukclucey.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gndfsqzfb.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxqinojlz.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gttdgqhkr.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbymsvnvy.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gwtfchjjz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/grjixwcid.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdlziabqu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gqcfrsumt.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gljmmrldh.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkswseyag.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gxbtdzfxi.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gbnsfxufs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gkxacmpcj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gclncmwpc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gksemguni.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gbwprhejn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gxasqqgfq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/guqploptl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gdajbvbqm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gwrmszeut.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gmtxtvqwe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/giuunlqld.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gcjqugswj.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gelkllkif.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gdlxmovsn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gfnjckean.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gnjkvskfq.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gqiigkvxt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gsregsqal.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gputtezsk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkqitpdzm.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gaqiptycg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/guqqznbbh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gifdlsrrc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gydborqfi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gzsqarqdj.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvwkqdijp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gtwzbybnf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gcengspvr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjakssxnw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzkwrtbyi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvovyoydr.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwledulez.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/grlulowje.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/golhztpsc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gyiyapave.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqvafcnxk.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gbaxuspof.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/glmrqvbhh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gkwlfnkuf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gtbfkdwkt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcgeoezjb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyghcixri.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gdvotgbhv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gruplfncv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gtsutjpqh.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gzyqixmwt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gidjbslud.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gjuovdmfy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gmyzhfhgi.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gnwxfqhnp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/glwizescz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gfdejwzdo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/ghglsyhlp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gbhraboec.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkfmrbsoe.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gcfhpfhag.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gilqlaptv.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gnkafylda.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gnseuymeb.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gpzxtwjhf.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gcfonyxgk.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gbcqdkfos.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gfnfrwteu.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gqvndglze.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gvixcrjbz.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/galqhwmca.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gsldzqzfn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/ggrjcuxdo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/geijmyprg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gubwydpwk.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gtghwtecc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gtnoysziz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gnxzmavtc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gbdtfuqce.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/golxvqfou.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gbufhqaob.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gwvvfbbxa.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/ggzustxfu.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gepxamjrd.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gfqxlwpsg.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gwvrndlkc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gudjviydo.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/guubafepu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/grrrmzmxs.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gvjdjbdbu.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gewhwblve.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gsonoytof.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gwgezfrpr.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gssnptitt.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gkutgjgpt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ghswwznix.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gqtkscjif.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gswspwyds.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gykeesqyh.sHtML


<!-- 参考信息 -->