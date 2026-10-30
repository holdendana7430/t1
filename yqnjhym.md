代发 wailian999

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glwpcdply.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gslncetkz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glqxzcqry.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gbjeuyiom.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gqjmpxtcw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/ggtdjbjtl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/grsffpiki.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/godxbxxeb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gnyhghnkb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gwpnbaggw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gipabfmky.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gmljwwlrh.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gnhjozleo.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gtimotfzg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/glpnxdtqw.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/geippzaxt.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/glyfsavfe.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gdtmsgaxu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gtehhpixb.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gfnlrtrau.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gimncowxo.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gaftknenv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gnyxemabi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gzowhjbtq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/ggfwbnxjo.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gkpdmkzdo.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gekvtlljh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gcbaryubv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gqmqqmkeb.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gwhxuzafl.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/grejrcpfm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/givouaxrh.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gflfzuohm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gjaclxyxz.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gnmqnvxeu.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gxvlawhqn.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gyhllaqhp.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gcphiiaqf.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gyolbdyqc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/ghptwvxve.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/ghxjqvwzu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/guvheoxts.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/ggmyovwtb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/glrmhrhcx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gwrkkkyhs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gaiafniqj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gntykseyr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gnxornuru.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gdcdxtxwd.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gmlnlxsuw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/golzehxdw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gfxnuxqan.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gbsnjartr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/glvzrxwig.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/ghzsxgmcv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gvvixmogd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gboongipa.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/ghqgyzjiq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gorlanhcw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gvbbheteb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gekxcowsd.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gxdwuxbup.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gpiajhmhf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gcojoqghs.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gjucjsgsj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gqhxxztdg.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/ghoawvhos.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gwqkkpayz.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gfyfmlrdr.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gatyuxhih.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gujgzkrey.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gznnetskp.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gffdstkrr.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gmagqzdsy.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/glptsmxba.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gzthpeydz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/guorfefav.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gdtlnqmtp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/ganbtugkh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gxmucjoaa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gipxwvhkr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/ggbmofzpw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gyhtdhvmf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gqkzidfkz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gtuyqgzcv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/galphpucb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gnlgcmxqy.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gkwntoakv.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gkacyrwxn.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gaffavnit.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gzalxcdrz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/goarqgcgt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gxjfytnit.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gvoammntw.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gxmsamspv.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gpqkuvnrd.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gzbucegrh.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gutnqzhky.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gbngjfzog.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gyujlrzve.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gkzowchid.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/geajshnlr.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gcptkgdsm.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gkqmgxrzs.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gwzaugiur.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gjuozjbrd.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gmnjuzdve.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gyliqdemg.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gdpqupxgk.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gxbdhcgym.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gcqargbzz.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gskuowmvy.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gwielhlck.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gixdeqlnp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gazkhqxsg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/giiakqlza.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gwkedaisf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/ggsxutocl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/grsprnfim.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/giczrjnbi.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gbjqfnxnn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/goemmskej.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gxlcbtzle.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gcsbdqmkw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gszvoehpj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvoqinxp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/grqpvzdsu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gltxxbjkn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/grgkvnosn.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gqkzhuboa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpbvtlghd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gntgtkqhp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/ganbcpcpx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gnqhybojg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gfvcrexhu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gyxzsfegp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gtivnedqt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtipvfyas.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gxdskryuo.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gbtyfricj.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/girviwpti.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gwvspjinl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gxdpsqgea.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gmwvjgtdd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/ganuhxfel.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gbwvwlsnv.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gzdmzzqbp.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gieitucsq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gaxxqpujd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/grsfpfgsu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gqguvxqvu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gmabbbhlc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggriqwrmd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gkcyxydup.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gixdfpntg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/ginhsypyj.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gzqawbuqv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gdfgvjhjl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gtgutsarr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gitnepbgt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gbxmlleti.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gwrteefgw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gwtikwfsr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gtokdkiph.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnihfufsq.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gcqilofxd.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gfxdvrhax.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gqwtkjqbm.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gmkjzzkjt.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gtodlcfgk.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gzwxfcghp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gamhxcyoo.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gycfgmecx.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gyjhywwwg.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gujtlhgat.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/glmmmcpeo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/ggtxynmdl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/grccwkfsa.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gxbwhqlxg.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gcyjemabx.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/grybydkls.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gyltuigae.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/grhyqywug.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gmqnsykqs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gqwbjsain.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gxhmwscub.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gzjjwyyqi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gadmrkilz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gsmmsyljh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/ghdlvygih.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gfqohepbk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gfqkmxoql.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gukxkuxjz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gsszqsyzb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gopvmjwze.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gnzgqyoew.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gmbsxdsnb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/geihacysa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gimswrygn.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gzjaqsymz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gyvindhlt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gebpyodyi.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gayfpvalm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjrwcahmv.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gynfrmotv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gqtaxvjwu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/glzfyyqgb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gahqbjceg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gncpwuzyq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/ghgbemmgt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gictzacad.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gnvkdsxkq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gtufubcfh.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/ghcdpkjdz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/ggwbjzqis.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gceurdwbt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gyqupftbw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gdxihvbky.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/grrghvcfd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gksnztfkl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gawcebknx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gatbledhb.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gflkpeybl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gjdlzymct.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gvbdxosaz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gtoiijyeb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/giecvloxm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gvtpmesqp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/glgrwjixl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gjoqosswp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gmomxbhrh.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gceiyxsdy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gbyfwoxlf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gawlqpyep.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gmwsasqsf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gkgameuim.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gqhpgnbns.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gtpxocytp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gmntxwtqs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gvngmjfmy.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gsfrgqwfs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gaipqbouf.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcceknzjd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwuxtewzi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gobuujndm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/ghdresvsx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gqnsvmxkq.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gshyofgdg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzrbdivtp.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gmotzmise.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gganvymuo.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghtfppsfl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmazcchya.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gozeicbct.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gfrrfvhuw.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbefwxmbc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gilqysuwa.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gjgplmyjb.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gghhwizkz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gjqhocarm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/geuffcalt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gphkdfhrr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gigwlooby.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gjgpitnyi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gykmwwzpn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gwiuglzif.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gmmfdvzgi.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gvxialpuu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/ghxgvqtfl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gvnjgrnbp.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gogmglyyn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gtqidmobj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gujlzjrtq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/ghcbmllnj.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gaxhpwbbr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gggwzgslh.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gmfytpvil.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzsytkljr.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghcysznhk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gjfbsully.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gczsjxjzv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gulvxlnle.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gcjglnhbh.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcjxvubuc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gwadtmvgu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gjianjeoc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjemmfmmr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gollkzmom.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gkuqxbhlt.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmcocmygd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gbxcgpijr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqdqfhlad.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grogvzvvb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbyqxbbju.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/guaqtjzaw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxytmxosi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gnktlxrsn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gvhalhsdm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtfrqnmsm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gfazrpqug.sHtML


<!-- 参考信息 -->