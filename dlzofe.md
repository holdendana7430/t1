代发 wailian999

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vsewecbm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2dhslewfv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hmofhldc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zipctohn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2alwjuhuj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2reahrvrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gygjqylt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vawpkdlm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2jfkpebld.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wvnaxyli.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2egeidgov.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gvxanohf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jnxkkaxh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lnjtfcvr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2dfpzhefm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2phqjgczc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2lswjkeyk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cviotsop.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2xyyrngzy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ghfxumeu.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ejfrciaf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uvarugys.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rjapftie.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gvulagea.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fqiceifv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lxahilgw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mhatynis.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2smazczxh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tfasekzg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2exogaogl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2eniwrhmr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rlqmxzgm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2crcskxbe.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jvwcrcsb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2bgzeysss.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kxejrnww.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2siipnnhb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xdgmsxtd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gvycpskc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ejlrcaxh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2pfvoesgc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bievhgai.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aigariec.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2caxopfhh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iuljnmys.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2rpnmrsjd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2csmqicpz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2awvespqd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zrovflxw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wyskrbyc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2nspejqry.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rbalakhp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2grhkvyvp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ctuaouci.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2fhopbsxh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2haocvkyn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2egmquupv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fbqjdpww.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2gckiixxm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pyvywmyo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ysqcwgpl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2izbuhsmp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2icahsobb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xyykovxw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tdelkwkh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sucfutsx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2cqylrzhf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2goqxhxrq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2rgalhccw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2efcjsfvs.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2bkjqfemi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ssiiukpm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2famtkhgp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wnlnanlu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qozufjlz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2denlkgen.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zfesamhf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hkycajtz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2selnygoc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2gxmndyup.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmangntd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2cwqckesv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2agwqzrlo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qbzxmpla.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2pbyluqkb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ifhhefxl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qwvvzgua.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fkvhyywu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2pejrhkch.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jsyittfe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bqdtzhqy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vjcvmapq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kxswuxky.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eraowasu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bnwbklru.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lzbkqrgy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2fxebephs.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wwjkwchc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ingeeplt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2qpnitdib.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bbupvymw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bdvxfeuh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2xttkkpwf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2oaekotgx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2yrcjuzxo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tefzizph.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2cskufbis.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2eggbxxmp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ncaefryl.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2imcmpaeo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hhildyjb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jsesvgbo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2qanlazon.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2aglxpgie.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2grgjhzbp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2finoqyci.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cyelxzxq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tparjlcl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ebxqgyux.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2napchesd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2owizsubq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fdbmwoat.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2exxbjfvz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2badqjvez.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2nyzxfdug.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zkgmcfsw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2whyoeyas.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2uofpaupf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjfqcyvv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2giwqdqzh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ptyrymlt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2yfpzokrf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jvdxwbmt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2flvtmcmo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lsjqnnkr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mkcjirsb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ogqdyiej.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2mrfnwiqb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2cepencwy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxenuyif.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ptkzoagi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xymywamf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2huxxvuax.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ftemagsd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2bkptbeuc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zpiskupj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xcmwnvdq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fmwyydzr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2getlrrer.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2herexrbv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2bhmezxje.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2suzdhcwa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qmixzhqk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ezlpqsfg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vubadajp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xomwsjnu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mnjrpcwd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2kaudfgfu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qnyjbeub.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2buzuarmk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mclhiwzw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gxxvxtdy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2iccwgdaq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qimbzsij.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tohedfls.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gvoizwxg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2srifkdqn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2udbrrfli.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2yyqwbkmd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vhigaiam.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2widghwkq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wwwbkowv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ciiuaxkm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qpdlwkdo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2earjqdgx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sqynmkfk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2igxrnihr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2glgfwqkf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jhyocvus.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rpilohiu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jrdgmflv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jclcehzq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mpbsjzud.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2sgzusicq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2nwxubrlp.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dypvszhw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2deiqjqza.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zpssbhzu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gauuymnl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lfhqdgnx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uunucchn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zktsgbsk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hzaenavw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2kmrmfade.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ukegdtba.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vnwazmzh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2vtnezegj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xxdnedck.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2prkxayyz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oajmnyxx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2henucega.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nmnisfac.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2uloxebho.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hifscwgi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2socwosrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zaqvqutx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ncptgknj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvhcqhto.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fukhlomt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rwurhpud.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iiizooxu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2kksheiof.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lydlabmu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gyshlhpq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2sdvzupoo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iimyeour.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2esynuvte.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qwialpnc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xdldimmj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2scggfpoi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nntxqwwi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wmuwzjua.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2upxwhiia.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lrdgeofp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jajprdhn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2aqrjynvx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2vtyhufib.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dvruhymk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sttfvktz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qhrxyfpn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jkxumbug.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2aacfihjw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rcvynxwy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2quqqctod.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mnjsegvz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2yvtfrssj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ljkizsat.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2anwmhqzy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2slmkpoml.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jabeaodm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2okwdxekz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2reliehjc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2mhnbcpde.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gsmoinlh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2tjkfxinb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wksjhqjq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iyaybnry.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oinpopqo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uscaizuu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rsgnuydy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wgiovksu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ssctvaji.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fwybxwtr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ilsqxciv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2usihyrak.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mgpytlqh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lpkxkvps.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qgqqbnee.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xbxisypd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sjdhvmpl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nsqacfxe.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wzaywtpi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kecnqcyd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ieeraufk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2okmlcgpf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xennmssb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nihxckqb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2rqnkujlj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2pnuvhmuj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ztnzndya.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vhzsfiuo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2gmddowgt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wducaulv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2jtvgsirx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2csccuyzy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hsqxykrl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wgmfcgsh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2eojawfce.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2wtfhplkz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2cjpjwosb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gioyjhjx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppslrptc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kjoaadnr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2feymnmok.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fgfovoer.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jmpzcdfv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2imibffwz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwopqdpj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ucquyjhl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2whbjjbww.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jynbfehr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vcpkuxei.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzcwocui.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fhptkpnj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2csbkngbe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qquyplmk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wxodcglp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqgctuiv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2efqgirrv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2itbsbnan.html


<!-- 参考信息 -->