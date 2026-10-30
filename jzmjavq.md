代发 wailian999

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwwcoeni.sHtML

E. 字符串处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdrnpmeu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzhdvswq.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvfqixvb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjaavide.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcmgnvsy.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowytyyho.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fanxiaobao.xyz/Article/details/geyprbtuu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyavbawdx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fanxiaobao.xyz/Article/details/glanhzsge.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fanxiaobao.xyz/Article/details/gcsnhggrh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gznsybqnq.sHtML

[E02] 重复字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghcpbqgic.sHtML

Py:   "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/grpdxlftj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/guyelnpdy.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozghtppf.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/ghmarohbw.sHtML

Java: "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gjyqyfxqj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fanxiaobao.xyz/Article/details/glflwzbnz.sHtML

Ruby: "ab" * 3
来源：http://blog.fanxiaobao.xyz/Article/details/gxemfyhie.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gipyaciqu.sHtML

[E03] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgerwpbu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fanxiaobao.xyz/Article/details/ganoijgdk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/grvqjbiwu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gdhoazbwv.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcjkywrc.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzxedabw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fanxiaobao.xyz/Article/details/gsfkejsuk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gmduhpucd.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gywxhnyey.sHtML

[E04] 查找子串位置
来源：http://www.share.fanxiaobao.xyz/Article/details/grqccqwed.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gnlffcuze.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fanxiaobao.xyz/Article/details/gudapklup.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhocfcaq.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjffxassw.sHtML

Java: s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbnljtlz.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzufqvnx.sHtML

Ruby: s.index("x")
来源：http://blog.fanxiaobao.xyz/Article/details/glypphltv.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gmahglurv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fanxiaobao.xyz/Article/details/gyuoqgcpe.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gggeonhyt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpjjzlgn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gihesjrqh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcufwwxa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcmfbunr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fanxiaobao.xyz/Article/details/ghefpkuyb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpnbnzdv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gznmqcntr.sHtML

[E06] 替换子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwcjsodp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gabhfwqty.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gieozdxyc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknshijco.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gldioyweu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gsluobshx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsqajrci.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfntbiqgx.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldbmuzfa.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhxichdc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fanxiaobao.xyz/Article/details/gzuphnuug.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqisxdtwy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjbedkhv.sHtML

