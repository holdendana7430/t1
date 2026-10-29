代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gmkmmfgrl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/giszwqvrn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gigoadzpu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/glrqfvgbe.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gyhdgzstc.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gmunowmyv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gmhckbtwn.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/ghokbnaof.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gdtajjzli.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gwivgiadh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gaeiwnnyn.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gumsumrpv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gdurcndco.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gzpxbbsxn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gqlwyfbwj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ggwgmapmi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gaqexemcl.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gkbosqpaa.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gpealklas.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gnclqekxk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/genijtpzp.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gojpnnlcc.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gzrjozqjz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gipjoctpg.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gjmaikhri.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/ggelrhgmv.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gujenqlnl.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gbhpgpxfu.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gsuiacqiw.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/ghnvviiqw.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gurknrggh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gfijzrarr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/goipjwnrc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gsedfjdho.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gasbnatox.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gbqnszfbq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gsqgiozyy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gdhfkiatu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gyeyojddq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gszvppnkg.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/ggaspggqr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/golottdnw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gnggwwryu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gkbbdetue.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gvteahhck.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbehxdzia.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gwdwskikt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gfvwogkzs.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/guozqngjl.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gqlgvfqbo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gzqrkxult.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gfdwkwlvr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gvrvypggi.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gkuualbue.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gkjpvezla.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gzzbyjrsf.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gdjdknale.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gjaasuzsk.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gltusvqje.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gpwsljluy.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gbujngtys.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gtyzqezqj.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gihepavyj.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/guvwtfyki.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gipsybfxt.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/greqokgoi.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gnzfqyprv.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gngxffffw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/gkjjixdgm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gxkfpjwso.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gyihvquud.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gulutkpuj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gylmfxzya.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gposmalbv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gcqozckof.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gorruacfo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gksmrfcfc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gcuuiatiw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/glwrwisoy.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gdlvvcprg.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gokgkjtrs.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gpsayjiiv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gulqyssdu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gkjxlylxp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/goflmkwpx.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gpzwcgskn.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/goddwhkgo.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gujscgnwk.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gipxvfemg.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gxeglceci.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gcpsdftlu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gzvafeole.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gcvyznahg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gpvazpicu.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gzgdzrwqe.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gnlvifknb.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/goitnfdtg.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gljeaakek.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gdumnxrcq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gtabwebcs.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gyrvrkwxp.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/guarkluql.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gqkcrufli.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gvsnfhjho.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gwmfsyllb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gntswyzyv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gwsvffchd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gkndmygwr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gseaahlmz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gieenduvp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gfdlohvny.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gkxneeuzq.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gyzujjnhq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gtnwxiwma.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gbtgzidtj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gfjkoeprj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/glhccbfzx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gtbgceopr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gqoslxdbd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gybwebzdi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gutkkmngl.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gwmchwvot.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghdwdbwsz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gjrhzatee.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gpqmoovli.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/ghlcpkqeq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/glbebmibl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gnqntrdkb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gpgvxzrkl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gwkspdchw.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gswscszre.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gwzcvaheb.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gfsexnswq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/ggixxsnlw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gmlqxozxy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gztayefgu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gutgrkuzz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gktoqhggz.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gwlbhvwbv.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gbwenqcte.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gxconeblb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/giqxfosga.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gzjfxjnis.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/grykpqjzp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/glmieozcl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gvjmhcqnn.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gazctwsen.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gjzgoutrk.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gutmmuloo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/glrofxxhf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/ghxpqgqrg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gfoiqskyr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gxrukhcil.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gcuhuhjzv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gypcxqdkg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gqneuxowp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gvngbkndr.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/grxrmedxg.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gxzoejkay.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gsevzcuwj.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gigbiolub.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/ghlwubzky.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gamiqlbwe.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gdsmjsvsz.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gmjqygrvb.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gznuxtjez.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gogutkqpf.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gpkuhmvev.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/galigsmem.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gibkxlknd.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gygzmmiwo.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/guonfimmj.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gxujtrhwv.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gzlsjdncs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gqsberusc.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gedzkzogm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gzinrkfbi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gqnapkgzc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gvxfsiysp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gxpoilqdc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gqhzszhjk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/goffrnwmh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ggplqgyvm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gjjbmecur.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gzgkobrqt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gbhsilcqp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gnazucrfy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gsmmhxmmq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gqhxwpbqt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gzxcjivfx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gxmcjguig.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gpbpdzxon.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gusavfcio.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmgdepfso.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gdqrrhenz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxibsaipj.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gwstnozaa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gnpgiokfp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gaaycvelq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gkbjwtono.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gzydbbgko.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gkahrnbpq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gaqytbzvh.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmolckgyx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gokajionk.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gbacukkpn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gaynwsynm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gvoflufwo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/glnadqbwd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/giwdaqiez.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gdvuflqds.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gkjoabivs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gphcqyddz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gqorrekem.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gxhltszfe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gfzvsdcwn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gtytgdtfm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gvpirmsdq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gcwwiqzos.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/guluyeagh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gguxhincg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gweqyqowe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gazmjsqzr.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gbdpzvswl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gpokxadyv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gjnymjwlb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gfwchvkov.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gclipniuj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/guizggmel.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gaucrmfbg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gnvtutybh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gcklzbohk.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gzdpiayil.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gwfvosbmj.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gaqcachej.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmnyqbsxu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnboxkvkt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gssupfymg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gdpjyymeq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gipnnoqln.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzoxkcskv.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gotaxilco.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzntajzda.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gdyaiffnr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnyxxcdhn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnijwclhw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gtkfpurfh.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfrlkpbew.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyngctnbf.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gszxqjczz.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gxpwkyjld.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gbidnmhza.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/ghowrpusn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gipxfzwxi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gcsvjgzef.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gdxaeczwj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gsjluaxgi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/grvswwvuq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gylblhchu.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gvhbohxmw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gslelhzcg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/glhrfvwsf.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/guzkevmrd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/goizmcqsn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gviyqixks.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gcxkgkzdo.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gmxwyxphk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gghrxxieh.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/goicujaar.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxbvficrc.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ggeahataf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gyuxkdkyk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gfejklcle.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gwcsiqkhw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/grbnkwmga.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gssrdmkmr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gcdywzoog.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gysikrpxs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gndfrmnnt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/glklppvys.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwtpreodl.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvhdlrmow.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gowrxxwbt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gkuanhhqi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdmsnhkaw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmohqwmmh.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/ggupokdrq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gtaepbyhp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbueryhsk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyhmcgtjx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gdmcutlhe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gbiwpruoc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gewylpmmz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdvdlwizr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gouegdsrn.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gsxhedtje.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gupdwxrup.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gbaytyrgc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gewizxwpe.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gilovcqlo.sHtML


<!-- 参考信息 -->