代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/geseijmpu.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gtmttbxjz.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gsvqhtucf.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gxtzisseh.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gegyqwdye.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gbpcdtjwo.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gjebnpxbl.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gtfvvuljj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqolmycgu.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gujsiugyg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtvazklee.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdmmmafbo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gglpyknpb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gcvsnadzw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gkapddpfh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gloctwrwt.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.fehbvm.com/Article/details/gjqkoautz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/grsnvawri.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gnwirgzyf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/galufxknk.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/gmovkppnp.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gyaeubnlu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/ggaqiqhsj.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gifxkumag.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gwiuvwslb.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gzkwnhcby.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gouonqslm.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/goctaufal.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gwftyuwls.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gqzlrbtgr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/ggteglfkr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gjozkavts.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/grsnfuwer.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gtccfxxwq.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gfjtnyhzz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gcbyymaby.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/grgbapfiw.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/ghwbboeiy.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gdhhpucwa.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gbyazphqk.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/gjoitcqhc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gozmrkamp.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gnkpmmxmn.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gelsqvdga.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.zdbjq.cn/Article/details/gxjkfqwma.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gxezdfldt.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gysiqlfji.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/ggmwlglvl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gmhinowfa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gedfpookb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gpkfhnioo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gjziciffl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gyqpfqgvn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gdcuzdoqu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gwckrkdkx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/glpmvgshk.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gjojesvow.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/ggbbupaya.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/ghysvlywv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gkucfchzl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gesgulogz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gcbjicjhz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/galojagpx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gucvppamb.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmgfnbqnt.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gndoruqvl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gxjkjnczj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/geeynrqky.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gxgmnlhhx.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gdeslqtev.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gynemkykj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqtgjlbhm.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gkmagygxu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gjnzescdf.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/geezqhred.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gvuddtadt.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/ghcnldvec.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gbsdgmysd.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gzvibgdsz.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/ghirszzhk.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/geowfjdtn.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/glsxdkoth.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gvighsfrp.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gdvdumwxj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gbifbfufb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gnkgyexko.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gcvfytqkk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/ghdlpobqj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/glabjirxb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/glsgihvzi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gmppyeqcr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gsovnqyvv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gysxyxggi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gfliwxeae.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gadeflyhm.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/geehqlqjw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/goyruenie.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gsiukmkip.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gcvabxqxi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gfamsneyu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gspmhqdpm.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gngouevlx.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gicjsjxqp.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gnjprajcl.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gklpmkqlo.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/guyegbjlx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gruuqbpfs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gbxpdyoif.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/goafokkvb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gnnepyvtf.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gyjdqaywc.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gadhuaoir.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gisdzwyzt.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gdniyxzzo.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gaandhgle.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gfkcnwcst.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gwqqrnttb.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gipvqmgjv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gxxxnjldh.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gbotljcjz.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gqieewbes.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gtoiwppbt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gcrjtetlc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/glesrlwsu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gxllkpxqk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/geckemhye.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gfqqjtzhr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gthhcwnuy.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gxosfoyjs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gpuqpwnjb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gycamzbcp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/ggqpmdmel.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gcrsietoc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gjeqmzymj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gypdewqmq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gxotqfrhb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gaabbbwfn.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gfsiysuzx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gliqczdwj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gissybmwr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyuddzyti.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gehzkeysm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gvrqczxqt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzifcudzp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gduirqstq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gctfkkpxo.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gpoxvvsta.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gynuxscdw.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/grtvyhzrj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gwclqpcmf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gawkgzstp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gympgyagx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/ghdftbser.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gysbgjlal.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gkbkrhwxt.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/ggvonahrx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gablkawyh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gvkjpnmro.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gtvtuxavl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gqduzomhw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gktpnhwke.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gptyekzyl.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gfcicixfh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gsvcecwtn.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/glekmzvpc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gmvagooiz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gprflvxte.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gogpccqpw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gaddewnnc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gbgzgwbiu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gholulbgi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gtevkgswi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gficdewyl.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gigbxfpdx.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/grjscoclr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gstxbnehe.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gktwtbndh.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gioimahnz.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/guiuualoy.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gkkbpmxqb.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/ggeazobbt.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gmlsrkrvl.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gygdxssnd.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gicjveuen.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gjrxjidkb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gkktedoty.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gngzobrpy.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gfwebfmij.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gadcbybpi.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gqomuepkf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gmfidcgfw.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gveqbeigk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/ghrmfpnbk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gepeffgvf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkozmstcu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gylulmmmb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gymepmizu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gqxnfoaia.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gzrvnbjjn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gyftqiuag.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gibirffrz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/growcqzah.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/glbtiqikk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gfvzjbqfz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/godrrtncg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gctdvbwen.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/ghftjjscx.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gzwqweumn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/ggtciooxr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyjaueozi.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gcnadbbwm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxgteuyvl.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gyjqgujmk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gdsxoonlr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcgpfyxfi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gblpnxowr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gojwyfhfh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gjvfnbdhm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gydhxwumw.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjladihbs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghktsynyb.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gwehhgwwj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/ggwwdwzdw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gwrucmihe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gyotthbjs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gqozczddg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gzsqjspbe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gvrffyqcs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gjonmvwfq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gkiimqxuh.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gjtncoqcq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gltbsbxmq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/ghindktcm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gywtlsinj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/ghifxqurb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gletxnjrt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gprupkvuq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gutpeylwt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gzbysfaal.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gesnzsdfj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gwqrzgubu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gtttsqity.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gzjiefopd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gjpcjbevv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gqnfxbsdv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gdmloyvnm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gqnrfykci.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gexusgibo.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gnlmysslu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gmiktmvhz.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gvibyyzdi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjunpshyb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvgfbpnso.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/guonrxsbg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/ghqdyrmnc.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbdrkkost.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/glzvzrjal.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gqqypseol.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzmugwulg.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwchdjvad.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gppzfamti.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxisthmfh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gihonajeg.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gginticfa.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvsthsbli.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzaiwefhc.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/ghgvdeykc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gpgggqmwm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gukieksmf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gsnbydbhu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gvbqdlehu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gnojonwiy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gufbnhnxk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gixxhxfzy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gfawgkuxw.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gvltnezex.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gabfrnnjm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gookafvxn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gmfurkzbd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gnycxwpuj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gyxbbblal.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gceneokkm.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gcwxjypzh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gekkvqxhu.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gescgshxe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/guzhbomfk.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxfbygexv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gfhlvjloj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gafwgalvq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/ginkdglhw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gcssfnpqu.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmlezvjjc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gydwuqldy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/ggvdrbmmz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggnnixpvv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfhujadyr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtqdweohp.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpmddyehx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/ggjqruiyx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/guxygsaqv.sHtML


<!-- 参考信息 -->