TS:   s.split(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gacagwnel.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fanxiaobao.xyz/Article/details/gmjwjecay.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fanxiaobao.xyz/Article/details/grqzevzzd.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/gahakzxiw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fanxiaobao.xyz/Article/details/gwsqrqghc.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fanxiaobao.xyz/Article/details/gqfahowsb.sHtML

Py:   ",".join(items)
来源：http://3g.fanxiaobao.xyz/Article/details/gdovpobdj.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrcnbkvs.sHtML

JS:   items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/grhqiomsa.sHtML

TS:   items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/glkwyylfr.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupalgkis.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fanxiaobao.xyz/Article/details/geagpllav.sHtML

Ruby: items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gfxzqaffr.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/gidjxhcab.sHtML

[E09] 去除所有空白字符
来源：http://wap.fanxiaobao.xyz/Article/details/gcvbcvffw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gtbcohtsp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvheqplpe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/ganqiqhip.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhhgfftm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmekceqn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fanxiaobao.xyz/Article/details/glreguvci.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gblnmbydx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfboptgj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fanxiaobao.xyz/Article/details/gfombyfxf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gxuktnmwu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fanxiaobao.xyz/Article/details/gylktxljf.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoezvksh.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gespeljws.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwxjqanm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsxcgssm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyejifta.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngzsptas.sHtML

[E11] 反转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfctyfkhl.sHtML

Py:   s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuztfzjx.sHtML

PHP:  strrev($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gmonfvstu.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxsgnmul.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gmoyekrcb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrldpszl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/gishxtxlh.sHtML

Ruby: s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/ghaskmqac.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/ggjjxqsjs.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fanxiaobao.xyz/Article/details/geczknsbx.sHtML

Py:   s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/glunyvtbq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuctdjah.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gijcoefhf.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghspvbpwm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fanxiaobao.xyz/Article/details/geymbaskh.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fanxiaobao.xyz/Article/details/gnddjzfaf.sHtML

Ruby: s.count("a")
来源：http://baike.fanxiaobao.xyz/Article/details/goimbmpeb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fanxiaobao.xyz/Article/details/gmiqgtyjm.sHtML

[E13] 逐字符遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gluftjqtt.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fanxiaobao.xyz/Article/details/gkpbdobyv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsjbflzj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggevwtllo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/getpzyhta.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfxdnnkk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fanxiaobao.xyz/Article/details/ghipaxifd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fanxiaobao.xyz/Article/details/gzaqcnnhe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtjbeeam.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gicumvlbn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkwynhvr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjvslber.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fanxiaobao.xyz/Article/details/gdrxxegne.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fanxiaobao.xyz/Article/details/grbqfqowr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhutnzzz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fanxiaobao.xyz/Article/details/gabxsgsgz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fanxiaobao.xyz/Article/details/gwwycbxyc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gteiruhtw.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fanxiaobao.xyz/Article/details/gdtzeahbg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlfapxjn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gqwzamwbx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuimkrbt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxcblksu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwurzlnhh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gdjxvdsdt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvirxbpx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gajxfxsda.sHtML

[E16] 数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/grabzydvk.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubjbjbdd.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumufamze.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/goopjnfkw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fanxiaobao.xyz/Article/details/gkbcjvejn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gtqtznnuw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpxogejv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gbjbapryq.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fanxiaobao.xyz/Article/details/gpyhdffqh.sHtML

[E17] 首字母大写
来源：http://blog.fanxiaobao.xyz/Article/details/goeelsbqm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fanxiaobao.xyz/Article/details/gdkdvbvfd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnufxlkuv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjdktjkj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtqbipcaf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggomgrkjn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqmeseib.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhqkdcdf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fanxiaobao.xyz/Article/details/gxmyibxxf.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrsreqrv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fanxiaobao.xyz/Article/details/goehxxagt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzczcynbm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdighkwv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/glwyngous.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhtowtgn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gvgfoovdx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooibtyrr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grtluuian.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqvljpux.sHtML

Py:   s.splitlines()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgvlbdig.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupemsjby.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwyuhsjz.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gbnppzfbe.sHtML

Java: s.lines().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkweelwcy.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gqwqqhzke.sHtML

Ruby: s.lines
来源：http://3g.fanxiaobao.xyz/Article/details/gsnnbwzjr.sHtML

C#:   s.Split('\n')
来源：http://baike.fanxiaobao.xyz/Article/details/guxogapzr.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fanxiaobao.xyz/Article/details/gwdzwujqa.sHtML

Py:   if not s:
来源：http://www.blog.fanxiaobao.xyz/Article/details/godwjvnez.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyqjquqa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqqhjmpt.sHtML

TS:   if (s === "") {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grcxzuysf.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gftvxyoax.sHtML

Go:   if s == "" {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsfsgzqf.sHtML

Ruby: if s.empty?
来源：http://baike.fanxiaobao.xyz/Article/details/gpzqidpzh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghakjffeg.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fanxiaobao.xyz/Article/details/glkvbpqnk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzxbscfd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/glnjdyhbm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryonictn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavporyru.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gqjdceuro.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fanxiaobao.xyz/Article/details/gjcgwlbgz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwnrdvnl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhzqtovu.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fanxiaobao.xyz/Article/details/gpbrtuyqw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvchvuawp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gdmblbzfs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmwnzcza.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gatlhbisk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/gsfxsyhwv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guumcfxku.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gbttcowrx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fanxiaobao.xyz/Article/details/gqxnpzbww.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzswtdtkr.sHtML

F. 文件与目录
来源：http://blog.fanxiaobao.xyz/Article/details/gvsdjsrdi.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gytwpjekl.sHtML

[F01] 读取整个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkdwwukll.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fanxiaobao.xyz/Article/details/gpersiwee.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyjgguev.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fanxiaobao.xyz/Article/details/goudpadjw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyfgstop.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghftgjlke.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqdhtrkh.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxeknfjq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gxosghkpd.sHtML

[F02] 逐行读取文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzjwvwso.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnqgcxuc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvcweeml.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtvtpotgi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyotwsod.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfwmcduy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fanxiaobao.xyz/Article/details/gqedoelgp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fanxiaobao.xyz/Article/details/gvglevskp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gddzuizfv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fanxiaobao.xyz/Article/details/grktbbijw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkawfejxe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmoaueny.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwtgqbhl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/grewjeqwu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gszbatlpi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfehtnyh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhcfsbcf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmhdzktj.sHtML

[F04] 追加写入文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvshshwd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gdjqvuhsv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fanxiaobao.xyz/Article/details/glpdsniuw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gmwvgmlff.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpalqnwgq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfapawiu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gouyxxxfv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdagrqyfw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcqstysi.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gxvviorbg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fanxiaobao.xyz/Article/details/gjmsgymyi.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtmtxahj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gajltbkgx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxmwyovq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gytuqjsxl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fanxiaobao.xyz/Article/details/gguqchqdl.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gdyyqfdhd.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gujplzdqz.sHtML

[F06] 删除文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcyipethr.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gonlbicke.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwkqkdnc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkdgbjyf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadinkbtw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/grkgbjeyg.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gpyvgmfjs.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkdphhja.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjvbucyo.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyasimadl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyjjdiih.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzgaxmtg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdzrqrvv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeddswxh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fanxiaobao.xyz/Article/details/gioovinks.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnubrpcl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlklporz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjonrdup.sHtML

[F08] 遍历目录
来源：http://3g.fanxiaobao.xyz/Article/details/gvnlfnwxw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxqmomik.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxombpyns.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gjtyelpnm.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gcpgvzllk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gicjdaydv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gjhrrzmzh.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gofztqwda.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxdnmxnp.sHtML

[F09] 获取文件大小
来源：http://blog.fanxiaobao.xyz/Article/details/glbatypef.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppwzlkau.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykrnlxxq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/gmcixhywz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfqcaqpn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gibzqljze.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fanxiaobao.xyz/Article/details/gogdbqivs.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/ggtaetbmx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fanxiaobao.xyz/Article/details/goantelba.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fanxiaobao.xyz/Article/details/gmfdcqtmp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsfhtbfu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gvocomype.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmapmanfr.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gpuqjamib.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fanxiaobao.xyz/Article/details/gixrrfnrf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/ghyniurle.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbuxzwxm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypcatgqc.sHtML

[F11] 复制与移动文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzirabclw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/giftuzbgc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkmpqqde.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnneesbhn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaaslxiu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqkkmade.sHtML


<!-- 参考信息 -->