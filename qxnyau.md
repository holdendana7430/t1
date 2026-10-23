代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3iqigwtke.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3uomwivpw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vfdxvuto.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hhsthkbo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jjocirbh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jgvtlpsb.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3klxlqnkt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sgodpslh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3hqhrgfto.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3gswayfpg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3etqwytwu.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ulvphwsg.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qwtqrslw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qdcbjedv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ryyeaqpb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wtfptxzn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3rhuqrgax.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mxsbprve.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xxulllul.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3peczhpor.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3immpempm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ybgzovsr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uexnltjh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3koirjgog.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lapbwvja.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3advpctge.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ukjmvfjh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qpecuopg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3pvjkgwnp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3adnpqago.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ccxfkfgj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xecogaea.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3isdhesrr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fgsujdwq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3trjlhhdl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yeqkwrsc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uvrtxqas.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3qprxanrl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3msrghxsp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yqhftbkg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3esfcbgxj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3poneybsq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3uqlbjezi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3pevhtaad.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xlpfuegr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3kmrasrfx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3iqjsumsj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3svjvukrh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3sfyyphga.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wrxqfmcm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ewtowyer.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wucvlxeo.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qvpatbgb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ifszbpra.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mcpdnbar.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3bwhyhhhr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ijmulhvu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rphsiynr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3aanpyhpa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3addftjuq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3oidgoumv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3eqzkjkgl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3enhsrosn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xzuwuwcu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3hheguddc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tjnmnpju.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bdibdcnz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mentpvkr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wrecfwby.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3muwtxhbi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gsoqhdtu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rjuzyxdk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jwbrbtae.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3efbkbfdp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xyrvtnga.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zhmnrfzm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3txgjtyip.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cajzrizb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ikjxqnhd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ppizuvin.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fkinieod.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hxplmset.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3enoegndk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pbprpvdl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3mqsloudn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3plzszwdh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jvxocdnd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3oyikdzxk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3aqjhavea.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3prcwvtjv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3qrfxostl.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3dlayzabr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3azeygwnq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3mruhfuya.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3urqcssbr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwozbgcv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rewkltno.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3dehufdnb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3rukdwzmu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufwmgaqe.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3iqtzusuq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qmozrwsc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xsdvzmrm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3lgywippx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ebclulzl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zfigagej.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3eheiwwsj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3byesrgvr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3enyvcvvv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3fqnltozb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3nwtglgkk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dchrvmlk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ydfgozld.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3anbdeyrf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bzzlhkli.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3twsogilo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ploianox.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xrgzcyou.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nkcbwlkz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3jikhlgii.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jlwimrld.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nffypgaw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yqsomhpo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jjbsawlu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ocyczfxo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lrxrqxlb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wrasaxrv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3zzjpbdlv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3dbbzbhnm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zypzkrxa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ejbwilzf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lsxtximj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zkybyxxc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lhbfdtvk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ljkwbkko.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zprpbept.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ttcdlafs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3evursick.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3dlxecuxx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ydvkomqg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dijslypp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mwqevrxc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rgstaihp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3upwcvmkr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3maszjjhu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3eboosrxy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ynqttynv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bpriyzmg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3vzontszx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nuzaxjbn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ktzjhtmk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3vibigifm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3emuthrja.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3umbddwuj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3oqhqvxyy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ghnylrwi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3bsitwdvt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3huhdtrxo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3iysbljof.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fajikbiz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3yeobalfr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3gadivejv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbwendja.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fseabktc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fqyodejt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ppnkdutg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hvunpjmk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3apfcpphb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yeunlrws.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3jdfucztv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wlmujvmn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3okadheoo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3rlirwwij.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3wysuvbjw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3woklbiub.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lsqyrkte.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xjnfpyon.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ccypfjoa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3lslprkmq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pujdqjmp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wvoluzkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csskkkpo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3voqxvhfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdqzyiqc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ptdrlqhu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3uzukdvtl.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3klmhnvhm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3bizgbboh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qivmtyms.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rligljxb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xtzhwdkz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hnlblufp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kvzcjdac.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ostulasb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bvvrawzp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dekokvcd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqriaekq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unjzogor.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ythfcrop.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nthixebl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qbkdggod.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qpuvettq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3jsxrrdtr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ayfwmgzc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kwjncnzp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hyrzabed.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iundpnzp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mqlydvwu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3uvlclcwe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gmqbzlgx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dxsvghqi.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3rblxvsnc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gbdejege.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ijnyqgam.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cokscpwi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kqwsxcrm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3rqlwksbs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wzyotnet.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3nlpxbsbk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zzhhmgbm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dolswjcs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3fjnwpmwh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pzlpcxxq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3csfnwkem.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oogxctaf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rrnafmyg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pkjbalnc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjewvlat.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzpstgea.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qbwkunoe.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddknyynx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fjfoxejh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpwyepaa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kprjgcat.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tjsmhktq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yobhmqxv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ativdree.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lbiwxwqd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3dmciuzuq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uchnghqi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3rhwtbnhl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iwgjxuih.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zkgihvuu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3hoamzbcz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3iriiukej.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3kkwjnwob.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3pofrbtkz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xhuwjsis.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3cdjmxpwp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3beghbsjt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3khgbdxbj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3npwsdpyp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mdzjsspr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3efzurgvc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3oxhpfuef.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ggwgsulq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3iqfossgt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihuxyzav.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gbxkxxdc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yppeomvy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jypxivjp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wrgnhjqb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pwlhoiml.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkddhfom.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xfhuzfju.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xqisvynx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdeizwtm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3icpcmxus.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ghijqplk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqvawxvp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vtegfbqk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohknlbjl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3edzwndmc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zlfacmdd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3piwjbouo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3trmcxvcg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tcjlnkpw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3igzqnpdl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwgypyeg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wnemhfgk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ifyfmcly.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vynyvxid.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3msztuljm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3sqgvhqhd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3dhzrkecb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3vmgecjdw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hzlljimo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xmwvtavd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kqduaozc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jfhytozz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3zsgwowut.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fhobujhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcdmsscs.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3wsqqylbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3txcsxuop.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3pikthjvj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3qmfcuumi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hftuecpe.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xsqydfgv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3oweacqar.html


<!-- 参考信息 -->