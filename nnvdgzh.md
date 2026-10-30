代发 wailian999

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gqzkipids.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/gortlpdcq.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/goqpvracl.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gdrtziubk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfwtqankg.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gglrzjsey.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdiwfgaze.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gygvaevcx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gsbubhejp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gvvzmtvrn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gahdpbfuf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gcsypwceh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gxyrnnsql.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/guuxpvldz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gbbwhjwuz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gpddttkep.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gezabwhsi.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gqghyxwcj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.hesvh.cn/Article/details/ghmbienit.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gljgtsdpq.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gvmjrwapb.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gpjquobvk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gefcpexto.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gowwlvprz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gemomsoao.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gdiorljpg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/ggofcxjar.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gbpayvimu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gnmzjgsap.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/giqidnchs.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gjwyhmhit.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gzybpcflv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/ggqffywor.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxzzalcj.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gbxybjkar.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/grvptschp.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/ghkpggali.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gveocsbih.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/ghwomsalx.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/ghqxcqyop.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/geudceplq.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gtrjpablg.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gbnemxsun.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gpwttjywi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gnrksvuaf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gydchsmev.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gzcjdfuhs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gqymgamgj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gstjhudrh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gumlgjuil.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gasjthtcg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gfetkcwfy.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gygrujnfn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gvrfwdxdj.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gqzyunubn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gpaowfdfe.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gbisnkuao.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/grutycldv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gswybbzpc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gstnffmma.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/grxrpnvdc.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fehbvm.com/Article/details/gyfxoobuv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/glgifvvlq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/grsrfzbzr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gllrxxjiv.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/ghbfrqsnh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gecpsejcv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gzzhnqmyo.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gcmquhccr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gsrfokxby.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gapygznsk.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gfuzhchjm.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gqyszioaj.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gncokmpbh.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gitdbucdi.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gimytiqxt.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gxhsytils.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gigktkqvz.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gtnjoigho.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gbjhedpso.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gdnyejdzd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/glcgegwfq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gqxwvspfi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gxkcharft.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/ghxbzowpt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gklvouphb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gihonaycn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gguhnvfpp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gjhicefpl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gbmcvmpub.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gomunitrc.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gafxevbce.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gafbxydou.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gaaxidhuu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gbzqihybi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ggtkmdtzl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/ggldenvoi.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gpmsclvtm.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/giraxxxno.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/guptloqrw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gwblvwaux.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gdjmtdyrj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/glzvdquvd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gphetseaz.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gtgmmecvd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gbwypymxz.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/ggxfwipbt.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gxurhqydn.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gulgukcok.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gymrijyhv.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/goritygvk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gcxbbykyu.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/grfwjvhrn.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/ganhhavbl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gzlzyqxgp.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gpdaljnee.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gonzofhso.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gxuqwgsaa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gyblkhkdz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/glqjqeqok.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gaojutwvr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gcshzsqql.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gixipxruy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gqckssesz.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gbvmhmnby.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gkjircjjv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/guiuxcxza.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gfnmgatuz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gplbiwwvh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/guvdpivtk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gqnrhyett.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/glfnxyddf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/glicpvzsc.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/grvosxopg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gvrhjugdt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gnzjrphwf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gtgoekemu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gvqiehiwy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gvnlcwdop.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gszyznkir.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/glohemsvw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gifalsimk.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gdexvlcwu.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gilvbupqw.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gwmskwyis.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gjvfcmpzl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gzbjvexul.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gzpujblnk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gnbvaxgud.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gwgrbaogo.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/grgvaitul.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gkfiuvsco.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gdkuprekq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gdztbybau.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gegbrdzfv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/ghhhhftdg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gssijhvuj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gpfzowmtr.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gmbuyysee.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gdipqkwxs.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gtbqgrxoe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gqwcbbxzc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gmnbtlbkl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gneuosdas.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gexneuggz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gokhahkdi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gslmahtyh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gjfgoywqv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gkzbdubwu.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gshbyxcrf.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gjqnuctdj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/giilcgcrk.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gniqhwsaw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gkzwcvcis.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/geucotcnr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gocugpakr.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/giwrzdict.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gmartchhp.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gvqsjfcxd.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gnrnezlub.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gbopjrojt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gxogvsddm.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnptfrlyy.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/goxujreyt.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gvgmbslij.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/goltgoikm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/getpxjomt.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gwmgsplqr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gbungtdbe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gaemcjuuv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gqjqrfiyt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gjbzvqkod.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwuykojfn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gqmzekeft.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gntgjgfqg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/grhiqzkhy.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gdddyzdll.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggxtozfqk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gvetlprxw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gbnhdtlua.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gfaykcjib.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gwbfkwoof.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gnjcctyzc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gjnbuuuau.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gprbbuofq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdmcwxhas.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/goanbikcz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggzabbpau.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gmqyshupi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gzhayshic.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gpbxktvve.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gykqraxuc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gkmwvqqff.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gfoofguov.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/ghrihemdx.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcumgkfwg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gujnpzkdw.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gqhvamezi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gczlbkseu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gpgqjtmfw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gwsjvnndw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gdcmlzzni.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gfmljwyae.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gjgkkbkwc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gpdtzmeoo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gntwuesvv.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/glmvurktm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gxtfbqlbp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gvewoxjft.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gmiglpook.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gktdzlwve.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gwfsllswd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gmhsfkuum.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/ggcvifyfo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/ggqifolud.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gettpmsxf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gxbrchzmv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gkrhutbdo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gtqaetjyp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/grijcxnyf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gvmzjpxvx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/galhyhohh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gjoahgsjp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gntgcslgl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/glevnjanc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gvquiyaew.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/guovodltt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtvbgqnlt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gobgyuggt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gymnpneuo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/geoxahkic.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/giybbajss.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxzlkjyvz.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gxoolrmwn.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghomyubwm.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/goouzbxaq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gavqkcsoy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gthxyepvv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gwohcwtly.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gofwmkvho.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gscqpiiyp.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gcfwdsrhx.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gzonhwhhc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqtunyrg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gdxwomihm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gaktfcnfo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gitfsvctj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gtsceohge.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gxaxkuqml.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gzjaahnng.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gseqtwjjh.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/grkcrvyrx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gdgvlaozw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gvmcsgutr.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gsjflkbtw.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gkgbexbgs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gxkmdjpab.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gygowtjor.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gpcgbfwzo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gbxdsdpwy.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gnbaoadki.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdhtlgwkf.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gsiimkudh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/glqbaiblk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gggdvhflx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gaazaodie.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gdewznohl.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guyuojbky.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gritpbopq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gzrckfxqw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gplppxlbb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gtmeowdua.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gfdryovuq.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gckhbyrrc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gediswxli.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gugykliec.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnwunfpyy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnbhebfej.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/grcluxlfp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gwtxsbzij.sHtML


<!-- 参考信息 -->