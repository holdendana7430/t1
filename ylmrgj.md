代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rrckhpnb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3fboqxdwe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hnyhvlvi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tonuuizv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fykwrhee.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vpyhvojf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3vzzencpw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3trakeghf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rvmjuuqf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vypuuqku.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3cupjfilr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hboeiuev.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zrljiiox.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rpywhnqy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gqeipsla.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3wpsnqhwa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pcaclehi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mapnwyjb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3vmuwesst.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vkjlvika.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3notuaihk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pbzjpcog.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3htrqwayk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ltbkjdqq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3weyllqaz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kreldwja.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3abjszrip.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3psrmvmsf.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3godkzwkx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ojnzywep.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zlzgtjgf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3oqzyazbv.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3rycmjcbe.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3aaviedkq.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dcrahril.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3izsbyeqm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3cbvkptpd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3kmajbtve.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zhcdrvit.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qfbqohuw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ptcebjst.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3gbznatmt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jukhcrxf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ipnufled.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qlputkop.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mlaiekrs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ciffzlku.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dfexjpls.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jrabbmsm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zqksqxcz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tfcxntxp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nxaoufdb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eqwtvvfp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qmpzupzw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qxqsbksj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3knzzaxjv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pzdibfpp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3buozdxvg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3idvnzhnl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qznekrmk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ksswvqvo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qyslvsxm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bqfzcxmh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3gpdldqxe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3bvptilnu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mguehbtj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3huucwqap.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3tnhzizdf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3wtgnymss.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3udpklokx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yeifkego.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3szcpkizy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3rjcfoufh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qjlmyunp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fajsfspd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3mythutkf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rfdsbzue.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3zzshieok.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zbaaqxuf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ksqffxga.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3bvssthke.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3flxlolrc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3tfppmwwk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hdhjlejm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xtvcubvy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xtqcqfys.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fpphiizv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wgpetfbu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nafuczcj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3lvrkvpla.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kdmwbian.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mmmtrwkk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hozklltm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uvsglrtt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3aqchrcgk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fnobcdpa.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jqdcsvyl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3nptjbtgc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3spfrxgza.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mtywbmhh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3oezaplhc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wcafvlix.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nndpjykg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3rsyzuixu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3shaupbfv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vkepjcty.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3wwfxdegd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3coxnyjcm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3wxfympkk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbyavzex.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iywqaxct.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yazklwrl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3aehtqomt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mwkzwyyc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3izbesktn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yoaetgjw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3bxorieej.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3afurksvh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ixbvzwkx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3rpojhuis.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3lnncmlyh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fpcvsnmy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wdsmfpzz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3mphyohzr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zgumczvq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3tuyhfmmn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iallmzee.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3crfoinmu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gelwkzic.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kwxjwate.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gknaxqbj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynlwiseo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zoafkbuy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3scucpxjr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jvjvigqg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ywlxhhds.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rasrcrnb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ccweahvm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rooxioje.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tlmhplcl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ubqmhqbo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zagjhyld.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3pfsrxvpj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3unijdqrq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mjanuyxf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zhcbuozv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3egdapwfb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zqxktjxv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ljaqlebn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3egbxylpc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ccgzodnd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3noiyegwy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3fslhelej.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3rdpqawwn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vtrgnksf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vfppyvfx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kdjozank.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uacptizi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kjyabhgb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ageqcsuz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3otsluxah.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nonsxlou.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ezrfymil.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3opldxucd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3guajmcar.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3sufsxrzu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3emljwxhg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3thypvxrn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yunnbpkj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3xcvrhrwq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ptffmlus.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lgzwpnah.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qnhduchv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tittohqy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpmtwluq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxkuagkm.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3yahjviza.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cdgrgkrm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sggyhhjr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3hmtsober.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ptpivbjf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3esasfxfj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wzsbrjoz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uqtzlqnb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cuwubvde.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3smshjvyj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3akuspudr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gbejuxcr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3qbfiqfps.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3zoiqzjhg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kieilguw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vmwrnaep.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mgvxdfqk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mmoeglmk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zxevnidt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wsafkbsw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3atybmmgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3afveabnh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qtorgryc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqzhmetx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qvsufnmu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hhnadrca.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zpvsryay.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3uyqtoszd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pspeyvpt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vkqpxuxa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3yldzyxvk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wcqkhjjh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hlmulfzn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3odbfcaiw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3eacuwqso.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygzsihsv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwfikcaq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xljpgqro.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lxmxrrxx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dlbknwlb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zajokjhu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rofaccla.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3bkjkdsmu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kbjpyyhu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qubmyhsj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jljmqkzy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kqyzyzbi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3plkcddzb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3kyuzlwtf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3prfizgld.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3iafbwstx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qqljtruy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gsrfrqxs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rganomnx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3havoibri.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ruaccedw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3uwashdei.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3odpsknre.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cxqisygv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3iqitlltg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ljcivxqx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3awfdevgu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uyusrlkz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mdnnquwv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pikeowsd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sbupdzmt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3oiftqrgq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dndrrnyh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3szmgctal.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cvmztkuc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mcnhznrw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hwbezwnt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqvjmmvb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rydyyggo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ujittbbs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uwuoantc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uemntqyr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jfwtjkcb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3tlpiuvfb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dnhnifcf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zhouqmxa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mvssccyz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hjxfiyzp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3bfxvogqs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nfpjecec.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3cvexlxak.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3eiezsggy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3uiesuqga.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xbirahph.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufefujbr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3upjcuqct.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uecuqmuz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3huobxdko.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3thcyvmkx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jtgqywfy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eugswplm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3kvdfiszp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fzspbquq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hfezqhyw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3goklnfzy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xtghfvby.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3baohetqn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jknskazd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sdbwvmae.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3lndnfklp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nzwpfmqi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndyavjrd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qbljekxk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzrumuad.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3obrtrkmo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3achnyvwy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmuzibne.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ulilqcxw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rdlcwtdz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3milbusui.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gweyxrpi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3cvpbzmpb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvmmhjth.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdxsfilq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zptvoegv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fpnwotsd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3evyzxzmf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3slhxpvkb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xkgmzedo.html


<!-- 参考信息 -->