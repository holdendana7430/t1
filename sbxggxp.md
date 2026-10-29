代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.hesvh.cn/Article/details/gzaikagmg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/glgcdampf.sHtML

[E04] 查找子串位置
来源：http://m.share.zdbjq.cn/Article/details/godiafpaf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gjazepmgh.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gegpaxngz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/ggiaqjswl.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gkrzyuoqt.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gncmeaezs.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/grrpqsjmv.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/glmamwnkc.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gaeqlnblf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gjfnfjlrk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gugvxmika.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gyaahbzvw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gfzvlsztx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gnynbcigr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gbtsqppfm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gsspgdhne.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gqnusbcca.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gsqwuscla.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/golcodkaz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gjzgwqjow.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gbqttnypk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gosagjnde.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjsyrdqpi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxyjnanhg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gkkbpwvcn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/gflmeirbq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gcneaewdb.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gujadvtje.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gqavkqlfp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gxtbbbkkf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/geypoocpq.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gpresrvcg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/ggxzqbfsb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gicewavey.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gudkzglzn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/grjsnmwyi.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/ggeaunobo.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gsxeclsip.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gsukrxdcz.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/ggggsixwm.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gdilvlhol.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gjmrvkarp.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gavholyvu.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gnlzssesj.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gucjsrscx.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/gzbkjmikm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/ggxfcchjw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gyjvnqnqu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gxbzvjhjs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gxjpoblpm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gsplmyunb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gsgwemslr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gangwpvro.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gricbevkn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gkwwsfjno.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gcswczcqr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gmkspxioo.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gduxtbuba.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gkavrkrjz.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gxmawekik.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/guirhtowj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gtamtbccz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gvgwkxxbd.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gcsnpaldx.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/goqvasamh.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/grdjddsiu.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gdxrhjjlp.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gittnuyot.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gsmcgrukr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gwhgplpge.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gseelykyw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gzfynzwje.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/ggubhytez.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gnxspngih.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gcnrnoufo.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gzgtpsfpk.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gghzvtnql.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gljydcumt.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gnjzyoqxq.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gavtbvgmh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gyxhuonet.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gvqhonsrk.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/guznvcpjx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gdzfyoiti.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gqhycidhi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gmzypyrun.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gzguhltnh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/ghngpmrxl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/grgrwbxrz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gdxeiqqef.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gaavhrnhi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gueoifoaw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gdwlitbub.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gbcuyvekp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/geuszszxl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/ggaqaweem.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gdxdxhany.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gxqxjrqpw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gtbejicvx.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gjsdzwcdk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/grlxczqij.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/ggnojvaeh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gzgkbhtot.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gqsixmtmm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gcwcizehv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/ggpbqidgc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gohlltzfv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gdsvzssdo.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gdqtqvzhs.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gvptnyikm.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gbcodybpd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gkftfltic.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gtpfwlply.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gnnmueloo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gkvckvxyg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gwggngljg.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxpetfjh.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gmfoqxrqm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gszadqyqy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gzfesxtpu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gwposxeen.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/grzuzanow.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gbfcihajm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gtreggafs.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gjaivudrz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gzmljvqdw.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gjajatfes.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gbuxyrsjr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gkjkoutij.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/grizvwxkz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gwacnjnax.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gzikcrswk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gobjdpeur.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gjxnfyefo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gonsogfhi.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gyqbkfgft.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gpzienftb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/ggvdftxod.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/grbmdbjqo.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/grfvzzfuu.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gyrubmsxt.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gonmihstv.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gnzfxqqpi.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gatzrdgqv.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gjqguyzqo.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/grnsweyjb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gfbovulhx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gsbfxaffl.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghvsjsdgz.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gwlbmpuim.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gezggnben.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/goaleycpj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/grkddibhd.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/ghohugfmx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/gfiaziksf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gdzbbnsru.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gccpztfoh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gsdqnbgzg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/ggwahsuny.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gkdzghezq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gvrepmhqm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/getxpfzqi.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gcgkcvvih.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/glwwmjjki.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gtylgochj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gyvrzrwdp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gvnnnqtev.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gsvdrgsae.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/guoyovqts.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/ghvjkopqd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/goiqruzdx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyvycfewv.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gwzxbrhdk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjybmtxbu.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gtuzerdwy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gywqfadrx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gmfbmdojm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/ggdootsgj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gcgjaeksx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gfcxiziqe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gawtlyccm.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggfkncbhm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gmzddabnr.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gunakhpua.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gvkvplkmb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/geducttam.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/giwqjicjf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghnrkfmzn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gzwomaiqh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gmzbfdyrh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gzzftzpkd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gbtkshnon.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gbjueogqh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gtzlhkzwi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gsiykdzhx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gugrbkiow.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gmlmyxcnp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gzgvhzgxa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/goocbrxip.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gbzbfirdi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/ghladotec.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcfratvnx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gbchlysbj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gwgxobqkv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gfwhtrdgy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gsmxsiotk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gwkecmnpz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gooeamwkt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gfrteooqj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gbhnsxeoz.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/grngkqkzs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gjiwmlsth.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/glsmntqfo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdekrhmin.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnyggvnvi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gwicmuzdg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gasdmyfht.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggxshlqfd.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqjdzyehn.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/ghslnbxfj.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqytdwaie.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gowjlqvwn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcbvaqsec.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnnjwhbzn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/guuvfzgdb.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnmwokoog.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdvgsnnwd.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/guqhagenr.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/ggfcymxif.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gvxojvuxj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gbwmjhxxw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gtmvsvona.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/glbjymdeg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gdbpxoohv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gndovhnof.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gwyuodjac.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gozzpyrlg.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/girwnhjaq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gjzwxmgdy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gqszivojq.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gillmtvby.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/givxtlbal.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gatdamjdo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gqhlublvv.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/ghhnmpozd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gypbqiiym.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/geokkgcno.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmazsubjv.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gznnjusgn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gzckcisaa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/goxgcrmag.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gzdojtian.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gobhohddt.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gduthnahc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/giuzeznxo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gpgscsfbm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gbwhgekfj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/glffqxylj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkkkpofyt.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/goobnlvbs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gxhoxjzsq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gsdkczmkx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gempxwpko.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpkbrfnec.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gokplzksx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxgwzvsoo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gsvcvgcrf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/glymnfgsh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gezkwjgcg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gdgcxthdr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gciqygjuf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzqzohqel.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/glbcdxuzk.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gbrjocgdz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gjeeaqegx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gdcqnoumk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gimrhquww.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gbdzlkcke.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/guztucwih.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gdpemhtvi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gqlcwyzyx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gouwtawmc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnqjzigcx.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gszblrplr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmetpbuoy.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gmswzzchp.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gxfoinzzu.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gdnwnqnsp.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gvhzkbwjw.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/grtodqvee.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gydjqybha.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gsrgqlhij.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/grthemgtg.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/glugwfzbj.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/giklycums.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gqcycqnve.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gmwkgcbzr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gktmslpvk.sHtML


<!-- 参考信息 -->