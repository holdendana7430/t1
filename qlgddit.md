代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gmilkscqi.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gwqgniopk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gpszwomrr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/goougttgp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gejhjbuqt.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gqaruzpkp.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gnnjimpin.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gvgaayrdm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/grczpvodl.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gvkkixyfl.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/goufvjzej.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gouytuaqa.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/ghflqhpur.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/glmtqgrdf.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/ggmvsmmir.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gmidzzqis.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gzdqxnvau.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/guhgnccrp.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/godmimdkz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gdfiwgyrw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gmowtrexf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gemfxycai.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gmetbstrt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gzqlgowun.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/guzqmocxp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gqbrisffq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/ggufzcbro.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gihmbhljz.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/ghdyqosgu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gznuzhgrk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gxpuwgzjb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gewmwmyxi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gitxldhuz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gmzgrfgrd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gctkpzrat.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gpjkuwsnb.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gjxvehzfe.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gfqzyymkf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/greibuwvq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gezpwggbm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gvzudxcsi.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/ggpgwqrdw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gfbqmlscv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gcbryrvwd.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gnykdkldy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gxhdabxwn.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gcrijazyv.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gwzqyuqyn.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gzssztwic.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gxpwluvcm.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gddjfrkyk.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gwpiqiaox.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/grvtcpbwy.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gbifujlrs.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gjfeabkfe.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gbdypfiua.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/geshjkwgz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/ganpiloio.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/goxposlcf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gwdusmwxt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gobuvznap.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gavrtdqse.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gjltnepaf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gfzwbafrf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gepuqajhe.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gsxegovna.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/glmqwqwrf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gpvfhffuf.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gdjlnpgar.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gltoeotuq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gkyzfkqfb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/glqmdajgf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gqyxiuqaw.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gpfurfgsc.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gbwyvuvml.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gsrehgppr.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gfpytzxkc.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gfmnqtvwq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gldwdswjx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gcknrnslj.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gmxxvlgvq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gonrgdsiv.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gpqlorubo.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gxlpuybqa.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/glsmvwrra.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gcyrjiobr.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gegjnttha.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gzcududbc.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gllyrtftz.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gulzuxqys.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gihvtfydy.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gesesoyjj.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gwnwgkzok.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gvmfyhseg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gtfyhpznt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gpdzgowut.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gmlgzsfqt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gsupdixfn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gznvhdidu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gkarqaotm.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gnsldjldw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gxmxybxef.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gvhytrusu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/glhglsboi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gypoddtqt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gjklwqkoi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/goopzsrob.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gmfsgoqvi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/grbmmwqsr.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gpijqmiio.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gpcjxhvee.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/giyyrhngl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/glumzidbh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gmakzkbpy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gqlaskqhm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbkfciwbt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gbbotsqmt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gcmatnyut.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gvnbdrhyr.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gtyuedewk.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gmnkmeprp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gxebgpucq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gfevcyyui.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gsdhnadit.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gginkohkc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gwtuugrpn.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gwdkmzhxm.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/guknhadml.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gqssyajsp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gprhqumeg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gsorwbgkz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gvigvwzrk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gwsqltwqb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gqaktiuax.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gctvspuys.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gcpactplj.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gaeppqdrn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gmlaipgvf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gxlwxwxuq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gvyhndoaz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gzkkbcoko.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/galgkghxh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gmmsdxahl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gypvcyykp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gabtzgbkv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/ghynsehmi.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gmofiouxh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gsefgtpcn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gfuisatyc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gikwjdura.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/glindnzbd.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/glnzxwusm.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gmembvuqs.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gdrkoasgg.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gdlsklqez.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/grybobodl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gqchsgptl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gxpoextag.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gypyrhous.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gnhgenbii.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gimueghen.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gknqknuyc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gqwroihws.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gttqbaxum.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gqdabinrz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gutzcjncb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gbtwvztct.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gbpxrtoik.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gkzprykzq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gndoqxmsh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gjgbeqcze.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gghqztmkq.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gdcqsslau.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gvcckuzax.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ghggncqth.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/guwfbhoew.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gftzigbfw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gnjarmrey.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gixyfaqum.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gtuulwnhz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gnfkybcrq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzjequdcp.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gdeqdejrf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gikezozwi.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gzjjcsdiq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gsqkyhwtp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gncpnxhsu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gstmnedng.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gaacmanxa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gbysoslod.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gbzhzuzfe.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guxdbzklm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfwtbiurf.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gbuzvmzcc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gyzqpkzln.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gghyqxoop.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gcetnjikv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gyguzhhjq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gtedkqctf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gnohdqkdq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gzvxpjhwp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gahgpozil.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gniyyyaat.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gbbigezge.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gcmkkceob.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/grjgldslf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gwedgbmum.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/ggyrobvpe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gmfsfkdwv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/glbbrlkpg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gjxabnesa.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/ghcxxpiin.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gccmbkvcm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gkgboedla.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gtccxnejr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gfujppvnx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gnxqygkrp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gvtbjlehl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gmolmojha.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gihrmnaay.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gmjykakju.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gactrcwbr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gimqvnfsa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfdvqibii.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggndxrqqq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ghomryhcb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gehjqmwab.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/giycrlirb.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/glrwskvdr.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/grqcuqrdi.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwroaqcew.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvzdisznf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxkmbsjym.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtvbyfegu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gjqgswhec.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/grvzfcyzk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsgtcusyu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghouontiw.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gxxhvinll.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gtecgaqrs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gqivjtgnh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gmaemtnnc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gzeantptp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gdwrxfliv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gytyubsrm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/glmkhkmlo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/ggvmusyil.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/givcmmnoe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/grmwxqayp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gyoktpifx.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/ggxqhkidd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gqzyrklig.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/getniqypz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gvhpdljrd.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gdfrlycfb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/ghgrlrgky.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/ggrcfdftb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmemqmez.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gsabvjjys.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/ghauwwjwp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gbcesicac.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gkouruecc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/govphkcks.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxcejuqxw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/ghtiuqhvb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gcndnhpcf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gqmeckqkn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/glxpfpiwt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaogtheup.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbagbzusl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gvwjgrdku.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxvtgmtmw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gvxgvcivu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwpwnvcfo.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gfvtiuxiq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gcrkqflmu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmripsfyq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gmkjcyobo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/golgbhzxo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/guhafimif.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gdtealpnu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtheaqawb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gvmpllbjc.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/grwglxbjh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/guzuigtvf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gygykghzu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/grtqrgyhc.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gymzkgogy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gxqzynapm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gohvzpxvw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/glbnuvaok.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gdgkqxrxy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqwrnjtuc.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/ggbopavax.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwmyyehyc.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/goqycbdwx.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/guqsjkeoz.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkpzrkpqt.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gygdwnuiv.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gkdzwtetk.sHtML


<!-- 参考信息 -->