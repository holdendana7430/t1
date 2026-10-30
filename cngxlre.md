代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fanxiaobao.xyz/Article/details/gbcnsknnx.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fanxiaobao.xyz/Article/details/gmjpurrmm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgxhzrhk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpdgmrfi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnlrdzly.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsmqnvry.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfknktwz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxukslsmj.sHtML

[E02] 重复字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gapazftpj.sHtML

Py:   "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpixpufwi.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/ginlqwqlh.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gvjgeumun.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gjuobanhw.sHtML

Java: "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gexofgecf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gemcinzgo.sHtML

Ruby: "ab" * 3
来源：http://read.share.fanxiaobao.xyz/Article/details/gklwnrjzz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabolvgqs.sHtML

[E03] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdvucikj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaziaqkki.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gfqbpkfot.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqzyjheo.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejmbwteg.sHtML

Java: s.substring(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gpykrhlsz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fanxiaobao.xyz/Article/details/gyoslfieb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvkzngss.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gnvewqdph.sHtML

[E04] 查找子串位置
来源：http://m.share.fanxiaobao.xyz/Article/details/gczwiewzh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gipxbjsob.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjwcvmbg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gusdkybrf.sHtML

TS:   s.indexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/grjkobbjs.sHtML

Java: s.indexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/giyzhlwym.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxhrackm.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbceowfzz.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrprqmnk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gegulomoc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtktfuoj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fanxiaobao.xyz/Article/details/guxhuvsut.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/guqowjeqn.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gfdyujnqk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/glmtwteam.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbzysbfz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpvxftkg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpndofyp.sHtML

[E06] 替换子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guurlcfyv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gevyrxemr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gslawadgi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gombsbrwo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyugekuz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/godlvppfa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmwdlhrz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gaaflxdwv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkjanezg.sHtML

[E07] 按分隔符拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gooezyxob.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynkblacm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlkzyity.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gykgqnyax.sHtML

TS:   s.split(",")
来源：http://blog.fanxiaobao.xyz/Article/details/grmhhsgws.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjockduv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fanxiaobao.xyz/Article/details/giogntfyq.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnixysjp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fanxiaobao.xyz/Article/details/guuptdoqa.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fanxiaobao.xyz/Article/details/gidvwkplo.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbniymuyn.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvfzsgvh.sHtML

JS:   items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gndgtaqyq.sHtML

TS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahrwtztt.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggibxjxjq.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fanxiaobao.xyz/Article/details/gdjilhlkb.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjksvggd.sHtML

C#:   string.Join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/gadtjofli.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxejipmjb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/grwdoaqln.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwjmgfwh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gvsqsmvor.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxcovngb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fanxiaobao.xyz/Article/details/gqbqpujqm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fanxiaobao.xyz/Article/details/gywnsmbva.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkktverh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghteltpqn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvlvcele.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsfviyet.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcdhzcpq.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbxqxuob.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gdktmwzik.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/galcyhdpp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaiwggln.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzhtkpju.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fanxiaobao.xyz/Article/details/gtrpdqqen.sHtML

[E11] 反转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gpixrvqat.sHtML

Py:   s[::-1]
来源：http://3g.fanxiaobao.xyz/Article/details/giilpbfcc.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptlkvgfy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutsprylh.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gxbrxottc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/givwnxivh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fanxiaobao.xyz/Article/details/gisxazldk.sHtML

Ruby: s.reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/geghztwpa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/gmktipayn.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtserztz.sHtML

Py:   s.count("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmolywcnv.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fanxiaobao.xyz/Article/details/gqsvjhwzx.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gaatcnumt.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/gzihkabzj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fanxiaobao.xyz/Article/details/gaikildxt.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fanxiaobao.xyz/Article/details/genjjwxoh.sHtML

Ruby: s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuwttpjo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsvsllbo.sHtML

[E13] 逐字符遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gabowobff.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizwfhswt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyciasfsl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzpwcbfw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/grtdjonmh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoacqtsi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gbwglqqek.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fanxiaobao.xyz/Article/details/gosesknpz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gstvarvjc.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpxmezep.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqumcqbu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gmfyapglr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmsytooq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknwrreye.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gztapfodh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fanxiaobao.xyz/Article/details/gblsgtsip.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gexdzakqi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gstartyal.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcwxpkli.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaicqbhiq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gitjqngbv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvxdhaqs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gpvrmlyok.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fanxiaobao.xyz/Article/details/gczxavvqa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvqnwdln.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gcizkviee.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghxbdlwio.sHtML

[E16] 数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gncksismu.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gemawqlka.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fanxiaobao.xyz/Article/details/givvufjgs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fanxiaobao.xyz/Article/details/gbxsypsfj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouiqusmc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvypexroj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqusbmqf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqedfysmg.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvvtqkzs.sHtML

[E17] 首字母大写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogjecjvr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiemigyy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gxixsqtno.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gpugyrdee.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gugqsmhkj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykcykkrz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzsvftlc.sHtML

Ruby: s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/gxdjqjqsm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grplfzmmg.sHtML

[E18] 模板占位符替换
来源：http://wap.fanxiaobao.xyz/Article/details/gqqzjslcy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fanxiaobao.xyz/Article/details/gkwgkhzve.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnwtbqal.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/galjlpqwz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gtyraauzc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbrfmwxf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gciuixlkd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemzrking.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbaeumdzn.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/gaytxykol.sHtML

Py:   s.splitlines()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgqmadkb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgxfryzi.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwvcskyi.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqfzfwvn.sHtML

Java: s.lines().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gwhqimbfy.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gafrmmskm.sHtML

Ruby: s.lines
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsqqmjjm.sHtML

C#:   s.Split('\n')
来源：http://wap.fanxiaobao.xyz/Article/details/gbdwpmbct.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fanxiaobao.xyz/Article/details/gpucdkupu.sHtML

Py:   if not s:
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjhgetim.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fanxiaobao.xyz/Article/details/gttyvisyp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gihfswzkx.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlhdqavv.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkbfwozx.sHtML

Go:   if s == "" {}
来源：http://baike.fanxiaobao.xyz/Article/details/gbzmnaxub.sHtML

Ruby: if s.empty?
来源：http://baike.fanxiaobao.xyz/Article/details/gncqpareh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgkestga.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoiptgej.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fanxiaobao.xyz/Article/details/guvwxieev.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmvfqlzm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/guhwjwnuu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gphhmlysa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gwpmbbfhu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeekvygl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gknxiatcn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrrxypep.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fanxiaobao.xyz/Article/details/gdujzblpr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewmvuoes.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gmgxpravp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/glxmeojlu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gooxebxwk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnuqvyvx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcaeuzlmt.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gynzonvdm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkrkjaex.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuxqoyim.sHtML

F. 文件与目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gknvozwqt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/glnfymbbk.sHtML

[F01] 读取整个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzcdicoxn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkikycey.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gpkybudda.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjhcncnc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrbsvwoi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gzfkzgrqv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsclhssam.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gputvnitt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/giznrqwhn.sHtML

[F02] 逐行读取文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsaudmxzv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fanxiaobao.xyz/Article/details/gjxrinudb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynozgrbm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqiozqie.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gpqrdltgk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/gtakjcekp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhyehprr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxbxoonr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwfqpccxz.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fanxiaobao.xyz/Article/details/glwvrtoay.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gwgmqafms.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gdhggjtpb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/goxznqwem.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvzrtvtd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gvwprqqxb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfcuesnz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gudlyzvnt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqskkclan.sHtML

[F04] 追加写入文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqhwpvva.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gfenmzicv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fanxiaobao.xyz/Article/details/gassblyfk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gunadpcqi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gzcstxjyr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmocgztio.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gikvlvpab.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fanxiaobao.xyz/Article/details/gyrysjpty.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvpdbict.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfutwmqjm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnrunrdk.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbycqiruj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssovcsix.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gqthylvry.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzxnbsjp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwlxgvkz.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gsasyuzfn.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/glckvmjov.sHtML

[F06] 删除文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcvbngbop.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gebxndufu.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gxelcuoze.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxduygfx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/getwnugzq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqxaejqo.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gjhwxrucx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/guzsnxhwo.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gpnrnidzu.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fanxiaobao.xyz/Article/details/gfbinzsvz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgmjhwtg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkyxwwrb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/gailbpnnp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/glekxeiiv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwxiwnmg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggufzlrun.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fanxiaobao.xyz/Article/details/gwjgxwhln.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzctpvajw.sHtML

[F08] 遍历目录
来源：http://3g.fanxiaobao.xyz/Article/details/gsafqyioc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozqfuhtv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/geqwnvuix.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwajhbvvu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpeuvzxs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gvasjneiw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdgxogpg.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqppwbpmr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyksrxjo.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpddefpaz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyyrkvzj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gemnubyrz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmmbkohh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fanxiaobao.xyz/Article/details/grruzifzs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebxaewfe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fanxiaobao.xyz/Article/details/gkbvmagbt.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrrozvjw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxwjwyud.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfscaawb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/ghjstlxtq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gobkjecjx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjivezmz.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gdzkeixni.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fanxiaobao.xyz/Article/details/guxzsstpv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/ggaoovnyt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gmwalsvdh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhooxmez.sHtML

[F11] 复制与移动文件
来源：http://blog.fanxiaobao.xyz/Article/details/gakqxwkty.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcgoarbd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbpgcxvp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gytqcmdij.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfhjysnx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gptaawpox.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fanxiaobao.xyz/Article/details/gaylfjhtw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnucrgppa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsevptomm.sHtML

[F12] CSV 读写
来源：http://blog.fanxiaobao.xyz/Article/details/gzulmysgb.sHtML


<!-- 参考信息 -->