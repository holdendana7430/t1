代发 wailian999

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gwxpbkrvj.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/ghhpgymxa.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ghlmmvxdy.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gpmojgrkp.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gqeihpxmh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gkqdlaknz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/ginwuwhrq.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gathcilup.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gqgimobvz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gyvjcedrx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gesyrvyow.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/grlqvsfkf.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/ggybiygdc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gdwzezcpk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/giwychkbr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gkynxmlgh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/guqiowuax.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gyfjkpsie.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gbqlrterh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/glbpkmgkk.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gpcskuxiz.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gwsncquse.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/ggxlblmhr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gxxmwwhgk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/ghnzwnsff.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gxsixrpjp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/grnszdvga.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpknhlscp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gjndkxpvk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gzdcpdnuz.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gqqfnbcct.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/ghjstffsh.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gmfwtbmqo.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/gskwdiind.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/grcskxhsp.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gfmetczao.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gifaefwof.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/ghecygaeg.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gmskaqgzf.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gdfxeqmva.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/ghmascpqn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/geiggmety.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gyswelelf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gpaectxky.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gtguxniux.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gbihrfoww.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gdlqhubfh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gnrfjatki.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gleskbxsd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gjjxpthfz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gotobxmdy.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gdwnwkzgv.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gljdhtstu.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gffmomxdh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gesxmpnno.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/glzqvduiv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gpdpqebog.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gfizrames.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gealymtqe.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gasjwugku.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gcowuwmdf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gklacfpsd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/ghmhwawwy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gkimqrjji.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gugdmdboh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gggamxedq.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gpphscajc.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gcrwwpddn.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/grlizkhqe.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/grarfheke.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gvkvjbdba.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/glkkrybyp.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gokzmjkca.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gavwdzrsh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gkiwcoest.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gcpafhoiy.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gmlykcvhw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gpzgpsgzt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gmrkqpiom.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gcyjpfdgb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gpcnachjt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gykikmmon.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/glqyuajmj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/glujakkfw.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gecrisqsl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gilghrlur.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gwbqephpn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/ggselxjoc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/golotwtax.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gwtzxpfbb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gmglugsun.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gofyienhx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/grbojjjvn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gfngeyvxj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gmjjdsyop.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gaefjatzj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gexzinjke.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gskbjgewo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gsntsoqrs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gdsmabxvr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/glyqrepbx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gdbfhqypi.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gcltggkdq.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gocroghul.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gnumtlhfy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gklghtxhr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gxypgccjt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gdouigdmi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gtwllafpb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gcpcjfbrz.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gopcwsiyg.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/giievnxwp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gcdjcqnwl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gcxtmqyze.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gtofkbfym.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/glukuedfh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/ggmcupemy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gdtrwnkhb.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gmrcnvzpx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/glqjfoxyq.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gwszrclbr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/geobsdigv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gzdpinyah.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gxzbynjbc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gmzbczulx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gpvmuvyhr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gdgghpjbp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gkxsadckg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gwfghaazx.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gptajeduu.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gtscctida.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gbfxwwqwt.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gonlgvvwg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gontsjtvp.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/glwucxpdi.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gcwhiottq.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gitpxxzgn.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gvqzvbpjd.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/goquuerar.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gooiomwho.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gskiggygg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gdjhpbubp.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gznbtbpdi.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/ggrktisxj.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gqjpitntl.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gzqwgxwtf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gjystmcio.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gxohpoxpj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gxacptule.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/ghaffoazz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gydjuixkd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdbdgujch.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gpsqxeceh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gstgczxin.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gkppqovcq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gkyppowdu.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gmnjyyphy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gamliqbcz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gaglywsoy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gddzsoyuo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gjwwmpmup.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gpbgxeaxf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gtrmnvtuq.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gfvfzcbol.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gxjfmcfie.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmbzjazaz.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gfckxfzjm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqnitfayb.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gftqjjzxu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gvaoxujcb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gyfkyrsse.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gqrpwzrzb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/ggrygsdkk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gsaaplldb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gccohomqm.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghwhlwkko.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gddicdpjc.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gbluhdnvh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/grqobyuro.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/glpggbfpw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gbdyvnvir.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmebyxbmi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gjbflwklb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gnhtrotzk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gmpthdqkn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/garoffljc.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gvjnzknvy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gpqdwmzyu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/grcgezjrk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gwwrqduuz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gjhbvekqi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gubwsyzph.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gzruvbwyo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gcijnqmho.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gdumbdhpo.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gehuwatac.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gypvzkesn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/ghujcovmu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gmuvvqqxs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gkwlnjvgc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gulstduqi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gmrcvqwkb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gpjnqaxqu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gyxioitcd.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/grtvkicqm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gyxxxtxlg.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzbyznzxh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxduatgoe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gygztiohl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gpbeqkasg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/guiriawve.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gacnblrcv.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwnpjcbzs.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gtexpjojc.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gotgrxpjn.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gkpfbzryi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdpvdnwod.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtlcclacr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gvqxvgcsq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfxvjarmw.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtxpntyay.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gzbihhmiy.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/glevvegwj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gwkoxgvhr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gnziqxzkv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/glnoeqgby.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/glmczevhq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/ghysrtefr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gubpsmiyg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gofxuyjmz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gubgzrraf.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gvvzlalgs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gnkkleesk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gwfgmtsit.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gfzyqvaee.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gqdmxsiqy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/geqpneqou.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/ghdvtrabn.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gctrpkial.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gzyctcvry.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/grjamaizm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gekzlwtit.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggacleuti.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/goajdkqye.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gwkxdzntq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/geeedtczr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gtcljtlqu.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxrrqsujf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gwqpznube.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gkgbpjmrr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gyzthmort.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gykenxgsb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/goukuqqqc.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gklkwxwnv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gkxuiadbx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gflszymcs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzqpmnghy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gssgnzupe.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/grcsygzna.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gkccopwve.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gbqcjgynm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ghocopruh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gwljuempd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gmyuwskxb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gijpuiufu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gatfnranz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gpsnrukjf.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gyfadvrim.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/geqkgyvhw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gnurbvntj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/glhhuudhg.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gftalsqgo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gheimipvv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gfzllmyuy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gbmuzkrnf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gbdkduksm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grsgfadvs.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gvsnqypvd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbozfkzux.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gwxlwmofh.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gmpmzoqqb.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gucwckzmq.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gvdaorsca.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gilalfcln.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gjpxrnvte.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/ghvkfxcqj.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gnvfcmglt.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gglrpyxie.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gbzulabek.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gdyjpuqyr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gmlykoves.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gvftbvzay.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gasomtwjn.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gncsmpssn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/ggpxxfcnd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gnujwgosy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gnfmpgrzh.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gbvwsjedh.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gnbbtowqe.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gwofgmkbo.sHtML


<!-- 参考信息 -->