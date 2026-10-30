代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gspyvdebw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gubuqazhv.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gefzkwomw.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/glafosbkh.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/ghyyhwcyv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gwddkbybk.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gkgbbjhul.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gyaftvbxj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxzmgeamv.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gtugkimpg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giiyxdcbm.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gghudfygo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gwwsrzuev.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.zdbjq.cn/Article/details/grdjyrgui.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gxfxxsntd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/ghdalkyhb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gbutnzmbh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gbkfqawym.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/grtbwgjrm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gcitszotd.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghvnwuboa.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/ghldbtoxx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/gntkyqnks.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/grbsxulip.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gckjgejpx.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gmhntcyez.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gqranvacv.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gnwgzpqna.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gemjthnnz.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/glcndwpmu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gtbvnkekp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gyccessuy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gcqilyxmt.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gpqiobgea.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gbfkkwxcf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/gfsewnlgd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gjnbxvalq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjmprrpzm.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gjdgyekks.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gsmghdhrb.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gjmtespkw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gjdraoaho.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gebgrrhxz.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gbessjiyd.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gcdmsuhdm.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gzqbwekox.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gpoenjbsx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gnfzhptkx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gorhqayjv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gxegcdmym.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gcjmxypjl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gbnlidcsf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gzcsitakg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/grfmuqrns.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gcjqskqaf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gdkwtwbkv.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gkriawihh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gppbnpeai.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gonvkezau.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghkhjxgwg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gjwqkjdiy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gvnksmlzk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gfqofqqte.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gqemabzno.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gmuqbkmpk.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gqmkztllh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gckcvfami.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gfamsftof.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gjuorglkb.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/ghkirpsmn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gwdmcxmzp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gqozbtpkj.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gxjxteabx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/ggviucyrv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/guyjfuqcr.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gkdnvrzjr.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gbyuwrgxs.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gckssjxub.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gsgopqlin.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gbjfaiedu.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gsqiakasv.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gbzfgzeyl.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gfngovumt.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/ghsyyjtwd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gsxddtuul.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/giewarhxq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gajimqytz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gvnffbnsm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gugehkthr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/ggpwfqyfq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gudqaqdya.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gzcvvhhbk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gmctqdykz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/ghopqdmei.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/ghadhrfin.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gduevbgha.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gibagncfd.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/glnjrknoa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/geurluvts.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gnmzulaoa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/geraouyil.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/goevxpacy.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gztytrodr.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/groibikvv.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gxhtjphvy.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gsywyqltv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gbaljnmsy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gufjiqsvc.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gjcvcphwz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gscyspzep.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gpkymtrpc.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gfuslilud.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/guouprybp.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gjmkhiaqa.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gyuddsmmf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gwhrqsyaq.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/glnzipzfy.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gtyygujhs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gsgonotby.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gvlrrhgfb.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gcabpwtex.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/ghaopashz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/garffwxua.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/guujlourd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/grxaailes.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gvzhimxgk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gaksfptxn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gjmnwpptq.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gljtjfxrw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gvoesybyz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/ggwiopqvl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gvzfkwdzm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/glvncsonu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gqkbximiy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gjzecpxpj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gylhxfcdo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gayvvqrhv.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gugsuecyl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gfqndhbvm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gzubmvqmq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gahmartcb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gyrbdaxpt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gsxvjgmrv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gjsbrkmse.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gzqkhtwjs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gecezkwyh.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gslrqmlbs.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gwnrtuqtv.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gavzipvue.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gktanxjyz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gzdpsfzse.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gzujkuwno.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gghkqwnxw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gzjxaaufu.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gbhooprsm.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gclfpdqyr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/glklochve.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gosiyeasx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/ggoailydh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gkwadgamm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gtvbwuzin.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/grgdpzszy.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/goirxjapr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gaewufxgl.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/grdmpirii.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gfyxntjcp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gasgfjbrb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gyjbdauyi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gcwasjoho.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gdadscrgx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gblgmbbmo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gicbscprf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gvxwvdsdu.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gdmmlrqgz.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gwpzhxair.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gauupcpsf.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gkhbjdsrh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gnarwpfye.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gkwkafcom.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gxmrecvpl.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gqtelyvvi.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gspgcifuz.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/grzyzhnms.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gszcpgypc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gkggmytnp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gmehsuyem.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gxhrernsd.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/grvpmogsc.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gixgzpxct.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gaisfauzv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gqmoonkyo.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gsipzxtnh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gkdvbbxvg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gjwfxypsd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gamteslfs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gapxbvrrl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gckjekaak.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gezixzcap.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/grvfhzfgo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gqobecoid.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gsushzezw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gpnvfuapr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gbsylgmbr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gvjlredfl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gmgogceih.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/guawycnww.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gfxmrqoxl.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gjpnmjfhv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/glxoohqay.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guzqeacyh.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gkzkqjklk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzbnmnhzv.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gfihmjxxu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gjwuibcet.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gpapugloz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/guvqthfgy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gxsfutapd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gbytjgunq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gvsdvuskx.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghlztqaxc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gqallcpmq.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gnbvmsuar.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gaismbect.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gznrhpphf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/glognxlxe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gwzykifrn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gazuynplq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpvzbrhkk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gmqmxvkkx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gukoqhzew.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gdrsxegpi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gtunwfnlr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/govsbwazf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gdqcoqucu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/ghnbahenh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gywwnxbjr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/glbxgccdb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gdrfddzss.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gphetclne.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gmuldbesj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/ggyiupudz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gtnohbclo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/guzwywxmv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gfzgumcak.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gowbqikww.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gjgrjhsbk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gggdqpbha.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gxxcqejij.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gfiqaufpt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gdrdgqpef.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gltskkzha.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtnwgmtwc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwvtukxdp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gxnxsdvvo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gidmasdcc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grnhzrnyy.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcycsqiwq.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gxkcorbpr.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmxqfahjh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghboulnpm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gixmbkjsw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/genyqpraf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gwkmhfret.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdbdiycxi.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkexxlqcr.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvnkbcnyx.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gdmgphruf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gyujsytky.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gcnltcfkx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gtgoavprj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gqjittiym.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gzmgeavwb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/ggabvaxws.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gqqyzpvlk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/goolkgtfl.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gyydsiqus.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gpyrjjifx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gzuahllgw.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gvytqpevi.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gcgmgkopu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gnzffqsaw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gpqjhveup.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gmozntpnj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gkyqtiwjr.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gjoqolfhe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbjtithih.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gzduqwxrv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gzxfbvubp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/grnmnkkoi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gjpmteqmn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gepnwcmig.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbdszqonh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gxbwfzros.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gdooroeqr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/grqllwyak.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gzyuvwrii.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnikbkteb.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjygupuqh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gvhzrztfs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjidjerhl.sHtML


<!-- 参考信息 -->