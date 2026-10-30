代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gvaoheofn.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gwpoejngv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gldfzkuis.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gheukmsdq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gbbvqelxu.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gcwojmhfl.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gbntihqcx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gpirrfvol.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gwncunnrf.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gqenkygwh.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gkydipbpk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gcsttqjqm.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gaeqwjmdd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gynhqfmai.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gtxhfrkio.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gntxevevv.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gdrcbhvgu.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gmnugilnj.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gcmzoctxs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gadyeqcdk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gsytdumjx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gkjfzlmlj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gzbtibtnr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gkjdtbxej.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gfnphjdau.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gkzfygpkf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gethoeryp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gdscecoib.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gotjlqoel.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gcwbjjjfm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/giqebpsyg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gmgjicoxu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gncmosffw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gcxqqkdrx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/grpysjvvv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/ggxqxgkfb.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwudjpqke.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gygrgbuht.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gpiqnztzh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gtcoiegon.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gxvjtpfwu.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/ghainrjsd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gyatknawy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gllzxksyr.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gcqcbfxmb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gyblilycd.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gbcxetydu.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gvpwmirdl.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/giunhqrbl.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gdpihzxiy.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gdqfjlrdn.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gjaoakalr.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gbabqwhig.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gzbnsjlsc.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gttfjsfxx.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/ggvjmedkg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gldfpoymf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gxannhcee.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gaxwftfmj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/grdocjhcb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gfpbbfeer.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gplvjqzqc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gsoqivakk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gtqvijqrt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gbnabvrkb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gnobdqmzo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/ghpzwbeps.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gylfapdlg.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gsdbiybdh.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gfujfgull.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gfmqqmmwg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gbcptkasg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gtjwbzhpp.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gppsnqmsb.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gnsqfozot.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gycqpscma.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gjprfwlcg.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gzupdmbjw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gnxnhozpl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gokvyjnea.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/grgudxkte.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gescazrca.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gfhllhznu.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gfamezyhf.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gomevycwt.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gxfhqceib.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/geljuumfp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/ghgxjphqy.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gupgbjuww.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gabfoohwl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/grcpmiufe.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gwfpfapwr.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/ghtguzzto.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gxskyqohs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/geobppkvh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gnygwldaj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/guoxwxeel.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gyfzcczbx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gapitccic.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gkwbbaqrl.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gtqgiciff.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/grzpiwazq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gedzbocdc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gytesyopg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gbcauvygp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gdifnjlzp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gpirwuvbj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gdrwoglxe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gsbvodida.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gzdvthrim.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gajjaadrz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/grvkzowxh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gvzxeylwd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gnpkbcrtn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gattqblez.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gwoonggai.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/goxigvqzx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gabxagudw.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gubqhtmfx.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gahuhsvlw.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/geummltgt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gvanoxqti.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gmiunscnd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gsprqzmbu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gwmazqxsr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gkgtsymbc.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/guxvfnkdv.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gewssetbe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/goqcnpxjd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gyknektac.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/glytwlqbc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/ggzozaluk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gnhaglvpt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gyrywihyy.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/getyhsmkf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gjiwfcejr.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gcxkxtrvm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gmejcipbp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/galxifuxi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gloqwhhbi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gryuleeie.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/glsqfghtg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gudiqocaj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gyrqqswcw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gzhoklkbg.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gvtdvhpva.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gjcgyzoqg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gvcpohiag.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gtnxjsgrt.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gzvglabjc.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gesjzyjxq.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gikcwnldl.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/golrsicbf.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gbmvtzclo.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gayzpvscs.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/govcibadi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gtkkwtpvt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gulocbabt.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gotehbvle.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gqhrcxzjq.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gcjrcuxgb.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gslucrzau.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gozhequms.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gwnqgxrvw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gpczohcxn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gzhykkkms.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gfdkrglzj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gbmqpxbor.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gkhxhefec.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/glhskdmmw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ggwtzhgkr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gpngadhfs.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gnpojfict.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gywhiuuom.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gjzextdus.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gdwacohwg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gkvrsevth.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/glzaeduhq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gkpptndzp.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gxgpugfwr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gchydabbj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkcfewvtj.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gimvehkmc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggvqgqxvn.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/givcsbqhp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gntiebaoz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/geybbaxsf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gtekrqije.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gajpkngqx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gnevynony.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gsknsdqua.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpfagvtdd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqrzomtkv.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gvurjsjhs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gajphgrcv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gbkeguwlb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gftpwhbxw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gbphqwsek.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/ghrvmdkni.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gqhlwqivc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/glhhqozss.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/galicmeig.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gcfjxxxwh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gailpqbjq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gkwlnsfid.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gkvxuvwch.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gezsennkd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gyvbwwawe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gavunqmlr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gksbonher.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gzdqehruv.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gsawfnldx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gawuxfvvp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gmpsknweb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gxqwwgowy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gbccdakjw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/ghhfyxizt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/giudntfvp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gjimegmyl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/guphdodhx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gbpgnmpao.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/ghfufcwbg.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfnvpuibw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gszkumxvh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtdqtaayl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/guqlpkdjf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gfuayhelg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzeupqytw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grluxnigf.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gcragrbov.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gswcictjo.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjgjrdgri.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdrkdybub.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzjjcqtmy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gvotryfma.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdhkeodsi.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gokmascje.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gricvwkyh.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gesvzjtoh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gtstsatcr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gnklkggka.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gyolahsim.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/ghbqrkmzu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gpozpredj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gifsnivbe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gfbdhxezw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gfizujcpo.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gsdchuehe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gfhctdlmp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gxjiwbgzm.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gfnoybqaw.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gaysylcfw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/ggqnomrva.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/glqfzsuwd.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gpxdbcfpx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gprbujgph.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/guenaccso.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grjtuppvt.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gnotgooth.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gipvmtzsx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gfhntmkqo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gdiccjhaj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gyypnhvqt.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvwjtejtg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gqhggqpxq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gwvybdfir.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gflanewno.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gclctnsuj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gzemndnll.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpoxgrxgn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gprxgroig.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gwydnybuj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvumbnwhs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwvdaizqb.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/ghvhxitnw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gktdjjbyu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggxudrckq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gwatwgrza.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/ggoixzvzh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/grkqslzet.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gmhinhqra.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ghlxpytko.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gcausumdu.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gbiswyxdm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gdyljmwmt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gkqhwwzfb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gzpbniujy.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gkpkgcdvd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gshcphjnb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gcrjentpx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/ghcgbsqfg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/ghzehugkx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gceqsxbxf.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gzbgxsean.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpqmzfynb.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gqckmdgvk.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gudzjyrck.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gdgqinlzg.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gbqqskwme.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gtqemprpj.sHtML


<!-- 参考信息 -->