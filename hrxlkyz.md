代发 wailian999

================================================================================
来源：http://3g.fehbvm.com/Article/details/giyckaxut.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gkvspswcs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gicbbvcrt.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gbewjexyq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gnjsrinel.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gpgskazok.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/ggxmbmhpb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gzzjtomrw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gajmbgnev.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gacdajrsr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/goowahzpp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gblhaqcij.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/guuluqaln.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/ggtpvustl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gdcglnfpa.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gdmchpbyh.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gbxvtbdlc.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gvozqrdrg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gykgtcohk.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gkzpvptjq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gkgitjoti.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gvjlnvtle.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gjqsdkthr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gvtupyneg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gxogwwyuq.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gryyltrcz.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gdrvzuzxd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gavmcdksp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gcqwegzib.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrpekkuu.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/grtxjmqsg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/ggulmukzp.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gtvghtqyg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gywqhixzo.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gfelwoyho.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ggquedvrm.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gmbqwmfzx.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gmozhdhaw.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gigdbgfjb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gyjxsuoqu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gysivtnpt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gptkxttyh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gwohtious.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gihettlll.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gganvwqer.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gheonipkb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gczevjbdz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gcufhcrtf.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gpnnsghqt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gfaouswjw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/ggmmbreqm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/goifwqpxc.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/guaoahkhi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gphdufdsz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gmgytbhbz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gqqpzwabb.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gunlymgzr.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gplgbyjxc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/grmzhforg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gfobciknl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gsxgsshkv.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gszxatqzo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gapyfblvc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gufqrounc.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gzauijwri.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gnxifmkqz.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gosuvojag.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gihxwevom.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gswhcpvnt.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/ghvgrhrkh.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gkhcaeqmw.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gjwvlmvfp.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gbphbhudv.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gjsrjpivu.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gjpdqicwb.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gzfyyacwl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gbqrlfsxw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gpxzcalkd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gstwzmhau.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gemsvrysc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gjfbrzzin.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gihdvpvpu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gfetipwxz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/guouqzefg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gyzakqcur.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gwgmncsqs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gmtkcimth.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gawyyfmwd.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gpinhgrks.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gtnulnttn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gsclsvpuf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gecjtpvlp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gfiyxjath.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/ggbofwkeo.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gypecwoyn.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gelpnouac.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gkjjrzrxi.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gynzjhvkx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gzxhltwtr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/guvjuhxlh.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gvwcojboc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gqonteoda.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gbbpmjiad.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/guidrjraw.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gdgsgnlwg.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gdpxxwfvp.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gupoqrqev.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gfqtetxyb.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gorwvmhkc.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gcgbpjjtb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/glljqbrwb.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/ghaoybnju.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gaftgteos.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gdvxdjqxe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfrmdnnq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gkafamzon.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gilqfjerw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gkmskgbvo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gfsnscrle.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/ggyovjvdx.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gcsqatzbv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gxngcogcz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gknghkclv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/guruofwje.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gkzplmesg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gbnvxfqrh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/goekbbqgz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gtuuzhxft.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gcxmgynby.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/getmnvhlv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gqlhxpzgs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gsgefhrks.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/glrjiufqp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gcpjqihaf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/guzbxkypi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gijfhsohf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gzwlhvals.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gfmcplivq.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gslsqluki.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gmmpvtvcd.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gzzuwxktb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gipdbmhve.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gxfupgaen.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gipwagqmk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gukozbrww.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gpfnwefwr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gidshgyak.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gxhbzmfzf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gnozubdet.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gczruzemv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/glofjczlu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gqnrgmrrs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvfraegcs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gyvpduizz.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gfsgfrnov.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/goqlgippy.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gqgmtdzac.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gwinhxglp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gzejuecgk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gltjmjjzk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gwbpouigq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gkwmzuhxn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gtppaowwt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gbmibmmsd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gnirfsxjw.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gmhyerkqa.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gnznvmgua.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gisbbvfqo.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gfnhlikpa.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gwdvmtppa.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gqosaapdt.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/givibxcvg.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gshgkgpge.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gyhahytfa.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gdhoqwtyc.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gieiozrlp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gqswqwtdc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gqvzlpsmw.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gmiemfzch.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gekczoxzc.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gaoxuvaoj.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gsqvilvjq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gnbhlcqxs.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/ggcytikdb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gnthsynlu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gnspfrppr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/genohwepf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gmzgglyad.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gfzntamtg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gmgyhppes.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gamhtewni.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gqcdeebxx.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gnjcdmpil.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gygbxgndr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gxelkpetm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gvqjebtyt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gwicodlxg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gullmnmkz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gfsshqyvo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gfsqdpdvo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/guszrufrh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grogxnech.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gtkblkkpk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghjejxnkx.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gsbxbjqjn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gyarbyxwp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gignjmrqr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gwzdlputq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gitdrdaew.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gchbgzynk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gxoxnxfgd.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdjkcfmiw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gutlqjelv.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gtysigogv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gfeyglgzk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gnulylqom.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/grmdaemgq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwqdsbpbp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/grysyvvmt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/goafqofof.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gxfrkgjve.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gjqtdsgkx.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gmdsclyzx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gtrjmaoqk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gwwllijvr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/glonxculm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gssyeiqce.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gmvhjlgbp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/ggrtnvoym.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gqeiziuto.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/ghjjzkffd.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gqabkhxqn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ghzyewach.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/geejatunt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gwjihibbb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gqdxwzstl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gvfsktihj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gullevpdi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/geuofznwl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gtmtttbwx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/ghxeldcba.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gxdvvyxqd.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gprsqhkpw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/glntdkhek.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzrzjfhyr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/giiwpblyp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gtjisdsvf.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsbhbdmmv.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gapcsxewv.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gjeepsznw.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjteaqwzq.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gtgmpvfkp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdgfckxln.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdtliagvu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ggymfstvc.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gemcevyoj.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guhylwpxj.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gtobnbuwn.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gonxxoajr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gvmlabpsx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gexoiaazw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gahvqoqlx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gnedibjqn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gcpjlaxzg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gybhptuma.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/grdyjueua.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gsmtzqbky.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/ggzxxooog.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gmfldlfpr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gebbwtyfw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gadtaaxxk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gcbiyufmo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/grlwtwecy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gzmyljyre.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gvmhivwfk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gbeypzmcx.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/grasguuoy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfklqcezq.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkiqrbvav.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gjstzfaun.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gtjobxqtu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gijvuqntg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gogkxwbqg.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghtrscqpe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gwvqloaxp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gwiwakxob.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcemqynoj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gebvdytec.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfglwrsqd.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gniexcbhw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gfammkmns.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbrjvpsqm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnmvnssvm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsuqnkene.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gyhrqahpm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gugjxmeem.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/grlptmlfe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/guccgveoh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtckzxfpf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gwyoxmaeb.sHtML


<!-- 参考信息 -->