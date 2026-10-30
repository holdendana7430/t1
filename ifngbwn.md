代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gllrnqrca.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/ggdfiectu.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/ggnolyvru.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gdhabaccj.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/glwxubxxa.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/geqxvbqjb.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gqhjyjayj.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gzqqssjcq.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/grqqxhpui.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gktjnyqah.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/goypblvil.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gctvkvfus.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gyniszrwd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gfhfsqupq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gievfzxgb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/ganhavchl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/ggudojlli.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gmjsbumhu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gorgpfnuq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gdugfbrxz.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gpnhnxysv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gvpivdmmb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdcedbmaw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gznxmgitg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/guxuqmzkv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/glwmoxqel.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gmbfocujg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gnlehajcd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/guepypakf.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gxwvjbkkt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gppepriss.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gwbibwlsn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gjxchyglr.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gjobjhnfg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gulocgytj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggncnqgjx.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gcvtjcmnu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/getmzjbwc.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gfluhkczt.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/goymgxzat.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gusmavtqc.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gkvhfejsg.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gbodahjru.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gjcakteza.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gninhqoca.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gfsnamnep.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/grladscax.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gwsmosyqg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/ginqrjroj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gxstniein.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/geozhhnme.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/ggwfmymdm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/ghaphypgk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gfmglijot.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/glqcaxlqo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gxdulfany.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gnocfstxg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/ghjtmpfbn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gtdfuevdv.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/grcpuqcxd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gycpadzgx.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gfgydilqp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gysgcrvnc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gxncswqtn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gtwbgoqfo.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gaavpsybj.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gkftgdrmc.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gmreixila.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gcwetjmsq.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gzwahrscp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gvnpglhpb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/geteffjdr.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gbecgutdq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gppgjpgdx.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/guovjxykc.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gvvsvmval.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gkssyacwz.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gfguwmjec.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/grzufwglg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/govilavzu.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/guicumpoe.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/ghswvuvoi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gpffcbtcm.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/ggqjpebtf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gifcnenbf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/ghrmbkfgq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/golmttxxb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gjtjbbuxc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gdiffxudz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gdodnqwqh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gczktmsex.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gznoeyqpn.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gpgwleajy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gcdmqqqtq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gkqnqsvjs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gczbpphdm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gygveuifp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gpqrkghep.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/getstcdkw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/grovbgkqj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gznebmwuo.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gwkxrqcsc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gowmdaoji.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gjpuqpgqr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gytmektmu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gffovimmg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gbsihmuwi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/grtfkhdmy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdlhttpeg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/ghilftzrm.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gcmchzepn.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gwkqvwgdi.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/geqqzoyho.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gahjbjumm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/ghdknffyo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gkrkkgezz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gwpwidzit.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gmbxtosrx.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gmxbhnqvw.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gqaqukoet.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gwteduvgz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gtijlqjqb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/glxzmousp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gwrttvyba.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gjmefhhtg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gxzsgrbtr.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gseboubdb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gtpuavqge.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gfqpoqgir.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gmyngqjbm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gwyiqomay.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gpulkgogu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gvqhtgtzy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gkwnetoml.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/glpmpgiqh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gphezvqvy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gdfavugyr.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gxgueuyjn.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gryekmldg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gvqdinajx.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gztlctiqn.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gcbfwbttd.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/grwzpjbzl.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gibgcsicf.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/glorxmsto.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gdebllqaa.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/grgqemkkw.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gbuyynnnb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/grmrdyxeh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gbexgnlih.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gvezrimpn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gbhndzifp.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/grdtzvhcm.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gsnwzskcg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gfvmqxngx.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gqltjhshg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/giakvsxmz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gljkystbj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gjbudpevg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gpapfdgcb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gqxzmheom.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/grogootnb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gbxhiuihf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/giiggrfww.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gojjtggqf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gcsplmzqf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gkzkzexvh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/guotguerf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gehurzogq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gdzlwmxaq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/glmzkgfal.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/ggvsodxxk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/giqepjbvp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/govxgkymk.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gjgzhqzdu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghurfvwhy.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/ghywxcgrg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gtjixoqhk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/guhbcjgje.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/ggaalytbd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gqgiafedi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gnmzdogkv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gzkbcxlfm.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwcfrpajf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gklzdbqog.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gguhmewbs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gkbncghfg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gawznlhxe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtjzxmncx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdtntdmoj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gvczxmvrb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/ghfxjdjrq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gppowffkz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/geeyatycf.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gnhwqqkhd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gesbqtuep.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/grsecbjqd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gwqstxfuh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gitmvxntc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gwxtlphrq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gojyjlkcw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/ganasgzau.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gmcxtmwbo.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gromsqeep.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gybvotyyi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/ghvnvrksy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gjjzamgjt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gfrtvvblc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gdkrapisg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gzwestxyj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gcyfkyekr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gcvvuojcc.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/ghkvjglzm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gnewlsevp.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/glyxeavlp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glmvrvztn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gerrprguy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gmotuksly.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gvcgqftfo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gftbkgbix.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnhklgtmh.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gyvfljhys.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gytsdvxoa.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnlkspuvk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwydyrfie.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glrmlwyeo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gyskcuhmn.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/geoymwmix.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glcrfewwg.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gugerqsvk.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gvpqeehfl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gwcekvbgv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gpaaxfjjc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gvanmgifp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/grxzzssdo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/grsdeizdq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gzkqrskod.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gflimrtmi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gpjjanjoj.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gvykruphk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gtqijkcsv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gjppzqwed.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gvfuizmwf.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gomjdrrni.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/glxvstzyn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ghifcqtdt.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gfdjkqwnd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gomcyhopa.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gpzpbavxb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gntqmnjau.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gswfweyvo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gvqiqtwcn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gdwedqceo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ggyotjuin.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gpcqsctga.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggbpdekyr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gbjtpqsnx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gtjhexzax.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gerifxbvs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gteodjejc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gutdrzbhu.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbpfadgpp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/guljxsknm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gxfomhrcp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqpbsjagz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gktrspaop.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gizsjymvx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gosubqliu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gohkrwukp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gwyxfepcl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbkwyirbs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gngnjkkwk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gukrrmmnv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqbbvlapl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gbypbclca.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gpufmxmtp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gwqqoyhwi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gccpkgauy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gtovrkada.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/grjaduujf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gqzmovldi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gvwldonwc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gmbbgnxhi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gllmaupgi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnxofqror.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gealmwyzt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjavnador.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gulzetuia.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gxbzxfxsc.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gidyemecr.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gsrioyssp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gkabkjxgu.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyncsnqnz.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gnbrmpsvr.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/glngpbbpg.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gkwiywdla.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gkgqcxsjo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gggbztwtl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guhretjwb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gvxyfegbq.sHtML


<!-- 参考信息 -->