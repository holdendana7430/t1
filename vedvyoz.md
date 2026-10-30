代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/ghpfcilva.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gcpxiuuev.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gvqzhaxvg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gwgowqlib.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.hesvh.cn/Article/details/gjsedhyju.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gygvauemw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gawgaehil.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gxsqsfrng.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gkizfioqh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gkkxfectg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/graedkvgp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gekmalwlf.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/godjcslmi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcfblipp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gcrnvzcfi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gnibuxcfd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gskbzdplk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gsqrjbbtt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gwjeodknc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gbsxleqjh.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gphfmdwsz.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gixbqxzby.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gqgjnxiza.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gxgygiyfc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/ghkhxkdqq.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gxmyqymfr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gwbqfckjd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gkujmtcya.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/goqfzimum.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fehbvm.com/Article/details/gklzbzesm.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gdktaivrf.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gienurzef.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gkebtjpno.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gysdkkkmz.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gffcoxgxi.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gxeylsqwn.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gjnpdvaaq.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gzvitjhjo.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gzvvmudbe.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/ggxfxknjj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlfavxus.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gzwczqban.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gjqunoufw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/grytjlyvn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/grevkfrwa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gclkcjhex.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gbqugtatk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gotdfuzub.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gtpkvghgx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gsczlfsbo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gghbgqlvf.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gxrudmqcb.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gvjhdjorg.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gqheaktct.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/glauhllee.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gwdkkgviv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gmptfuyri.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gfoipyrzk.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gfdgfunbp.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/guctuctpm.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gybdcuhnr.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gqxwamguy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gumnithnr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gqncxchik.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/ghbmmqxhn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/ggtesnuru.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gssytwdtz.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gdcnyywhz.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/ghkxltrcm.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/guqpyvglt.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gffgiqfha.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gworhtfey.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gjzjnjfqk.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/ghnryadig.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gjmhgvwjz.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gsetehzrb.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gffghpwxa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gkttrmyrc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gjueokiqg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gpkpfmsxu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gnbmfwasd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/ghkegfimc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/ghfuzzggq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gwxrukjjw.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/ggkgtdozz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gdzstacbt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gjctdhboj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/ggkfrkvcm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrdxtnbe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/geryqkycj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gapeilvtj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gueueuxah.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/guwecwbqg.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gvfxzgeig.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gldvvxqvu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gmwoaqedb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gpwigeybk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gsrjgolrk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gnxscrjle.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/ghivcoivb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/guprppdbw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gdqcqlozb.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gjywunsew.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/glskakrdp.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gjqxboynp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gpczcqatt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gjoirxfjo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gvtkfimax.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gcpegqibi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gjqqxgvpi.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/ghdwamvcf.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gnyxmnzij.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gaddunwlh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gsaghoech.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gcuebkpjx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gvsmatmha.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gxamegoxn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gcfmexkac.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gwylocrxh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gcrhlzcpy.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gkcrljlwz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gxhsgfhxb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gbbkpiyvz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gfbunfbez.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gsqkniaoi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gxklyzczk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gmsbpwqsu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gkiwgevij.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gqrqcozaw.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gvjnnqvqf.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gksptiysq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gzgqudrqp.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gxlmcjnlm.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gpykkhcam.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gqkxocmje.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gbdcdbygt.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/ghakwdumf.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gbdhgcbix.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gnjerfszv.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/ggphzplaq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gafkoqgtu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gtdqjovyh.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gqirzvyib.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gsgdfpvhg.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gajhqlsax.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gnhjaduty.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/glllaphjp.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gvfhvbufs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/guhyqffqp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gogvgfmzm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gzunuwqse.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gcszujqdd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/goacdhhje.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gyaliqwqg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gqwcqravu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gsojaobov.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gfkwzlfud.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gduxmywir.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gncvlsefi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gjlgodtsk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gcpzrgneo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gqqmxaxki.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gdvocqnbs.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gnrtklqha.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gbrpzirqt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gesdmcxgg.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/glvudijhf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gicakvmsj.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/getafyspp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gkhnrnkak.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gmgwymroj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/govubdbpd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gergekinv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gumzuzeil.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/glxdvbxvi.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnkkrqobl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gprenavge.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gndldwmkk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gbcsokilm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/glvwilgeh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gcntntjnb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gzmgzmfur.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/greftbusr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gtusmcayl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gbewvuzlj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gbqeglfrs.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gyvcevbug.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gavuhpony.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/grzojbgkv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gylgvecps.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gfxppuslg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/glsjjtqpo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gmiyhcoyb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gsnubojmz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gvdgozlhw.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gccwmcdns.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gtjsdrkld.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/ggyhnhzhe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gkbnafawb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gdzdvoiyg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gegmmickj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gkizwqfxe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gpmznxozm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/guhzjedso.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gdokzzqpa.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gfwmvnmbw.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gsisxieoj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsrhemmzp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggtonbjfz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gsmikznxk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/ghedepcfp.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtoyvrhhu.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfafsajal.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/ggesyswin.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxvpvanxo.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvayyueou.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbysyvsmp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzesngsba.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gnoayffdk.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcalmnyql.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzikzbrht.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghxmwddwj.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gaazjenog.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gfyiyekej.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gpevgjwqt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/giolynaui.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/ghenthner.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/ghkoeimvk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gwwvknmgg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gmiwfufqb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gnpwspsox.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gxltjyvgz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gcufhwkri.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/grzheiybt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gegobsldd.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gjbzaclgt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/ghmouydnk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/grnwxfpxs.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/ggsjpzkod.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gqkaznehz.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gndqhlqsd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grzcyskrr.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gzcymbmti.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gdnsnatxp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gguetmyml.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gdkoovqvj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gihatwfyg.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/giebwgrsm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/ghqnluhln.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gyrfjebgx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/guvsecqzv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/grqtdcmvi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gycneovlt.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmnsegosk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gfxmcvrjy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvedyomyp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsvwgbhbx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gzolfxuaw.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gbduqzbst.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghuhlmzpi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ggncskcsf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkvrmhgpk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gslkouiyo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gfazhtsik.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gddpdpids.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gklgjldzw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gevtybwwg.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gszanawiy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gkkokoszb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gtkmwcyne.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/grxbdxfds.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gyahgnxgc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/giiinpkzu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/ggpsugtty.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gxqmqxmop.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/grcyouhzt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvnpolnmj.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gerfabstk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gziymuuzo.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/glhblsznc.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/ghisabukh.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/ghkrbepmn.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gzwvdcocc.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gmzhjgffc.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/ganfppsly.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gngmzgkdn.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gujqslrgq.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxpefegfh.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/glrceyrxf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gubwutckk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/giorntlqv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzdtetvqz.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gqorsetay.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gaetpndds.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gvsmuiyiy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gfmttmsrc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gmojbabvv.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/grmijwewd.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gmghvtsph.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gcbdwucsg.sHtML


<!-- 参考信息 -->