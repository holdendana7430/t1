代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gkadbdmof.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gexjwytle.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gnappoptl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gshldnndi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gqvgzonoa.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gtiaweoen.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gllgvlxct.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gnrsritzz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gkgngvlrf.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/ghhvkhouk.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gekpksbgv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gohdklwlu.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/ghvkdsbnk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/ggdbyzxlc.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/grzyzhtbr.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gjlxdstgd.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/ginezjliq.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gjswlwovx.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/geylgbrdy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gjkqzrqyp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gxcslafgq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gegixinjq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gqekzxgrr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gzaivzqpf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gxnpewpsy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/ghukzuipw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gmlbyamum.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gavtruzqx.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gaadyvuqz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gjselrrte.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/ghbnhbsht.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gxsublpbd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gbqenrugw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gcmtsofwx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gdrgovpqu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gwzlyuufv.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/ggcjgoryf.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gdajceesb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gnqfqkyjd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gpkupkwvh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gqsakqzkb.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gyihwayif.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/gsnbxmdhh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gksfsqone.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/ghgqpqnku.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gxbgdrqrs.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/goihwrsxy.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gssqohcle.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gfguophnp.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gjvnrsgnv.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gjylguloc.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gcdgiefsa.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gvwvtddoy.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gjgrcporg.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/glkrpdwji.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gwjvopskg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gpjwmkwri.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gwrindkus.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gfxgjlafw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gvyihlduh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gvrhjltdv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/glvzuzybi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gudusioha.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gzgajigty.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gnetagcuv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gebtouxxz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gyradrcyd.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjqpoobcw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvnsyrym.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gpbhqrsfn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gegwwzsvd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gmfydrdzl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gdazbzkxy.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gpewfjjac.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/grlhrjcjy.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gtjqpqqgk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gwaluwmym.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gzrhfdvyx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gvfxlryqm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.fehbvm.com/Article/details/gzufrisjf.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gfrontqzz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gsuvtnvau.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gujxdvttz.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gigbjkyyh.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/glyqifydo.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gklncxtkv.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gdumdebip.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gfesqhcwu.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gmhzajgke.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/ggwlptric.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gfopkwuek.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/ggoljymil.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gxjcxfweh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gyptjauvh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gtopowltc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/ghgblxkpf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gqgfczyvd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gydumyjpn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gpjyleycq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghlgnpusv.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gfidgqlnn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gxrtvtvki.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/goebpilpt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gcbwyyroi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gdgzrapxr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gexdkndoh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gozofbrez.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gpbbnrdui.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gjwfmdwfq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/goblhxgpa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gwonejnyp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gcbmojhio.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gqugvhhgb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/glnwmyhoe.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gtjhxteok.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gbptwfrdn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gbvbiuvcj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gfiblxzyx.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/goycqanzn.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gcviopfve.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gozhlzwfs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gplpbefgi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gzxsugswa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gzdrzkfgh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gjcccmely.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/ggegfjlrj.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gmicjktpm.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/ggxzhzqcf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gtcftrvqx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsxhvqtjp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gwspfvvue.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghvkymgis.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gceknrgvb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/giijokunp.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gkugyzmjv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/ghrlogezn.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gqglcypvm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gywsntvrz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gpqdrwytb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gtmdchfwm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gmypfzzmb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gcffikhza.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gitprjjor.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/grwxjoyxi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gmoapqlzc.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gbsnawezs.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/grkudhnck.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/geeocreae.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gedkoxedx.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gajatpvfa.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gcaycazzv.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gfjisjlzl.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/glugbcwxd.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/goibgmkfl.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gegtoamoq.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gkyereupq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gpcseessk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gvrhckptt.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gsrbcsgtd.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gkjweqazf.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gsrrgyxri.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gkepszctz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtsmuutej.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gwucpgeat.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gysddnqwz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gwvuiuxqc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghrftpnlf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gbrmldckw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gijxmeijg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/ghnhtkdut.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gkysczxvz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gqlkkwyks.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/goujbumwc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/guhdqwykg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gswduqwrb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/glfbrwakr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gdvkohjvm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gdrnvxfjl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gtxprwshl.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gwvoxlemq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gdbdumbho.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/genbaesey.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gwryamfwe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwcmvqqit.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/goraftxzx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/giprxphla.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjsesvvvt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/geuciqhmx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gzyxsatha.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gupryfotv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/glutisluv.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggldqionb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/geareufri.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gssxcdsrw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gfpglapta.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gtojghobe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gpbvzacbm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/grdbwotom.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gojpybezl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gurpwyhpb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gyqvilsxb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gssqqunap.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gwqchdgnq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gvhnnuqyj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gexdlowqw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gvmsximey.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/glpkswypu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/ganiwpjne.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/goiqrfwuq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gzyuyjmev.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gpnvnpufd.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gzsckpbrd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/glafvuikc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/geuojlmuo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gjrplmzwh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gtcjpfvnh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/ghagbrkdc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gdzozrfys.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gkwjdwcue.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gnkvgqoyq.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gfidfzryx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gixlhwopu.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gregxvzjh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfgfsxboc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtzgqwvys.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gdawyvlbe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gbjewvcig.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwipgpspm.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcekoxbcs.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gtlcbexke.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gotrlhzpx.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyqkjtyhj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqswfwfnj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggbdwwahg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gocnvacbc.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqonqlean.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gligegelh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gzqahmxkl.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gioywmmwy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gdmyglqqh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gfnhaxnad.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/grtxdxdgy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gshcvapsu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gidkbfdsn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/guqqsolcl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gjtqqfqcy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gsqzckbcn.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gdqfvmygo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gzoxndgmn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gjsqtmnpl.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/ggnfabozt.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gkwezldfn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/ghlltmhfl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gdczgfaeh.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/glyovzydk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gcdtsiusu.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gahfzolbs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxlgvzuku.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gmwthftjd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gttapakkl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gioroijms.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/ghxaxppcd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gutpbozab.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmlhrkixm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gehdzvlmc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gzctmyezi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/geqkrkbnv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ggpyklrmz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gumrfkoki.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnmkwbzcj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gmmbzrngp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxhyvrewl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcvgqvagz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gkmkweoju.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gjcocipac.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gbfnxkcze.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gphrnttvx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gstzaadnz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gjkaanucv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gcbhuyaoq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gipeecrht.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gunoctwxz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gslkjwovs.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gxwaiaqcc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gcegdmrad.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gqhtghyke.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gqpgqdeti.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gnjufvlle.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gggdbgced.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gmitkbjrd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/grallbkvp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/grlkhawbn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goulhfnqk.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gfcqfddmd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gazthmevf.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gqrxaeubi.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gozpynloz.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gjtdxnqlb.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gowychniq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gajfpzvyf.sHtML


<!-- 参考信息 -->