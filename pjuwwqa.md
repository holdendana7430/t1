代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fanxiaobao.xyz/Article/details/gxdmcnrfl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrvrawme.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gpghsgxmw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gnuotvswc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fanxiaobao.xyz/Article/details/gmunxyzmv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdzbacyn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fanxiaobao.xyz/Article/details/goljpimay.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gdvgfiypg.sHtML

[E02] 重复字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhammduh.sHtML

Py:   "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gjghykitz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszvgohyu.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdchfcca.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxmffdfw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gytuygfps.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gycrbsyqb.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuebcnqp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmqpzgew.sHtML

[E03] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gorhliyey.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujyiugum.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfugdasu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmikeczrr.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gitkqbtzw.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrhivmar.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fanxiaobao.xyz/Article/details/gxkrskuki.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fanxiaobao.xyz/Article/details/gmguitpui.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoivgypx.sHtML

[E04] 查找子串位置
来源：http://baike.fanxiaobao.xyz/Article/details/gtqlronki.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtyzwroo.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fanxiaobao.xyz/Article/details/gbnwhljqg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqucwfuac.sHtML

TS:   s.indexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gctforzsq.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudwzhpfd.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gypwjhnhu.sHtML

Ruby: s.index("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gnuimawmq.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gwwvqekxj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fanxiaobao.xyz/Article/details/grqjuhwok.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gayekffil.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fanxiaobao.xyz/Article/details/gsjnotuxk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfvwzots.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdakcpczc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/geycjyonh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjeikfbz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxgwsusl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghumvqmoj.sHtML

[E06] 替换子串
来源：http://blog.fanxiaobao.xyz/Article/details/gqfgtdimp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkezmibdy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvrrqfps.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxhusvfe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gkiqadhuv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gqsyibmxd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gniatrdql.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gqxbafuqj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geetheuer.sHtML

[E07] 按分隔符拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gasdvscgt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fanxiaobao.xyz/Article/details/gogoutloy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gincxpais.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/goaryfavv.sHtML

TS:   s.split(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvzqefkg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fanxiaobao.xyz/Article/details/gagiezptv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/givivsgms.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/gpqduqxol.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fanxiaobao.xyz/Article/details/gcavwdfyh.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fanxiaobao.xyz/Article/details/gcukdxelv.sHtML

Py:   ",".join(items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvbqspyq.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtwklusn.sHtML

JS:   items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiiqknbp.sHtML

TS:   items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyvimsqq.sHtML

Java: String.join(",", items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvyjhpfl.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fanxiaobao.xyz/Article/details/gwctbmhvj.sHtML

Ruby: items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gadguspvj.sHtML

C#:   string.Join(",", items)
来源：http://blog.fanxiaobao.xyz/Article/details/gazllxrqm.sHtML

[E09] 去除所有空白字符
来源：http://blog.fanxiaobao.xyz/Article/details/gsavncxii.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwbbcgbn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhvlpynq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnaqgupf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gsskpeyas.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fanxiaobao.xyz/Article/details/gaflwncaj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fanxiaobao.xyz/Article/details/gwuqtzadd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeaagigu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fanxiaobao.xyz/Article/details/gspldhwow.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgaxmlxk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/guubmxblk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoikmfer.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gjjsamaak.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluanoonr.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gtvqweagd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gfaymuwzw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoxbdyoy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fanxiaobao.xyz/Article/details/gcobobsgn.sHtML

[E11] 反转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gqajutupz.sHtML

Py:   s[::-1]
来源：http://wap.fanxiaobao.xyz/Article/details/gskpsslmd.sHtML

PHP:  strrev($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkfpsgsc.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/godmcewzx.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gbjiyqeiz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gwjpyyprx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/ggvfwchml.sHtML

Ruby: s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/gkpgvopqk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fanxiaobao.xyz/Article/details/gxbcgflvx.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxdmvqdg.sHtML

Py:   s.count("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/guvqtmwui.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fanxiaobao.xyz/Article/details/gexbhwrvd.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fanxiaobao.xyz/Article/details/ghbzwzpwj.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjcicbnd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fanxiaobao.xyz/Article/details/gkhsdfrtd.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gokrzaqpd.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpeqqcjuf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fanxiaobao.xyz/Article/details/gvfenzytp.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrbdwrkr.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqlfgown.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvevzystv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwypweeil.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgpciexk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gefxgxwzh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gnqmstzae.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fanxiaobao.xyz/Article/details/gzmwsxqvw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gboqtploh.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fanxiaobao.xyz/Article/details/gcnlbezii.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fanxiaobao.xyz/Article/details/gfrxfwcjv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gbhnbpowa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goequulwf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmiynhlt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcxadapa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fanxiaobao.xyz/Article/details/gaaiydfkg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaxdkaqt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/guxlrjngl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuzcgmcc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjvklopg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gdeqneicx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gwgexldwo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwvxzxeh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fanxiaobao.xyz/Article/details/gjskotned.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuxsriez.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfcekrmv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gzkqvaapa.sHtML

[E16] 数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gurrdsytc.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/guykomlwb.sHtML

PHP:  number_format(1234567);
来源：http://blog.fanxiaobao.xyz/Article/details/gmqhnstmt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaqramqg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/gbhyazujw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohjirtrf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fanxiaobao.xyz/Article/details/gcypkrepi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gulzggcad.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fanxiaobao.xyz/Article/details/gicqwznym.sHtML

[E17] 首字母大写
来源：http://3g.fanxiaobao.xyz/Article/details/gvitlzlid.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fanxiaobao.xyz/Article/details/glewgonwh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gojmvagtt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fanxiaobao.xyz/Article/details/ggcfyodve.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxltjidak.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvadaeips.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfpcprxj.sHtML

Ruby: s.capitalize
来源：http://www.share.fanxiaobao.xyz/Article/details/gphatekvg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fanxiaobao.xyz/Article/details/gyhaicrli.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplyuffqv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fanxiaobao.xyz/Article/details/glzpuqkne.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fanxiaobao.xyz/Article/details/geffznawp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gulvuirst.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gpdwommgm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gmcngqbtq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/graaswjfi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvdpsbmhe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gasfhrgro.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fanxiaobao.xyz/Article/details/goobmqewg.sHtML

Py:   s.splitlines()
来源：http://baike.fanxiaobao.xyz/Article/details/gfmajabse.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzqqvqtg.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpuhecvx.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gbkrwrvhy.sHtML

Java: s.lines().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsjigstb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gymhmdlzu.sHtML

Ruby: s.lines
来源：http://3g.fanxiaobao.xyz/Article/details/ggiedkwxr.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjquaomc.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fanxiaobao.xyz/Article/details/gckfcwvfd.sHtML

Py:   if not s:
来源：http://baike.fanxiaobao.xyz/Article/details/gyzmlxavj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgtnwdsj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxmypqugo.sHtML

TS:   if (s === "") {}
来源：http://blog.fanxiaobao.xyz/Article/details/glajkbyfk.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyogftili.sHtML

Go:   if s == "" {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaegmkhh.sHtML

Ruby: if s.empty?
来源：http://www.share.fanxiaobao.xyz/Article/details/gikuldiba.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gpnjfaqzx.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgtlmvol.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fanxiaobao.xyz/Article/details/ghitdgjrn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gppbeeals.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gxwmdqkut.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/ggzvtsrrv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gsdulddpr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhuznkyi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gucgwfrkx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlzzapsc.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gtckfstec.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnirbpbvv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/grsjlvlla.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gifucdlxa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gxmtzmyux.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxlqotkh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fanxiaobao.xyz/Article/details/gentvolwh.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghewblsfs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlbbjmte.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjehsqpl.sHtML

F. 文件与目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gybbyvlkh.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxskgmqy.sHtML

[F01] 读取整个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxkgiaqj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjhmosml.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqxhnzct.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fanxiaobao.xyz/Article/details/glgoaqgvo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/granbjsuv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gqqomkkvy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fanxiaobao.xyz/Article/details/glljjlrpr.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnzvcxbo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguphksfz.sHtML

[F02] 逐行读取文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgzmgfml.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fanxiaobao.xyz/Article/details/gqruoohop.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghyobvtxl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkynbbpqr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/grsbreeql.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxedptqu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbugjtaw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fanxiaobao.xyz/Article/details/gothbdlkl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvgozmiho.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fanxiaobao.xyz/Article/details/gyslkqzvx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fanxiaobao.xyz/Article/details/gppzcwsqj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzabnvcne.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnqxocjb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/giijgtbsk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyziutgf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fanxiaobao.xyz/Article/details/gwlyjjjls.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgdhuxdp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gaszcmnwf.sHtML

[F04] 追加写入文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyimaulx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gxrkqkufw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgbrxmrq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwcliwzr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gqmkahfuo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmkycuwj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdkhysrn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fanxiaobao.xyz/Article/details/gqmsluomn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fanxiaobao.xyz/Article/details/glosjebpn.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gtbarhdwx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqcgdeck.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gpankdzgp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkoeosxc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjedtqxnd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmogcmonw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fanxiaobao.xyz/Article/details/gtxjasjyd.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gfijbmfmq.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnbyxxum.sHtML

[F06] 删除文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvfvtgqxq.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/goumjliio.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxvibabn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/glizntxbm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrandyur.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/glmxsfpih.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gajdrrifl.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgauzkyn.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkbdhgyd.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbiwwfli.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/glzajxpng.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gymkisgvo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhtwegtl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gogqtmsda.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegalecic.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fanxiaobao.xyz/Article/details/gzybyiknt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvcdhbtx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjsupkor.sHtML

[F08] 遍历目录
来源：http://3g.fanxiaobao.xyz/Article/details/gjiuobhsl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glelklvfy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmwefwpmo.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/glyquslqg.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gvmdjshqq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuuicqlq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gttsggibv.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gkprpotyi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndppmble.sHtML

[F09] 获取文件大小
来源：http://blog.fanxiaobao.xyz/Article/details/ghnoijrlc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfksakqq.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvbwhcrr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhlvwypr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gtblcbqbf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gownbzipz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnewzjdy.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gdcrhfrtr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzpoeroj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fanxiaobao.xyz/Article/details/gnsfeyqjb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjthbbpat.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/grqeaufoc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkxkqtil.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgmhetlp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fanxiaobao.xyz/Article/details/glcbduafb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gahtziyml.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gcnpejbbg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghswtxafx.sHtML

[F11] 复制与移动文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmytelbq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdlwnuxl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzdkhnrg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghygxhlfk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gztkvpics.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpticxce.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fanxiaobao.xyz/Article/details/guldmzsom.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gjrhnnfrn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fanxiaobao.xyz/Article/details/galugdokd.sHtML

[F12] CSV 读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnziiesi.sHtML


<!-- 参考信息 -->