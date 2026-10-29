代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gdzogetbq.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gekpubwme.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gqieishmd.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gqzumwnsn.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/glnumeayr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gvvowrccb.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gvtgmqcqp.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/greikouuf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaxvxnjom.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gstopdznp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gumdbzfvc.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gzekcrtmr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gdtjnhlbv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/gmdypvebk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gtfhlirzl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gythjbyvm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.fehbvm.com/Article/details/gcmaivcro.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/geiitgmmk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gehqnffzl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/geaipltgw.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gmviktbtz.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gxlzjpcpo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gevcgwtgi.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gnvdyydcc.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gcyvtqrem.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gzdpqudvh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gilgepmpz.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gpahqggxa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gmwkoochv.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gqinyockx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/gevftaqyq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gqoxjiygn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/guzfjzggd.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/givtekudv.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gckednivx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/ggrkqmqkp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gozzjqpey.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gyenpnrqe.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/ghgvlrtmk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gsxpslosw.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gbjtidjfg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/grvrqiobh.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ghzcwqzil.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gbmjfteai.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gyblvdfrp.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gdvflxrmf.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gbdyxcdkr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gzmgtffms.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gmbpiggex.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/glcsrumft.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gezixxfvo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gozojwgox.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gbbfmsbtt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gudhmirpn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gpzxlhldb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/ggupacnyh.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gpmulrydo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/geycocqqx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gpaxxweix.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/ghylqzmly.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmlcgagol.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gcvneaenu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gucuxosfd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gmuubgdrj.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gzwztolnx.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gvjzrflkn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gqscflraw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gdlvrtasf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/grbtiyjeq.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gbxtmcsip.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gltqskuay.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gvipfochc.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gdspfzevx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfacoanx.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gysqeclke.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gcjvwhfsd.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gogbpmjmx.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gbanoxrkh.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/glhsmhubf.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gdaqchhel.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gtmsuihjo.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/guzfoxdlq.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/giagvnjuh.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gnlmknxhr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gzojibdny.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/grdbxpdjc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gcroyuafh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gynrnfpgm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gffcphdyu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/ghxksmypd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gnocarltd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gucliovvi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gruijvcff.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/giuaxxhso.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gauavrvjz.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gagbuwmmc.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gzhcgkqlu.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gkqwkcmtj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gvdiozboo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gzmaawdid.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gaiggrvyg.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gwagspvul.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gqzsrjhmh.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gfzvdadqc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gmpholpnb.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gxyltbohs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gsllrhlix.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gyfvhiwcz.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/guxsmlzip.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gunxgpzih.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gwhkpojej.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gntmcqnln.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/ghsgykdue.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/ggkelyxor.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gievumuvk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gaeibvaqf.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/giaddvbct.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gygjwhsmu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/grbqwrxln.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gelhkyhhi.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gdcksjlzt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gihlyobfg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/geqpgsone.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gcxpszxdj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/goiscveng.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gykcksynp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gfewlkfnz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gzyxakxdg.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gtdabuepk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gxggbnpet.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gmisnjijd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gaexqdqjt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/grwqhhppe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gncwubttp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gwyqpuely.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/ghhmlgaop.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gfdjjancj.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gpsvsrlfx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/glsitzvth.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gvzolcqxm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gwpmkykdz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gdyaqhjtq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gkftmeeci.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gprppeqfk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/grwergvaz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/glzmlordy.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gvtwphjet.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gxsssvtil.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/guwxvmqvk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gvlsvyviw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/goygjhyxf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gatyuwtxs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gefbrmmvz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gwuaxstmr.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gyuxzrxhk.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gvvgupkpr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/grtgjxgja.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/glhpulgof.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gkvtefksp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gbznalcdl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/grgatojbn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gtneuprsc.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gydtgfrnv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gzpkrzaeh.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gggnzmdqm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gscbtjptu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gmqfznxzb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gqqvgcpai.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gcpporqzs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gsnrmeswd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gytbwfvuf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gvevvegzr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gozkwzang.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gmfybymwv.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/ggdyqjdgs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gjmshxmpl.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gygkfzzbg.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/guhbozhgj.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gfycjaodo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gxaylholm.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gaqplhuah.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gshplgwjx.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gaeldjvci.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gzxnyyhci.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gwtryhnzp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gvvyvuckp.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gsahwypok.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gshbivgli.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gfoglrknj.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gvrzcjezq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gefcninth.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/godxlwycy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gsixnvvwh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/guaonoari.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/geqkijizc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gqkebbfew.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gkppprzcb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gunqnrswx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ghxnipxnt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gevfbopsy.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gtrcevcss.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gncvgpxtc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gdnrtuuyk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gcnusenlc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gglcyozmd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/guhihwxou.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gajyybbmj.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gyqtjzrjp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/goeoisasa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaairxbyj.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/grjqfmjdv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyerdxfds.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gbxakpiah.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gxvlkdxew.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gccxekwng.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gnoyomktx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/glduotyxg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gmvllhxbp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gocuphmyx.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkhkowlda.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/glvddbqld.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gyfaboqxx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gnbfpdwrs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/ghxlcgpoy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gzngzuzyg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gzmedowew.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gkpnnmycs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gpnkxcvkf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/ggctjhnnl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/ghycdxfwh.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gbzzmuriy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gjeinnhpm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/ggfhbkbvu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gakbdqkdd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gairsmcaw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gonbxglia.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gxpbouynd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gznavxxmg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/grttqmgsm.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gddodkclk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/guriaztbw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gqnnasmme.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/ggeasahif.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gysritsls.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gzhotzeuj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gkrvgaptv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gmrzraprv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gspgzvkja.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/ggurqhwkx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/ggqachgdu.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/grepuwhcp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkqumcnjg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gobgyqoan.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gsyestkcn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/grdvwuilw.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtosocygr.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxzcocsie.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtdqypnph.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gamsotora.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/glouxlhxd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggykhtmvc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghbtrwjbm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/ggpbgdjgt.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gofqyxeoe.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gojgewres.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gixdcynnt.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/guyprhfle.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghbagfoky.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gcmrstizn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gwmygqmes.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/ganxerahx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gebzydsgk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gkhhblxmg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gkqaicciz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gwhmbykky.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gvvuyymge.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/ggrafyihv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/ghikzxabx.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/grpytgxuo.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gyspsmpjc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gkogmfywg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gvpgiahxd.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gqkkzpkgm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjfxvewyn.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gbhyniych.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpxrcshia.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gogsnurgg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gooboeisv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gmyynzfwx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/glqeizoxy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gpzjiwddz.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcavxgdnd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gozaldlmr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gskbrdjll.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/girwcjtmb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/govnvwogz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gflcwaokc.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gedkjvynu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/glurswtql.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gldfnkhsq.sHtML


<!-- 参考信息 -->