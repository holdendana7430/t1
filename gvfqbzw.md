代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gipybqihv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gjitewuds.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gwkzgzaqv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gomoupgmu.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/gddohjnkh.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gtsfxawqf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gpwfbbbfp.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/ggpdldcph.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gwdfgtgft.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gqsqlyqma.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gmrhdfyqb.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/guwyudndw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gdamsgwrz.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gplwvpgxr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gtvkpcqho.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gpzwcyuhd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gzmwfybug.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gkqzvepyk.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjvdwnhl.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gblyxrszb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gkswfsyle.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/gbtiaxxgn.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/grcusacog.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gfrgqjxmq.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gxanueriw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gyfgaovry.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gltjkcvnv.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gasgqqbgl.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gyhsgefeb.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gtepqnive.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gqhvnajuz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gznwgghui.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gnvyyzgts.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/ghfwpnazq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gfeltuwsv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gkpqgkiom.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gsskbupwd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gpiscfjlb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gnvmwmyfm.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gnmbsbkyv.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/glreixxkc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gttbmlnmq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/ggpkskrnr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gtrlleukn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gluejpxyw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gyyhhhjha.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gerbubecl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/ggqwqxtmd.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gvleybzzk.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gywlieivz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gjewnegep.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gajvqheao.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gqeahidcz.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gdpigroou.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gvhvgtcwk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/guhhjxiqa.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/grwgkwzhn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gsfbimifs.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gyntfitme.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gleblomqs.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/glmznytip.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gghkznmas.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gpimkzida.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gribpvccp.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gptshvcqn.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gaexkmyxi.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gybhoxnkt.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gdzhuftwr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gtfjirvle.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gdzybkawb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/geyoxsvmy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gxbgutopu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gujgedcxa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gndhekpjo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gikdicbrp.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gapaiyfoj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gyncibety.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gytekertz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gopbpfihj.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gwhbcbhho.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/goolptcpr.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gzxbykskp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gubkleufi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/ggmutguyo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/grqpffdos.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gawaylfhd.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gjhhwbklz.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gznuhgsko.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gzulvhlyo.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/grtxdbozf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gaytkjtuo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gvwbjxfkh.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gmsujczvs.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gxgcqqdzh.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gidzqeegd.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gdwtkyvjv.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gmjfkctna.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gvmyenfil.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gcipjlshd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gopepnfsb.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gbaqqoxqc.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/ggtaqpswf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gclthledw.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/glbdiccce.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gizrptyab.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpowgqphn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gcgputlkp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gcwehaqxe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gwdxwvvoc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gvnatjvnh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gltwhxiys.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gkbggcrnz.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/ggbdrbkol.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gfcqeisna.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gvtutketn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gzfaktmuw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/ghiuprzqj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gsaisgrpp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gjqjqynhh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gnvdwhyyj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gyjhcggpo.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gwzbcnzxk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gnyjgdjjf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gzekgnjsk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gunxpbkte.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gqfxmfrtw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gqgikqwoc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/glszpnfnw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwilkqmuo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/ggmgduxvd.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gxgswicxu.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gxjzzwuis.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gqubhiskk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gknykpzcj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/glcdotbcw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gvctcpxho.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gqufnbevx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gxgkotdhm.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gikddrbdl.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gohbbzdvu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gtbwiaahu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gjopqsaum.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gukcoouzz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gmwiwrvaw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/grrwnxmfu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gfjqwrmgj.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gjxamtari.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gzybaeggs.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gkpnpuaov.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/glkycljql.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gwgyukpzj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gjkxzjsdk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/ghfvphbfx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gexdjsrqq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gwcjanmfo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gunuwafsu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gadblzfft.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/guisedcso.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/grydxcfjq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/guvvaqirp.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gdwfclgfw.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gpivjbtcx.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gexfppvrk.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gsdvbvuoh.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/geqwduaii.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gcyeeyowf.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gqtyvvayj.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gswtnfaov.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gkbfalday.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gseqbsydd.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gyeirnuyc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glmrvhipp.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/grbwefpfr.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gkbvhyoqr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/grmdbljko.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gxvgfoede.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gpahzzido.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gdjqwjyoe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gchivtmrc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gbqwotxfu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gwscfwjhi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gtoyzimup.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gfuvziyns.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gqdckhkob.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gpazqdxhn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gekehvylp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gqzjjscrc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/grfbfgvch.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gbgtdueat.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gtxudbpps.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gmrxhqzuf.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gqgcrodtd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gosnlpkcg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giiuaiklr.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gukcyxqfq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdwxlnmkz.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/grrreypjg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gfqgyvwng.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzkraaohi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gogbynhgg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gjjzmxzvj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gtrfekbtg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gpdibjgdg.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnletxhmh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghbshtiny.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gyvgunipj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gzfvcbvqg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/guzfgxydv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gcrfgkksl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gxhekxwho.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gvsfzlwpo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gqbhvabza.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gmfddscud.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/goaygcynz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gqouzrhlk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gspzsyura.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/grspqklky.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gajwrukgr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gymsjlhzt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gfztwtgbu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gywsiznew.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/ghudvsdip.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gdvsdytwg.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gakoqqwtr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/geqtmcwbc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gsejxxspq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gtoejengz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/grczgtkzj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/grhlliube.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gklsvhupz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gkaeypkzc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gzlmxcasp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gqajobdiy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gkcvjmxpg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gsevfbrkw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grdnexgns.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/grfrrztgd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gbbeqmtyk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gohsvtihn.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gympmlseu.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghquzbbyf.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gtygfcrou.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtdtvetmv.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbuxjdeqz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/grjianwzm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/geusbtisr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/glryctwks.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsomfsrdi.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxdnayrfg.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gulbrvfwe.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gwlsppdjc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/grumjwzam.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gtlsahdas.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gpaamcknz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gbgwpjjga.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gurnrvivl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gymgeqjyt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gjtegdubc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gouaqdyeb.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gylfhxvit.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/girjtfhpt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gumnbvifz.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gnfcmvfkr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gftcfgvpt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gcqthvfxb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gnudtkbyn.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gdkfvkjmb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gifpmlagt.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gmtdlojzv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gflcbqvmp.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjwchxded.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gjryqjueq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/goubbgwjh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/giapjwhzq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gjfsqawiv.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghgwlzbnl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/ghbkjurzp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gwiyaumaw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfrgvbrye.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/ghbmjqxnx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gamewfipo.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/geomdaeuy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gzvfdjcix.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsifyjklv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gaunpvjfk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvsiemonw.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gzggbfpyh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gwhyuttzv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gkbgckegz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gwahhgbxp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gazbhznve.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gkmboiwcn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gyfgmqgbc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gsiytubvg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gsukfavwg.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gronctsvb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gddikqest.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gdhgrohpr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gmfnhbqfy.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gimykwrsj.sHtML


<!-- 参考信息 -->