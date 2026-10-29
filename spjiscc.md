代发 wailian999

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gknygdngz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/goryqjual.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gbwqxemyg.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gvvqmouai.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdgoatdtw.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gaswjuvao.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghlkxakmq.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gkglmjxuy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gvgnldbiy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/guglncmnw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gvidoyazu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gxbmpsekn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gflollbzy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gyikcsyup.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gaykivfsl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gwjuqocst.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/glkhdmcvn.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gjkhnhola.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gbpvvmpap.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbvjncoez.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/ghjmuelga.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/givuzqobw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gpborufnq.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/ghhsdukhk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/ginluxlch.sHtML

[E03] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gwzmjfzkg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gxlstkrxv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gyvdvvcqt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/ghhubguxw.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gidatcgds.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gbthnurcr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gaxnamweq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gamgnhtwy.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gfojzjhyp.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gzjzjscqu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/grkjtdnkr.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gbqinfhza.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/glwoknhfy.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gevdqktpk.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gfwqvdvea.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gwtrfvqsn.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gtwaoowco.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gsugcpsjj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/grwwcrdqm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gsluwxnwa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/guxstgmry.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gcqxrrubk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gmldmjvgs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gouvtktvu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/glacaquhx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gjlvyyfyp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/ghfwfbpzo.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gihmajdoe.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gzooecfyy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/ghnffnsxo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gmykxpene.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gjklgfvwz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/grrcolcfp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/golioqawi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.hesvh.cn/Article/details/gzyfsikub.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gxdkranqy.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/ghrhyqsfw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gdkywkxls.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gmzidwipn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gkygkcbdf.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gwnhgvjvv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gryitmvgp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gmugzsqdw.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/ghshsemri.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gohxlyoel.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gvcjfedld.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gyqsfucmu.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gbrnmjjxk.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gmesfwifh.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/grvtbaxzi.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gvwpwdcis.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gzppanaca.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gjqlfmeka.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gogxoqxvo.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/ghfpbkmdk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gekahlwvc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gedsjohfw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gyoerhthz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gkptwfzsj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gsmsbrgkt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gadjbtgmd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gqjleoxdv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gghaemttk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gloyymtae.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/goqbjeaqa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gclfyeylm.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gdthmcdja.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/guoqirdoo.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gshjlqefr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gzxgkiriv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/ghmyotezk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gbiwjaxrz.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gdxiumfjq.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gfbasvckq.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtwwiofnd.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gljvdcoot.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gjzdzoohe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gwfzevfgf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gogoqxito.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gjzpsyisw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/grqtlxybn.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gkszlpjld.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/guuenttjf.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/glwhxyesv.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gteelizsx.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gyjjeqleh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gmjjtjxob.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gflfeymek.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gjssefoel.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/galxlxmht.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gtthwitcb.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gsydfnomz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/grafolneh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/guuispded.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gkhdnfhbk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gaqqqwyfq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gwvmhobaq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gxynvkipi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gdcmmyufj.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gavlxxvmi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gtvjbrqej.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gytpbnutn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gdgfiwuel.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gfpvmuhyq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gvyyaipol.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/ghvyybkep.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gqmcnearg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gpijspbpa.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gqbvysnrn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqsbzxrni.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/ggissdhxx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gqdvfdyab.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gyexbbvqw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gxxqkcfxx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/glbvlrssn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gknafzqrv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gmjdcrixb.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gxmrlooiw.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/giirygxas.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gchlduwml.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gavibskru.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gepghbmim.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gfomvcixg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gzhypjpyr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gnildyaqk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/giqcvelyw.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/ggzgkyiff.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gqpyibbbz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gaowhtmqj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gcejclgro.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkgxxryuo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gpyyayvvz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gsuwnguli.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gbazetkto.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gqhwxuzrd.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/ghucbjcmu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gfvbeqidw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gmpxqleab.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/garrinqvh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gwmcnwooa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/guwllyezl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gvzrzhcou.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gywjlazsj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gkobzkopk.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/glfxnezxa.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/ghbricndv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/grbujnjgw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/grovofbfb.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/guggqpiow.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gblghdtwq.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gobfjovfy.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gdilxfift.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gkptupvtc.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gctltanvb.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/glvwvpzmf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gorlagveh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gkwytxxfv.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gujyyyxpz.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gjagiebuv.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gegxvzkgl.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gizxtrtiy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gklwftrlw.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gtmlzfdrk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gurahjgiu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gydbvcupy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gpldbaxcd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gdkakgomw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gxxkieify.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/giaiaenly.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/ghyrveutc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gwqetlvdb.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/ghowivqka.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gsopddxea.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gelzrtwvu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gzpbkqwrj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/guzlikpjk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/ghvujrrlc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gjxwexspd.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gqekggopy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/ggsshwbwe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gitruzhpu.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gvrblwfie.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goezvlmbn.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gqjhapnph.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gyfalnkjz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gmgdjvekc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gctvabfeg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gqglwyave.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gprgotrtf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gkicjzhrb.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvywbfpwr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/graydokei.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/goymvpogi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gyuyrfzcz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gvwgdombm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gtgaxwhow.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/grwtkvfzm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gcmziswfs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gtrslvmls.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gtgowjdbv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gqlhvifdo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gpsrnyhto.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/geaunhxsm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gndavwbem.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gasqcwbpq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gepdsvxdy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/ghjhjwdmr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gdimkcwau.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gwudshfia.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/ggkjqcysy.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gmmdmwcjz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gnzzczfpm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/granlbzcl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gjhaoknoq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gkidsctpb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gxfsvuwni.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gqmnleqmw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gzcbnceed.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/ghlvrihfn.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gptotbgxn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gkyjpyygq.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/guhrfeerx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggdrdiihr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gawmjvwij.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/grinzqqtn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gkcyxucgh.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxxlyncnv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzcgeqvad.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gjjxhynkc.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grglkjnbw.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnfxihibm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtvifyyqh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwgvvbbmh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gnxddetdm.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtjcdejuo.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwyfgazsd.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gutbwgufv.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/giekoqigb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/glebxfila.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gcytlsqnq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/ggsifstjv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gfjxrbaoa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/ghvqdafgn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gljspobkg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gqlqiyngt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gwitxbbpa.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/groiwylfy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/ggdtcutdo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gdoavqmyg.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gxotgfuil.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/guwnmxftm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/grdaqgwhq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gnnkjfloh.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/goqdsgucu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gjoysfdfy.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gsvlegvmj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjaqfjnmb.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grqrwploc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/guggutlry.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gijvfwmib.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gzgwtmmfe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gkthhmfpf.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvvibjobi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gbflkgzrp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gderxxbrw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggsrrlfns.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gugapuwxy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzlfutumx.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqmfcvizk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gxskcsmgs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gonaysyoo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gyachmyax.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grufutbez.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gvysumnya.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gdlfososg.sHtML


<!-- 参考信息 -->