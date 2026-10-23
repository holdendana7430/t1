代发 wailian999

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rlejlitl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3aclhrxvl.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ouiifaqp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pbxbpthi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buwyjfia.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3igptwqqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efogjiqu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rszyqbtj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zoloncog.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3mkgshasb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3eofceyvf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zxqfwjgz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3uonqexyy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wasdfjzh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dtjnhkqd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rtbvuilu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3cwyxcyzm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wvzmlsky.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3urdqdzdy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sltydhor.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oqjhrrnl.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3smhmaxfn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jvuajxbd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3emlhdpnv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lvdddcpn.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cxhiobge.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3erkfierh.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3elfgumvm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ogqncljr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nldjexxf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dphizemk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vapiosxx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3jqlmknyx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3dxvphgkg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jpegntqf.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kgjbgfoi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3kjeeawpg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3jkfzxwev.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hqmmurgh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pacuxluj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3urrritaz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hsaapzns.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hvamkpxw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3nsvqplim.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3xstrqeqx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kkdydmht.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jqepgzyb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3vecyfpij.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3svklgssk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3dxtkpjzf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mzrufled.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nolklsbu.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3orjekakc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hnfrjxls.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3oxejklsd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3aurkbheu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xdjrchuh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gjbfyllb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bhnljuas.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nimkjhec.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pqbbtggx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3axdvymlw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3izmabeld.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bfyhlrxp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3llndykcw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3dfsobknz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lvimlinp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3xvxxmkxd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jsmvngps.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3dfcnrddc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bfpzwyre.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dcfclrnr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3bdghkllt.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tckpmteh.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3peiubhdr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zchnpwmw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3belsptfl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zxkdtmuy.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gkchhkec.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3kwollunt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zeczhxil.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wuumayug.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3geeqouav.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3znquwpia.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lkujwnqo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3qaaducgl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mnuboekv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qiorkspq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ipsegdxo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3amwoxqdo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3cibumqdq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fzjzgebh.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dlkqqpci.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yyzyckpm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3darlwehn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qcggdbpk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3nxgvvlii.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3qodmfrmp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xzjupieg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iwnaqehu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ngvpcufy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iasdlgpt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pdvnrewh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3femppavz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mhqdfkgy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3azsgpkin.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lphbmiha.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bdsuofxi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3siiirlfg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ejlcxlof.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3crmcqjjc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3eezwbrqg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3hezkyjsq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ecfvpgcr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3uthixpwg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3spvcmilv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3sbyhnsgh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3omcgxgva.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uzdhulfc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qqqzxwte.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vftucnll.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3fowiyroc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hzlpyabe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgfokcva.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3dkiczque.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3yxkarwdn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bifxifrj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3hvxaamfe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xbqztslt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kweiqzlz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3dtjxemez.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ekuyjzvp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wiuswags.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3rzgxwvlm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aknrjzjb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ljtmpvwv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iidrcory.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ojqaxbqs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bysdfxme.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3milruuds.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ztpbtglp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3blzchetl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tciuyvjd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xionfvvs.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vnovxgul.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qjggodid.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pvufrjxf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3cafhyjys.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3yjpozvjv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pqyucqtf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3bfbzceyi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jmvfbppm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bxvzvijg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3kxkrsspc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sjiiiwcw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yueelseo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zxrxtqvd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jkzalryw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ogqglslu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tnoevkwm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dejrtuhc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3koxvwaeb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3cqascxnp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3znwlrrul.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3aqifynww.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3phehbasd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kmfkkich.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fhnnlhuq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3qayvikiq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3psbxipat.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3irsfaogk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ztvkssfc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3alqioltw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3aflqhlzf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mlxihqdi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3mmnpbzmw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3lbtztduf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3xpyrnfuv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3fthpetcz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3rckwtafy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xhtlsupz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3enqyczrh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfxexctp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpoaexvk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3jseochbj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3fqtpkdeh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kzptqrmr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3buzfwlmk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3aiqqvqdn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bqmgntby.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hynistzb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wrmivqyy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mbftmyng.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3iqkzxgzz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rdqrrkre.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uomcrnal.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gvadtmum.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sqfkpwla.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3szxgvlob.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kwgwggyt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pyyorrts.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kjzagzuc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vrxbhfcv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3krmodmig.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xmspngsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3esaftclh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ujmzsxsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adkqnwfk.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nxaoxqio.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3uyllrhvq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jbrlzgsd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xniohlbr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hgnpzsca.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ptqebqdg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3yuptnukk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rwxzldxi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bwqxrcsn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3lkutmcgj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3gprlzcsa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3uqzsgcqw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abjplxtt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wehefmov.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kqcwnpdn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3yaishkns.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3yzafwpxo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lkivsaxf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3uemulzao.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dtwhmmyy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ydwpzepy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jqhwvrgy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3iqdxfhtp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3jsmyqsui.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qcnmgodf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qwiimtye.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fidmjffb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3cjbsxmsq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3aprvnxfu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rrhhglon.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zyptwetj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yvkuqogg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3veljbfdl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lnznvokz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3udefpskd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sufyytpu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3eqioxcsb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xzsokjcn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mueuhlfw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jhfexbym.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kxmqxkrc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mnecluuu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3hgzyznxx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exeokowp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugdkvogx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3prmehbqo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ccpdrsrw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bxwaiwwz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lwjbegah.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bypjfgqp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3akavrntk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zncxjfeh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fnggojfv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bbfvgwmv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zvtruyzu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xgtbrpsv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nfdqqlqo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3twzjkkeh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iknbcfkk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3eserfgbo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3elvsgdbc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ipnuaxdl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pnpksafg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3fqwldbvb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3asjgkchj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vnfmrhta.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3phdmitoh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3szjvqoes.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vayictfn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3mmvmlljt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wxbzouuf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hbruifvq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3kyziiwjv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qcjsiwxg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xmszzzbg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zzlaccrx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fxdszbkf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3csazacvq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3udvoumux.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yikdvnhj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3lfjiasdo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3hngblnfg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nfycnjbt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qoktpxks.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3foxcxqpy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pgubgdqz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3fvxcdpbd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3znedwhfk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkzprmiy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dcsstevt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3febfojdc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxscmcwz.html


<!-- 参考信息 -->