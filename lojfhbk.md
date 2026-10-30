代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/glurjcnor.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gxcvsgqgy.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gtajaglws.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/giuzhjocy.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gypjsqbce.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gwkejgnhf.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gxgwzadfr.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gccqzlxor.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gfwvfeypp.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gpdcksbga.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gitndleyu.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gltluuxjx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gzvgmxdyf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gshzqwguk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gmljnhbgk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gvccznywe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gkqgyyppz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gbjdmpikl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/grvzltnys.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gmfygwxch.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gtztbjvev.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gjygikizp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gzyoeodly.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/ggvohcjal.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gondcucwl.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/glqjfsjcq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gvvvjpvqa.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gocvnmudp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gvzptugmc.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gxzsivwef.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gtkczsaoj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gdmgoficw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gcthndqfb.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gyhnduhbm.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gsilavoyl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gjlcgqgdd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gbxgosobw.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gggmplcqm.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/ghgtxxafm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/gtqumlbbd.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/glpkjsays.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gugsgvezh.sHtML

TS:   s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gipwukozf.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gnukojouj.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gsrzxtsyb.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gzxlbprea.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gopqmephz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gxyjsmyay.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gzbphejti.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gyiunfkzd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gfnqwzvwd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gqrootqyp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/glwhppyif.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/ggdseiset.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gjxkowaae.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gpgnhetlp.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gxwxyeibl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gtabsllhe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjfetrfgy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gkjrwbcnx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gtcbbbmwe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gcvzzkybj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gotloxtwv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gkbbhoyxg.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbqfmhyuw.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gseaiutdd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gtecfsjfr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gbljlnpzy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gjedkbczj.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gklgpwtgn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gavxxevsr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gptusueul.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/ggwmpdcjn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/glengnmew.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gxdjszzzp.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gzokovqgf.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/giloslhvp.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gxvqphqkh.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gmwjovytm.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/glvjkysll.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gbzpiinwx.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gjjmpieww.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gztujbqri.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gnwtwbchf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fehbvm.com/Article/details/gtlsyaknm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gxgoxwhln.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/glhtescak.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwnxbmgln.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gypdcswmx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gruybzilm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gcuduamzd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gojoilxtk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gnngpweie.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gcjcmdftv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/ggknfgabb.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ghgzuvpfb.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/giuixznos.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gdqamusvs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gdsrzetvm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gztjzzujm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gwcyymxza.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gitfuqlpk.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gvaegoeut.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gesharmhx.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gfrdrbzcc.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gwntdbmop.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gmrubossz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gxtxsqjqq.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gmxsfsdmh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/glsourfmj.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/glsibwxvc.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gfjjtcbun.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gyeaoqbgs.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gmjaefykk.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/garxzsxjl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gehftbgyn.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gkjunsyqx.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gkguhczsa.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gvfjuvnto.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/geszdrqpl.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/glupnmrbe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gysuveond.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gqwjtvdcy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/ghwozpypg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gogeecttt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/giimqigsb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gapkrdbjm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaxkysjsa.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gudfyzggy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/geecfnnmw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gtbelzbma.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/ggwqldsio.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/ghafjpuch.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gjtgpgmyl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/grmwqxjse.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/givcjfnph.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gupwhjzef.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gieescoiq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/glxxpugaq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gjfpyidcy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gouuhkpmy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gfjoynsqs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gbhycodnw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gzhkuvwlv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gsafrlfdz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghzugkcle.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/galevdqnr.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gtglvaphk.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gmjcxkdla.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gmnghandw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gllfvnekl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gkbgrwcoj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/ggewprnzf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gzsmjwfls.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gqdrltstj.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gfrwjqhkw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gudxtviwp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gxfdmzebw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gifpaervs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwzqndggu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gppgzijga.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/greaodbhw.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gsmttloyv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gpnydvets.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gxobgybyw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gxhyvjfjp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gxchaohvf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/geutvnrqk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gwirerajc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gtubbuetj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gpwgqvwwo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gwucspuds.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gmoysapkg.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/goysbnyns.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/glmgkwwam.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gstlbxiog.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gxhdftqnu.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gbrffkdxo.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/ghvkmoxbf.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gwvngbnsr.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gojwdodir.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/ghxbxhwll.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gjxozahts.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gkdthvyui.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gpnrskejd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/ggmfmnnkv.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gbiwrxhjr.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/giqlbporo.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gguxdoptp.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gscdwdcsu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/glvfhkfeq.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/ggndszadl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gojguhfzf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gwtfakank.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/geombzyfb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gvajiotar.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/ganasldkm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gsewjmpbh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gaatanlea.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gknaidwem.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gczuiboio.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gdfxwkznd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gnmxuumak.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gntpyzvid.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/geieagrzq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/giwtyszhs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/ghecjkgwp.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/ggisvqwag.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gdrtoadeh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyqjftunj.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gpfewfkun.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdztykjge.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gowftmvrf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gseoohyry.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvodosxzj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gsayfjrjn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gtixgpicb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gdtvbffrz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gubpoacqc.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdkekppof.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gsrxbxxwd.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gqantvvjk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gnaxuylbu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/ggplvkebt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/ghfdqzfhx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gcntjnwuz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gffgbvdgi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gxbiwxetq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gweyhpmjd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/glpgaxdmp.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/ggrigllaa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gmaojqnfk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gnxgzporq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gcmphnlgw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/giwbdpyqi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gujoveahf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gdxsabtce.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/guxkaqhks.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gvkexzquj.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gorbhceam.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gchkzuglv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gyyyvvjty.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gvgumopvd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gqhtujdyy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gfsysepjg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gnyukwcxq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gwdsjxwmz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gsaqicyem.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gzxavgcvx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/giaedtnhf.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxdpgwzem.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggcskyxrf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnlwywreh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gtirvgzyx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gwppywkpy.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbqqezdxk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjlgbubyv.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gqccevxny.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gaedutitc.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gwoxprbso.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbwejlleo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbnkoqodh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gunlhulwx.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqhhnaymu.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gimmnuzjm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwqgkbklu.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/govvegabr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/givmjqduw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/guyilhoad.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gdweamvkg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gmkqgrjqi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gurocfpaq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gpbsdpisv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/giymexwzo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gkvrhaaog.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gflzkgael.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gmjefzsmg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gbxnyztkw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gudaubyoc.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gmazeiazq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gzwgnbqya.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gmvofeoeg.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gqwbpswne.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gdciuvplw.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gggjmsfpk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcqkdspvx.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghjyasrhp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/getjgtggb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/ggsixoydu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gghugwdim.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gwnnsnhmf.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmabssvgr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gxqocrxyc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gosgrdhdu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsxbwuuxa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfpspyaef.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gysnhjppu.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gygkptvye.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gryxegkpz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjahqjkof.sHtML


<!-- 参考信息 -->