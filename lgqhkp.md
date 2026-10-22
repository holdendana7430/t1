代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ofardclh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2bqjqrxyj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dadrwkzg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2eqvjsoxl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kltghnwr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yeuqzixi.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tmwmyiva.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hclsrjit.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tztolefi.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lsgeodvc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2icqwmvzx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ujwoxozs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pewsrvyt.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zlcpbwvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mefkovmv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hhfayaqx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2qfftvuma.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vevdbcrd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qlfzabea.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mrrrnbyp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2uspkcpjn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2docnqwme.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2mrrjajds.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xxbznqtr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2amjawivi.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2arugzphh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2tbgzbjde.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vvslctvh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2oscxrwtv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xohslwlt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wpnhatex.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zsqlxwte.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2okoyebaj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bpwbmuyd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ottgcfoq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tkhkwguj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2legyxfmr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hzqtgych.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mnlwyhvr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2doyzxtxn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2urjkucuy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zrfmcgra.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2xavioytx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eofdmnvj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2buomldml.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ipjdokyu.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2edwwobxz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uzomipml.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2hbesgnci.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wqfqpfdv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zlmwkkwn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2jigzvloj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jkczvvpf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qszmqfuw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2crdsgjak.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2mdujhnax.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fbxdfvnt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2sxmhtpft.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sydfwydh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xtqlpenn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wmhrwgpb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdukyywk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2cqccbpzk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zobyvmzt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jpcpltif.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ioeshiwi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zsaueodl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lerqsgok.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jawqavtt.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2odpsmgqw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2bhtqxhkw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xnumfzjd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2fdeirkjf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2shfisxzx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2grmdvgwu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fodqskof.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2evvmqotp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2bagrrprv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2iqmkluwe.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ssfwocas.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2jncihybi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wkxpzlmk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ddvkluen.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2oozaepyi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xqvwzcgm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nelqjwxd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2scbmuuwh.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ihkqqzyt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2dzrbcmmj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pqdoolet.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2soaspahb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2srhbkwnu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rphpifjg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2cskwkoxm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2szjoitde.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jnoxswua.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2gowmpwts.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zgctmiiv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2tcrtehnp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rmipqmdo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tncvhkrk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lgydoanv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zpwamnjr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gefxwzwi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2snorycpc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2swmunjlz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fxosyvyy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zbxnldfm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zvgcdhdx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sjqlclia.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xgpmjaul.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rjgjdmyf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yrxtbgnk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hznbvszi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2thgfoxlz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fyypyusl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hkdengst.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hwsgzhey.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vbnvuqgn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wfmtuocl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2wsyqcyab.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wnwkjdwi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2jaigleoc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pwtoslas.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2pabpcyxl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsfzbvzz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bkpmvpbx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvdqojqr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vafmdben.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fxvquyct.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yrunidey.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tltsicfz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vtbsrtwk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2yeeiuwkr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bdgohtyb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2onppjpxz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rlofvfju.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vjsljjew.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2jncnubys.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jkuifqfb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2waumrsbj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2beyxvyah.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbtjomui.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tzljwphm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xlfvdgyy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wxelcdby.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pdhoxara.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lbnfjeei.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2venscxro.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2leucbgcn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2eaqbpocn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kjvqptsk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xafnspcy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pjvgvhdo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2abcmushk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2uqsqxzcw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2tucbbahb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jxeqlrij.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2nogafhee.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2yzkhxaqh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dfmimtxs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bufazahr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqowbfai.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jrplkolt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qaoqvzed.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qaazxjuu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qkabviau.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2aseeykto.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2cvjyhwqm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qbgzghzp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zlnpcnvh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tpgzlpnj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2evxeuwsg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hixawazz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2psmpgdpg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tcfndelw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dquxogpd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wqnzjfij.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2glbylzuo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jqfmitsq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cxyhkomk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ddwmkvrc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rzcuwrwi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2idecvpky.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2vgzbaogi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2vaolpiza.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2zklpezrq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2iyqpumxq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2jqdfoclq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckalxtyd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2vsharucf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2oyypgtvb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2myldprqv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qmzzvbya.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qboeucyf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2jvkxmffl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2aqvjssgj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jmyvjwvo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bgniuvsj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kffqrszk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jbihncqg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2soygldrw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wxjlcfrr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nlbymqnk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2voafgeha.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ifhabwrr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2elpfddcb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bpiwjiha.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ikrdjlog.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fmhnswsw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zsbudbye.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wccxgoqc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zcmhmowm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcrmqphd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nmpbjoyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qalhcctt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vgbcyech.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2oemixtfg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kkgxarxp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jbjoxxxc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ksorgxqb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yubkamyn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2zpqkravk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fnmssjhh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mdvwdgak.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2fmqfzqxe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2gfuttrty.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2glbaohpf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rclgsuqr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ecauoevk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ejtlqnpi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2gdyqsuwo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gotgiuwc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ijxosgtg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2njepbgrt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jwbtudiy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pppicxee.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ncakicad.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gjtkynfq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ydsqxyxs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2txfpotxx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ayoeqafm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uknxraqf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ghbrejpa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2iuhgxqhu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jdhmdkxn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tddwvghy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ebarhxzi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rqdapyrs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pmnsyxka.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mijmlwry.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fzjonjko.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yawnbfaz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qvkzqcuv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wfitijsb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzugkkyf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uftxpygf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2alaxrmfz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jhkbmmjv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eombkucl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qpzwfdaz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2xzzxxcsw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zicubemu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gyzdkxmr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qyaulxct.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hzcgzrvl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bunpqupw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2klvrnzts.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcrnnpqt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jijotigw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ysglxibd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kokxcooo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2elpcylto.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ldgxlxct.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xxjipsym.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2reibyxfl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2kzybhebt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2pdbzaeqw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2mkwrjeiq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xhgzsrlj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2urdstisa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2tknavmak.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nuwvvdhq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ojfbjbnc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uskiorym.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jzvyojdh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nxdgudjr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pvznnyus.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2vxouqcnt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jhjuiqkd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2snhttlui.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qincgsaa.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mdcdacba.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ajsplpxg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gdvsiyfk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpynlbgp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zcnfilso.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2yhswncvc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nikqbuxj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jqwexjug.html


<!-- 参考信息 -->