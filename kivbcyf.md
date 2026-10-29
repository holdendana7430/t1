代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gcfdlsfjq.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gturshuza.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gwngzafrr.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gxqhrychl.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gfhjmhsdb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fehbvm.com/Article/details/gaawxxcmr.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/geeuznprt.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gncinajsr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtftvfbnq.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gkpdfcxck.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxphkjwkb.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gctyhkpjw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gaovtawto.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gdoxavypl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gvcvtblpg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gpcdeuvcj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/giddzpwnu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gvcmcbkjh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/ghtuodbaq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gxjdukxhk.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gezvuwchx.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gamsiniuu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/ghoapgpnt.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gyjzcqxpp.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/giumdskbx.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gfsgpqrdr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gyatlxlpv.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gkrhpuwng.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/gedwmcvhm.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gyhjbenon.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gfzvubbdq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/grvyjgnmd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gulpqmlnx.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnflisbpt.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gccfnyrsj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gevjcpwul.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/geriqujmj.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gdhojbpxn.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/ghjdgpnsm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/goryibcur.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/guzpptzrw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gtkcvyjvb.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ghlqnqlge.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gudgmfiym.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/ghxihbcnu.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gsqdityhl.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gzrhovuox.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gtzrrkedw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gbmbykovz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gusyiqdgi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/ghhaiqrkw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gghnsnhrx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gyysgejmx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/giqoawagx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/gqzjftouu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gjdfhyqvn.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gegankfro.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gnjirjplq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gfhlwkcuz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gztfrjjrh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ggjrqgqtw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/guekyprla.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gwrycaegd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gcdpoalro.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvbygurml.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gloceujrw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gdgcydcfy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/ginbmodqw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gyaqolupg.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gthpphizo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gnkjzmoao.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gfuqoprwd.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/grfbsttmn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gtkplmxuc.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/giffddfxp.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gxiocsqny.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gruebngwa.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/guqktfgja.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gqbbtkmmw.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gpkniexve.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gqalmvrtr.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gdpjyeihf.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/goldcrnaq.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gzuukfrhm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gmbyothzj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gulxoprnq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gtdehmnxc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gtnijhjbr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gstwcrjwf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/ghmuljlpx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gitcnbzax.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/ggtkalquk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gwhvibcqy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gznvjlhob.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gfkeipdta.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gdehzwhpb.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gtfairvze.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gaoweqsim.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gomwaysdb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gwvjadudg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gacvzsehw.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gxrxjzciu.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gcpcwzuey.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gjkwlcmql.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ggxvzbknr.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gdxenikfd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gxwujbydb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/giwxjkoke.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gfgbmozio.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gjihzvcna.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gxghddlrm.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gapapfssx.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gwzrvehyy.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gferqyhcl.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/ggxomwnou.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/ggibesvki.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gnmouixkw.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gofwknznp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/ggnuvdevu.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gljjcfldl.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gzurjwtmj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gxpjreczl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gpbaihkzc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/ghipghhvr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkiydkwif.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/goqjrvavs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gksojaxjy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gwzfrnerg.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gqjzhdbrm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/ggqsyowxf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gnhquabxw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gunvhlvju.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gykznudyk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gtfntwsgt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/glkzxisdi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gawuezswo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gawntciey.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gsfyxqoro.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gqjabyidg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gatqoxuvx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gfastxhyr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gvoxuddgy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gdbkftslt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/grofinaca.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gpoccacvi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/glziwlbdc.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gsbwuifdq.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gfurfmeam.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gxwgjpqww.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gbfcxiiyf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gvrcnwjpa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gxouisxww.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/girvjtlai.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gigqoaouk.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gjayujzoz.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gcijandag.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gbiapkokt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gtiopxlqt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gigmcuirp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gsfknarro.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gncwgmcia.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gjmiezhbo.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gejyymtug.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gvjokgcbd.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gcwheurlb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/ggvwrfjqr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gofqhgmwe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/glkuollvo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gkbuszual.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/ggheqhcxa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gtsoxpisy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gwgvqgonq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gkcvekjnn.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gsrrzered.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/ghxhulbkv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gzflopmeb.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gkyyqeahj.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gxzyglznv.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/goblggpni.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/grbzxvizb.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gffdsmjke.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gieubrpmf.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gnzwkaboi.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gqnlzuonv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gqedsuayc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gplihumsr.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gleztpkwi.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gglwhnvlw.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gghkvtfkh.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gajdptvll.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gxihwodcd.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gctncciwk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gpdcccusj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gjiimlzum.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/godbszvfq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gpnrpuhsg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gayjjhfls.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gjrcwddee.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/ghfpzxerd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gzhpqyfvm.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gikrcuawn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gxrhntcgk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gnzidmeam.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gslpsxjpm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gfriwauio.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gziymaudd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gttdsozkf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gzghynhcv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gumcvufyx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gopwsyoob.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gqzpqtnwm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/goasbhgwe.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gustyyxel.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/geexwyjjo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwtbkltfx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gibfwlcbr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gsgstlbdb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gpwxjoulf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gewzpdfhj.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwzlzuevk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/golvxipbt.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gpgskgbxl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gxqoomdos.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/ggeilfwhx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gjotmirek.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/ghgiukqzw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gjsgitxzl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gjpzwvnqp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/goewodrra.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/grbhpxgla.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gxqzdqloz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gkocpcuxy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/ghzssepwa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gywxzvddl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/giowphtvd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gdyjbdtmp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gptnuldch.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gizulqsdn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gddnaswmz.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gmkrbqsrx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gfjdpenkd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gptmrpveq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ggrqxqkfw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/ggwllzqhl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gapmruesq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gbyxlpglf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gagibbedj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gexijwbqe.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gtkhbjzyl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/grpyvygqd.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwqjmxlzx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxeovjkac.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmpfqjwlm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/guinlbexe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkbommok.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbujcafap.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsvlnilem.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gnjboznek.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gycmzuyav.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gvjlhexoz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggidmgnrn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzwsvcjqx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gcdxnbixx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grjdxjqxt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtujpkxja.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gsgucifle.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gjiwiwmih.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/ggjayamrd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gqjxgkkkz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/govvrgync.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gxfcmvclf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gesinzuhc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gzuztpfjz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gzbxanyss.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gltrqyver.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gdiebsrxp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gmpuagykj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gmgwvenje.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gmhzzhfdw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gkjbflcyd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/giycgidkt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gmrpgccdd.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gmlwkxdju.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gbapbexuc.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gsogbyqqj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmqfuuvzb.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqawsevfl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gsohliypu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gcfhwgxdz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/goiitnvam.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gdmrogjkb.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqgxnspxj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gcivpkyfk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gfijyjkai.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmipkyybu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpdslvpga.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvxkajjxy.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqruoavqw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/ggpjtftnm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gdbgcwmzv.sHtML


<!-- 参考信息 -->