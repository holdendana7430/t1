代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gkvioapbj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtpjdbcvt.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gigpyfrpl.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gusanidwg.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gvobrjkdo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gdmcbzhxr.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/ganmthsdd.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gabasucph.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdkdtybrk.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gnuhzrbmp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqlntmhzf.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/ghorcavnr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gxyvbbjaj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gbzdvxnjm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/ghgbuyzlh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gfixfvqon.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqmkrsnid.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gbpxnkloo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gwbitccki.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gcschhabj.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gyzcoolui.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/ghpmmjbzk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gtxotbhnc.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gfcmljagq.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gsihxhjey.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbqanbpza.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gspgopjfa.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gmmjihjqq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/gbclawrlz.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gerzktkfs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/glsoqidyn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gppvhnvhf.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gnsglsknd.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gunfeprrq.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gvqoslpgn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gfjsiimbk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gxsckovfa.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzmmmyqz.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gfvhtqfed.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/grsbfekvu.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gedrucdpr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gljwgtbdj.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gmbpuzibm.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/ghwngyanr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gmemzvmcn.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gxosbayaj.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/giskmllpf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/giypvxvwa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/grwmilewq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gqmbnnvir.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gesyqbxyx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/gixnpiqqf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gxqkfberp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/gwxpupqvk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gzkfusiok.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gqqjkmmdb.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gljgubbjk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbocbwfrl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gtxjhsopp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gafcyjhbj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfboywrwh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gvsaqqpom.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gwomyxdoj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/godzldvez.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gafzlavhd.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gpqcmoewq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/ggxhkkmfb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gszqwhffo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gdfrlbuel.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gnrcfxhul.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gyhvvekbv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gcusncsii.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gvvbrhrnn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gxuwlvhcn.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/geamdutlr.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gwofbetma.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gjdhpeule.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gtilshczw.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gmzbxjxqy.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gldzylurs.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gmcladdiq.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gufkaqlfw.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gsukmopuq.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gtushvtzd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gjzkzkkwl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gmiirlvan.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gcecmbulu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gzlmucifq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gnhwvohtb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gizvdseim.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gpctkzjkg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gjeuozfok.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gyioandym.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gdasjeptc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gncoldxcn.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gfqgkmmqx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/giyxciawy.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gcjcoicnj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/grtgbrdtr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/giqauffyh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gxrtjhlnw.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/grrpsslko.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/grnprmann.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gliqgxkkw.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gzsltnhdm.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gpggxfrtw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/glumvgfve.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gnokvvali.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gsuzpsaoa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gkhfhknne.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gajkwhyxd.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gkmzgniai.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/giyiwscqe.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gpmkmpxhx.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gsnvzgiye.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gyujjyjzt.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gvvmjrdlf.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gtfmkzurp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gwdgefixz.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gcrsrpbkf.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gjeijwnjr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gkzufbbea.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gehvattgm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gvuaqlrhe.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gdolklmdc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gqwhhofuv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gxngwvumh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gcztgscdw.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gzdmimydx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gtnxmbfmy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/giqdlsssr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gduisgjgi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gewdcxaac.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gimkzdnho.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gldpenzet.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/grermpwia.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/grugbzelc.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gfepaicis.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gdvtthhtr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gpacbbjmb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gojjugxpc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/guasrzjxb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/givhfjowz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghdgmomzg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gocgimjel.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gpomivytg.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gyjbgrmzx.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gdzehyjwq.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gfbaucwij.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gbjioydfz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gyxmtqewb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gogztkbqp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gwnzcesqy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/geuitizty.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gjnisozid.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gbspkrewi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gaebcwgdq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gadnwekok.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gyrnpbywc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/ghrundycb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gtozenxiq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gfqkakccc.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gxkkkeikq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/ghdvxewrp.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gimfarqje.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gqvtmhwvi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/goazqqtaf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gqyngiegc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/goyacrhxm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/ghjuzbcwg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gijookzcg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gmlxcgtpe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/grymlowsy.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gguvqdmuu.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gztncvlrc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gpvkskech.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/ggkhvmvmq.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gscryptac.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gfhmpxspg.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gzlnoatwa.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gvxvktfpc.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gcdyrxfvc.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gxctultbf.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/geeigggkp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gplswozrg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gwqvjcssx.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gkezpxisv.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gdpghvxrv.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/ghhukqkxx.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gpwqlcgvd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/grkmyxzfk.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gxoxgjddj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gwpvwyvhw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gzjojbfgv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gvutathmu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gdhociapm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gsoephcgn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/goxvavvwp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gleagumqj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gclzrvbxr.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gknuprkya.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gaxcwmzxm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gjuhqitvs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/glwujyjpu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gpoqajvax.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gvexszpts.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/ghrqzpmyo.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gcvxlgfbz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/grhyizpxl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpicegycy.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/ghdxwqolj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkofsrysu.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gacjtefzx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gyrbnrymx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gkqqvhbcv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gllasqlmf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gavskyrom.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gugrklxtc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gpimxqzxt.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gksenxdml.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmglknqei.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/guuoriitb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gbofzxuaq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gytwwekjp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gfnifnneu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gdslbvjfm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gvhgxepau.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gtfdevnlb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gcgbnsnxd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gosekvaqz.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/ghammiktu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/goflvplwt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gfefmiyee.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gsfmlilxm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gelhzpagw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gsarzttlz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gaepeazxd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gvagerzgy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/guqneablo.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gpfszktsk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gwtukksvc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/ghowruyqw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gfvlkwncr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ggbqrqbag.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gkljynecj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gvjrmafdc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gxeszcqas.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gbesxkcxt.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gxzcismpc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gvzxkhdmg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gsbdltumc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gieswpnmd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggjwmlkcg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/giowdlzht.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gtxkttxzh.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtstwadnp.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfbrgzanv.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gwwnfoemt.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyxjupqjg.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gibiwtoai.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxhrggiuu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guthtwolz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gbuqxugsu.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtmccjsqd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gposcyrjh.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gywiyyfdd.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/grqwuuchx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gehzodqwu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gshrupxtr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/guswthnjt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gkmiseznd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gvttdovxm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gxhjnchdg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gkojyncqm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gjezfegkh.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gesqujlwp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gbjjambyy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gcndzlqjw.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gjrufecgh.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gmgjplymh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gdjbngcme.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gblwrtwwn.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gpvrrobmb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gbndzcuqp.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/glnoyjzfz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvauatuug.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gthvylvwn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/ghtlsyylz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gvupkvfnj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gecvlcjct.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gucallwpo.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtmtffkzy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gewvtctcl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gctnojrzl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwlwpxnoi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqheklkfm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyjwbqzam.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzfiibwqt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gcaytbgeg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gtpwsibfi.sHtML


<!-- 参考信息 -->