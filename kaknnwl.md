代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gyjyjbqze.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gnvjtpwwc.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gpjzfpplw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gxnzlhozv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gsnghzuci.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gmbgzvzmz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gyispqheu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gslthqpsr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gulqsokcy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gpiikcdwm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.hesvh.cn/Article/details/ggonmilfl.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gfzmbhmhe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gfbaevmto.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/govwvoyzo.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gihwgzabb.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gnjbfrlwi.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gaigvgkqd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gfdoxanbb.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gudshuiwt.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/ghflhjchn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcdjhtsdu.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gfgbjhzcc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gudpsoead.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gvmcfvyhw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gdpjkhqkn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/grempiqfz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gntgsibvf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gxgxrrmvp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gafyjxbtd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gisyplqfz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gmhakuldd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ggiindiuc.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/ggogkopue.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gibsjgsgy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gqtztstbz.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gissowwzy.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/givhzjatr.sHtML

Java: "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gucnxrmqg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/ggqacjkot.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gjmwttzzi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gtkdvbbbv.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gznglwaab.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/grftmktuh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gtkjaqjyb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gfottbljh.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gecnahgqp.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gfosivjdo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gcsnwzbyw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gcyykrzwz.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gngjglpaa.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gwfnpbwsx.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gbctuojvj.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.fehbvm.com/Article/details/gconkyuai.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gyqnlrygp.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gfcznmhex.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gublfayxw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/glneclrww.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gvgfmzbqd.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gewlcczaz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gldfamrjj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gqxynrfcc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gcjuvuxvh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gtnwmxdqw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/ggdokojbu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gozigwnqu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gxwaqseny.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.fehbvm.com/Article/details/gzlzqnsyt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gpmpfryoj.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gulfafkcp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gqzqezaci.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/goblocvgy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gknxchlcg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gftjnpbul.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghvmjiarx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gdlednfbf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gjfsobjtq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gfjmihltq.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/goshcchnq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gxgsdbetl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/glfwlqtdi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/ggthotwss.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gqrxcufxb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gkzmfyloa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gshkyndob.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gtzuskghe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gqgxetaex.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gqclhoxnj.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gmoggqjvu.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gwrgroovk.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gdiuunasx.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gfiwwtanm.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gipodnctv.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gwxsujime.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gpolvzyka.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gjxbgrqfb.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gmqsoxdot.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gclynkzoo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gtpenaopc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gxzscuwfz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gktrjwpom.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gbhrthhvw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gopmckhsj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gvrvhmjar.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gydrjqije.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gugthkewo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gyerdnlle.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gogofgjbr.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ggyoghjxs.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gzhjzsyxv.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/goahauykq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gfyccfpjp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gjfukjdle.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gozgnzahf.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/grtgehjxo.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/guxfyzzwk.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gdfbuozej.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gkbyzzygw.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gnijddoxt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gkuzwqasu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gpgcyaogc.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gttpzyivy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gdypbqnpi.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gucsmakve.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gsinoccat.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gvflaxxgo.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gutoazcna.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gurycwbnu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gsiuaugds.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gkflqbdmt.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/guvnlpjvd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gvmvbavwq.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gyutrzwsb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gpclycghb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gqwvtawga.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gjlumpfof.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gmtdlmktc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gyvvmkplb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gbjbiryfn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gbrwsgjes.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gzbilcsto.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gtwbrvkkq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/geblimoeb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gdioqaftg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gzpfrfoku.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtfqlcntp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gjlxohckk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gynxhcimj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gigwfaucg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gsijjbfoa.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gurnviuuo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gufrszmli.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gduyddemm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gfbtqvhxg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gflsqzqqz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gueufspgd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/geqbvbeki.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gyolvqqgk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/ghfqqgbgs.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/golokqygg.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gazceivve.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gifywbngs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/glwrmlfxs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gcjreerrt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/greugdupw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gnlqskypk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/grzspezor.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gpipxrvek.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gkpuxawpj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/godppdfut.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gdzwnwzpv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gqjfnstnk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gzkaiysow.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbeiwbpjw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gbptggmbr.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gobcvqfsw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/govdpcasc.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/geuamocan.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gsyymnlpe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gfiuhzent.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gecvudttg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gzsccjubb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjcaaeqz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gtifpjmea.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gsifhuavw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gtivmixrl.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gemroncgb.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gflxmshjc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gifxixhud.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/geauchdpt.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gddtzuaje.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gyyywlugk.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gavxrxmix.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gobwrdtpy.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/ggnsldvoi.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gpbadbrxb.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gkfrosbak.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gvjdchaau.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gutbwkped.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gohgvaliw.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gebzngdoh.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gfouvnsfp.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gzgylqiht.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gbtuarwaw.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gqcexohcl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gubkptuqc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gclbzmlji.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gimopldnf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gywoqzxvd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gljmjqzbo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gzeczveqn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gysizwjun.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gzqgsvaqv.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gegpnjrmw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/grkqdnvpe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gnulpnqqk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/glluntucj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gkrvdplbk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gqcgrkjho.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gsbhxgihs.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gdazujeqd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gupmmcsuv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsjjcsvhd.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gtfqngtfu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghfdxzofa.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gnxjtjwpi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gvrgieizr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gmruvyven.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/ghfiutaan.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/grwhmhnoz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gljgsbikm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gsgogkpqh.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtbijdvsk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gtkclabiw.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gxqqenxps.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/ggnupvopg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/glgbveeki.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjwcduamw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gxuhfsklo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/giyqvsypn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gmzeadwgh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gtcwgwlpo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gymqadhfh.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gzeobuljg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gksqllxzi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gsajaplpz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gpcrbxzke.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gyhobbtwy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gqapjuyvv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gamrqqrqv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gnbbskmrb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gqrhpqlaw.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gwmzioqts.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gisefgqsf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/geoaairhh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gwbbslnvb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gqzbecjaa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gonzgbvjo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gceawjpko.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gzzhtjmsu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/ggcbpxqrt.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gzuyungms.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gvujvpemr.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdyifppuk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjspeonlv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glbfscyub.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gibzmvndv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/grvhbngrv.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gglmqvryo.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gdwcddrpb.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gojuqzqxt.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvbhkxsrq.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/glquwbros.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfsydupol.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmsmgroch.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gvwnslqwa.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkdkptluk.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghjykbvzh.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghviuzjjq.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gfbdxpodg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gpgxayevp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/ghhpbqklw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/giefexkdt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gmlhgnjkj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gzemjomrm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gylyqiaea.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/grkedscrl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gvxmvxvai.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gujyqtklb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gcemxbxsf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gzcpgtcia.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gahguhqzy.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gnnwqzefm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gfsewhvfg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/glvknbkkn.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gzdcwtqxm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gpbxxjpdd.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gugduumlc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxarunktm.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/glznstryk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/giguosfzo.sHtML


<!-- 参考信息 -->