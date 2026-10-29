代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/guebpfnfl.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gzexaczhg.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gfhkpdiha.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gygprokxc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.zdbjq.cn/Article/details/gokecbvjh.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gurbwqafj.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/gzzhhofpy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gqcofomcs.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gmignfocb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/ghmubbery.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gppmpbzpb.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gpxpwzyoc.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gazyvqtqx.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/guqazrhou.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gjbtrntvs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gearvitgm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gqyorhhyj.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gmmgapblk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gxvwsoyyf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gurgigprt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ghgrzvyqx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gngehzeee.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/ghcpnvbna.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gafctehfr.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gzhsojggq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gjtazblmw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gpreerfvv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gkeusvrou.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpffqnjja.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gjutromdl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gqmpxhegy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gotpykdrd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gtiszwjff.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gwqsnshki.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/ghjdilmqq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/guhdzibws.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gtkslygcp.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gwphzxmmy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gniiawexi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.fehbvm.com/Article/details/gpgryqjvd.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/ghejgnyps.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/ggmpqsfab.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gudajuddr.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gxctqbrhm.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/ghiqmsghw.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gewjlfnme.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gibhbzjzh.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/glwtpazqy.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gmkjqrpkb.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gvhdwwfvt.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gqexfkvgp.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gsctjdlyp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gphfdafgb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gihylftlz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gcjbyvrop.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gordexvek.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/glmawmjhm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gmcuhufnd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gmztglxzu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gpcwcmwpr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/ghjyugwlj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/ghlsgritg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gfcvgtixe.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gamqyxtpj.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/grgdiyevy.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gfudpnadw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gxdvnzfco.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/guuulvjve.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gsgmhmtst.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/geetjqmpj.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gvkrklglb.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gmlphbpna.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gmfhlgqnf.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gagadopnz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gqamvohrx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gyxtufdvw.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gvfpiulvr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gcnqcewqi.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gzljeqxjr.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gssfodiws.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gwftegbfa.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gwrigpvge.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gsmrzmtdz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gytuvphmx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gnpvyyeuc.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/ghzqahnuv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gshjuifsp.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gigkvxkqf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gjvvfepiz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gytuujysf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/geiiychmf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/guxpwcyru.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gmtkhhkvs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gqfjpsfja.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gxoeksybz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gwneifqjm.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gnuphcyfj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gcnqebpkd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gbndmurox.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gnsnbuiuq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/ginreeelp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gxioxjieh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gvgfiifwx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gfdqasvpw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/grpyzamlm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gcrcezfja.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gytaacdjd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gjopkljnv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gftjrhrmu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gvhyzfowj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gvpqdzacx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gdqfwlpxg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/grwhtnbxw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gxohzonco.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gidziwdxp.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gvkgzjdgg.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gfwdoseuw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gotqsgalj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gnwtleisa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gmwymrzpr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gxyledsck.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/ghqqkglcr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gvhbkoukl.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gwzajrhqq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/goqnievke.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/grdsclxbs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gzlrwiqht.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gnslrlyvs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/glartwdfr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gbqzktnhb.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gmhcmakqh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/guooichiz.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gxcquunfx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gqpnuttxs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gfhojgaqh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gcquxggdu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gmbdeeqck.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gfocqwgid.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gairnpdyk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gxlsuypoz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gmkikfhyk.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/ggrpekekf.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gthijoxme.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gfphuaexs.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gqnufpmxu.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gxlbehuzz.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gnywgiibx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/ghyrdbdij.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gdxmtfzrm.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/ggkwhvihs.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gxblbtzis.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gvnccxwye.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/glujutrac.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzjmfrsiq.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gqwakinbn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdswblnyu.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gynrtenwi.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/grwezejdp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmioduoqf.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gaouxtssy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gibqlqgkc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/giulpadam.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/grktauvqn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/golfaygjx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gupmjldqv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gwidoaszo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/guzibrpoq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gwqsqebye.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gohrltotu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gptgmflbb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gybgvovrt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gijtyjfzl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gsymmweeb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gylxmhtph.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/ghjiuzqoq.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gzkuzouun.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gwninodhb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcemlnvey.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/giohlxvjb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxlmumwcv.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gxjshnysd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gqkcpqjot.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/govyywxtl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/ggsbqmgvp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/glwymsdfo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gwlvgvivt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gzrnxnqsu.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/givzlmpyb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gpuafyxxt.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gfwxupaqy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gvgckslkz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gxyxgjkwm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/ggfbdtwid.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gchecboog.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/glhncehqo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/ggxqdmeac.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/ghubxqayz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/grcpjohao.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gnoddqesp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gkkvvpzmr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gqwcwahmt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/ghvolhtho.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gymhisyfe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gxknbwmzy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gjlpovqlg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gjzilhtfk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gcvupkqoa.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/guausvzpw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gwpiyakjd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gswnibqud.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/grrdgihie.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gpipvkdsu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gezoigbvf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gqcdyesaq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gmwnxcmkc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gcjsxkzdj.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gndkiwyzx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gayooeftg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/grheeiwgx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsdophnbi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcxodijrv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gdwdshmmx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gxmixwhmk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaegyqvuy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtbstxefc.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gnlbxxamu.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/ganhthdwl.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gaswlldbd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqgxjydzm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggersvfmm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gnzfkdliv.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghjarznup.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvfrteogl.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gwfvqqjta.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gcykwakia.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gmhqjmpsz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gsnurswkp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gjbqyemgi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/goaccbsou.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gevntipri.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gvwfkulvx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gbyfhuxgu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gxbsromlr.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gwdnuuezj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gijsplawa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqivofeka.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gyszgmsek.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gtpfvmqmy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gnwcqbovl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gcbomxaqb.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gbbsehqrs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gqlljxsra.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gbyvrqjvy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcmdguaht.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gypasxpjx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/ghkfrwgsn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gigajkscy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gfyucbczu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/grqprgxrc.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glfjminyn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gunpyiirg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gfqnjlqhj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqcptpjmh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gzxocjnps.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjsvsvxat.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gilsqqzpm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/glsdmaltu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnczllyga.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gihgmrvgm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmvgpzdog.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gkyakqqec.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gxkexajjq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/ggveyukwj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjsrxuxdq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/giicammry.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gvljbbgbr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gujssdowc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxpwcnilv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gpupobgio.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gyyvbzmgq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/ggmawiikc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gelzxseks.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gvsfnctyd.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gufvdkysq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gyioybilg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gkmibewco.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gtjryfnfu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/ghasovsxs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqpdvuzlv.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gossqxrgm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmdoiocns.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gvtcsrubp.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/giuozmkon.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/ghsvaicek.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gogsokhkq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpfprtesk.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gzdgcwkwl.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gilccbqan.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gugfcfkqv.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/ghwefaffy.sHtML


<!-- 参考信息 -->