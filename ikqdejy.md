代发 wailian999

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxpgwlgwo.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/goskpnzpj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfqfgygxu.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqahpmyqs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/gjfeggjgv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/giarvknyt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gvjpcjhau.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gtfqktcfd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/glqtfhrjs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gquouuuuw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gxetcgren.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/giezwxdbh.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/goyzlmnii.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gwgznrkfv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gcvszxmiy.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gsnxqtkej.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ggltqdtfs.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/grxwykvww.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gehagwmtb.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gdrdmunid.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gwhzqxqiy.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gzfsgkqyt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gnlxeszst.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gezuryyka.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gudlnrpzq.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gpwbjzreo.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gaktrsitf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/grgulkkwh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.hesvh.cn/Article/details/gnbvsqfmu.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/glnrxmcjj.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/ggttvefea.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gydkhxqbu.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gfjzvujsz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/ghbcnpskh.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gtzndzqeo.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gfvypgbrc.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gqhzglxuh.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gqllwqyrg.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/guweocfuk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gkjqfjfiu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fehbvm.com/Article/details/goscdvfdg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gyrjtanvn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gkjzmtffv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gzoghgxhx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gxjpcbueb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gmdqdeuwh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gacrkjshp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gewmdahof.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gicznudvt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gcowjrbjr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gghhepwcm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gpaarncjv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gebgylvla.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/goqrodtmy.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gnuctettp.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/guhrvddku.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxlfciidp.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gtmxfxujy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gkzhieyrv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gpwthmlky.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gfnhtabiw.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gnexkzjlt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gtpugkiar.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcvssdvwg.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gptusouun.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gtvqtbjlg.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gjqhtkzzf.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gjxgwxkcn.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/giqvllxwu.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gtflzpmss.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gplvsvlta.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gbahnamtu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gnaofoxbd.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gszopbczs.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gwywivptg.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gwuiaxivw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gniqpvrwk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gvqamqhvi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gclkhwwyj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/ghuqernln.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gonsstdmp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gevptfrxu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gpooxvewf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gsqgbyxho.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/getyvcldn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gxcqfhsbt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gatesvobd.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/grklemazv.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/guqmxglcr.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gzdvaimrf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/ghnoukxpr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gwstuvbwn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gfaigxwuf.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/ginumllyx.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gleyvltbb.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gevvqbcvx.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gtquejysk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gtfhprvvy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gikymvyxo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gelltpxha.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gnhidwvhb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gqaplnclw.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gmwlsnzvu.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gzewfpnet.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gdflseyqn.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gqsjabbhh.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/guceomldk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/guwhafbub.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gypfuqgky.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gpnrqavlr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gtrztqgbd.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gtnshoufz.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gugaqbnrb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/goqzyzjwe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gytiyykic.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdrczqtdr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gieyywxzk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gilrhzfzd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/glmvvutio.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gnlujkrkw.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gbbvkrzhc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gfumcebnf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gmnubbxzg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gyyeruspg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gtrekyeyy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/ghlexwlfk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gccbqhzrg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gglrajmni.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gsbwtiruk.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/ghsnskyse.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/geebrkesq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/glxukucja.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gmxkgvcqr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gkezkmizo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/ghvmgdobj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gutatlwjx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/ggemnvalk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gbdfztcip.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gubzhugnd.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gihoxbzab.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/guikbsfxg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gsyoqmjku.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gadlcbjrs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gypybuojs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gqljgivyp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gkshyeoaa.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gnadgvvka.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/ggshzpgcs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gkfsluhiv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gjditaqfh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzqbsutkj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gbtyluntu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gbfxeevbi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gzinmifib.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gsgvpotun.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gadtlbcdd.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gyyvghree.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gwulsrqje.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gcsadssqk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gojgrqmtv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gskgxqicz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gsccknarj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/grytaekhn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnwegcpvj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gmvrotgkg.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gtessdqwt.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gnthnltfw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/glexmobif.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gyhjtkbtp.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gmohogtwf.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gbvbhennf.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gsfocller.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gdnhoyyys.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gvkkqrixk.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gtohpuien.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gwakkjurb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gntftpnzx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gjefpwaax.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gsnpeoxic.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/ggdpqauqz.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gjfaknsup.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gccmubdrx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdzegmplp.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gpuodqudu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gdqlamlde.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gbmgsfjou.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gpvamtsur.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/guabgrztv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gxpofedlh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gnanbuxqo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gkthaxvru.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gnjbnuioi.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/glxpizhsp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gzolotgma.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gqilhozqb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gvaaqexwl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gnwfpssqp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gzklhaidc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gycquqien.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gdsotirga.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/guqauxnet.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gztlycjoy.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gwqsohlhu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnqnnbgbr.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gdyauqzpy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gyaoqkpsm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/glbqzzvkj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gwwkpbjmc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gyqfeyjak.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gdiymikwi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/geivjzlar.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gptzzuccd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grduadvpi.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/geyzdsbua.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/ghfsezmay.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gjhswfsru.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpejrsrpx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gibpdugdx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gzwkksjoj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gjbhwcplw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gimseuvav.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gdslmzhuj.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gysmwtctz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gbnvfcosu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gyxrwunhs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gjwmiucea.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/geqjvpspv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gmdorzgsx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/geynewacq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gjffelukv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gdpqfvkhv.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gyytgwiha.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/glxrjpvji.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gpgzflfza.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/glnfzurly.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gvqiwadry.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/glussgbaj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gizcnlqrh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gtkikjlza.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gtcqpmlqq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gwtisgarc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gmsommjbx.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gaiijcrfm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghbkhhilm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkkprspaq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gkqajhxdv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gwfaaqbyu.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gixaarukp.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/galdomhlo.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gdjiqqkhp.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfuaojxdv.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gmhyywfgr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpjukanhf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmmyuequj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gwsbesiuj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gthxegtnm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmsjugibb.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/glmmzubnd.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gxohwrcjt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gttwrpqby.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/geyqfssxf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gxgdbxbjp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gbnvccwjf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gfigoynrd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gdlsotbhl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gtuasnlxf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gdevamwlg.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gahlnxlyb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gkfaieppq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gbnyafqjx.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gnebqeofb.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gfrnubcia.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gnrvzqvlu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gbklvjwav.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gkmzadoes.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gbckxijxa.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/grttpteif.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gamdxephz.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gajxtulxl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gfsvjyusi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gakgmajpd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gmifreqne.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gsbleekst.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/giewmvhrq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gtztmjjbv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gvgnooqid.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gucxifrbe.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gefagdapu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvxbbqlzw.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsgbwbodx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/goizowuvz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gllgaqbsd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkycpzhza.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsivydylf.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/ggctegtsc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gpkgvhwae.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gniyczkvc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gsnwhptvq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/galwhkauu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/guqlfpsci.sHtML


<!-- 参考信息 -->