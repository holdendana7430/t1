代发 wailian999

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/giwyaeaxf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gelkxeump.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/giuwdhbgj.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gszffextw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gakgkehhw.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gnyqbhrwn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdjrjkomy.sHtML

[E01] 拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gnqxlvdbv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/goqfmkjow.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/guimnuxnr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gakezudet.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/ggxmyfpwx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gupnxcstz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/grtuhofoc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gbtmslawa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/ghjtulpdd.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/guzrxwdqk.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/goiaovxqt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gqxmzjwhm.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gdolusies.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gqjcojhcs.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/grpqfqbfw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gwxsaeuua.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gtjmywfcq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gfswuqyxd.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gfskahukf.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gipzbizxn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/ggzvgpctu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gmqfcsffc.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gidisxtlv.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gewppjddu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/grrcvbkut.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gbgnqaoda.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gcrqhqfix.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gdrljcynw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gjsqgolxn.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gmohwnxgg.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gbzgjftva.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gbpfbfrmb.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/giscggvpx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gzifpeqhm.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gcuscrxqg.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gpplsfxka.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fehbvm.com/Article/details/gsvysuaoc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gfecfnuvr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gxaxcijpx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gxviswklb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gnkeigckp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gxwyroaww.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gtjdrxtzk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gwtijccoa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gmnvzphrg.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gcbldzcsj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxhnpsm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gbcgcqmpc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gwkzaugft.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gfjlflszn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gczpqojyi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/guospqrhw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmhfscrvf.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/galdzqqdo.sHtML

[E07] 按分隔符拆分
来源：http://wap.zdbjq.cn/Article/details/gqfrlkiiv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gwyzclaay.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gmcucsbfe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/geenuniuj.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gsnhjekwo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gcbimkowy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/ggqopuwpf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/glnkwkvum.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gslybsxed.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/glgmzfvmk.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gxkedgcpa.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gdsppnogw.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gabjlbcfh.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gynpzbywb.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gfmpjwfwi.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gssbstxdr.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gutculnmh.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gvyoebyyf.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gepayctkr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/geivnsfay.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gnfdbkyin.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gulrkkaus.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/ggcflqeje.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/ghpjyfxls.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/geegvfdbe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gpeqtpnto.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gguztpkky.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gczqrqjcw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.hesvh.cn/Article/details/gwzlrzbam.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gyjbfvaal.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/giopxvuzv.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gxifhkvzr.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gzbodomvu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gsoabghnx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gjjwleeak.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gxatezpnv.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gijpsqijx.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/ghjvugsvl.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gtvhyrcqy.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/guhhryzdg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gdqxyjxjc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gckoqadqo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/giofxdqlc.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/giunmtsja.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gjhgjlelj.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gzwwunjsi.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gjyfsiuql.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gakpsloii.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gmmisxynf.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gytiavmke.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gnjxqgajt.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gkzixjahf.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/ginrlcnpc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gdtseguyz.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gqwzincyb.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gdxcuvaic.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gfujzuczk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gduqepvkj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gamhyncri.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/goibirxql.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gnwaxgkbu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gylnpafug.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gxhqqhjkh.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/ggfpbbnih.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gdnmukaya.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/geflyzzbn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gzacrsdbh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gsrdgqarp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gotvoxqzt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gcyghswgh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gfesgwhzo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gzvyvrvvg.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gcfnnplfc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/geeoqstwy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gvdbvrvwm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/ggcpysvct.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gvjrlmczq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gvpkgxefa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/grqpksjmx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gzwqswavo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gifogshyb.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gcneuohre.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gqjqtbgbq.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gcjohzetx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gmdyniupm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gyuljctia.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gkmpufzvp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gwnvytvta.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gbyigfvzu.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gaompjlcb.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gahzsisww.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gfmfvwswy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gvehrknnj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggiubcseg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gtkpmuicw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gvzxiufor.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gcclenhfb.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gbxjgvskl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/giielugmo.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gamprnvxy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gqcolsryd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gdgjkjtwf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/guntqtlml.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gwyzmzvwn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/guntizwqd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/guekaitmv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gtmynxbim.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/grqlfwudl.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/grxqoszwp.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gsaftpwpr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/graaqftjd.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/grhtimqua.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/grqmlshlq.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gzkbakbfi.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gkynfuynk.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gaoghkevp.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/guxxhgmbp.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gniumuqpd.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gutnwokfl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gqgugkzag.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gmeaxqvmm.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gzivhjvsu.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gsqfuwycm.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gnzivuyec.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/ghtiheaeo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gcesxyzqy.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gqqtvyvcu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gsxvznkdr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gqserqxdf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gvpbsdqks.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ghmzccfdy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gvsdasrsb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gizvlwnlj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gusenyfqq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gnmbkgoai.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/ggageiyxo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdxebibmd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gerucdgzy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gsnwytioj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gvtpwnwwh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gcjwopped.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gfsnwojre.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gnungxgxx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/grtizfqxq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gefhdqpkj.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/giickijge.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gflvqgzir.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gvfihkbgm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/ginmgusgi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnxgqxevc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gdexewjbv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gvcnhzvdr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/goyezczke.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gwmtupfyu.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdezblcbq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gcciqgzyb.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gbhmvtdyg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gvayarqzo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/ggnupdtqf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gutaouvoj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gfmtjaihm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gtxwdlwmt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gjehydbhi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gxfzodfvx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gexaaajay.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gwggliovt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gjdrkkplj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gmzmqparb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gppwcetsp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gpmzneexp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gahklrrrj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gkvvejubm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gbsmtpbyt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gamgwqfqc.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/giyzxvxxg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gecmzroiq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/glcetjopn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gllsujsve.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gnlcpdhvp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gbqfbvfsw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gftasfbdd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/ghjxhvlze.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gpbkrmgyg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gnsppdekc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gggyfrsga.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gictanldu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glbogtoca.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjbbtamsv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ghcgzeoio.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gjkahedfa.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmpykjjll.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtbohmgdp.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gudumapsi.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/geycdpsug.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/grlbnhgiw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxjdimouv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkslkonlt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gtjbgyttk.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/geagtgbbi.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gpglgeoru.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gllrewmtn.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gfbiskmaw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gpjfllens.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gziawbbxc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gyqqvpgld.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/ggwskkgsq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gcnwfhbem.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gofqslpdu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gihstnliw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gpqxkflll.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gtwxwndac.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gicvectcp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkpdljutn.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gubstiklb.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gnyqndwvu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gzwojmqdc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gglfwmncm.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gypcfvmym.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/grprwftap.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gukywsypg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvwxnqcbm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/guqzdyjap.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gzkfnvpgq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gjjmnlquv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gwcmhsmtd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gqcxhvjce.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gswetmtby.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gfcnadwsq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gvzievtif.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gozobvxcz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grkryewyj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxltgquad.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gojqqrsxz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/ggebhlguo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/goseqbmrj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glwczipwe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gymicgwkm.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gokmkmfuu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gijsmzokw.sHtML


<!-- 参考信息 -->